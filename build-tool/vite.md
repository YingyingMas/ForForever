
### vite run up

1. 开始我的第一个vite应用： npm init vite-app my-first-vite-app
    
    /Users/dk/.npm/_npx/25529/lib/node_modules/create-vite-app/node_modules/fs-extra/lib/mkdirs/make-dir.js:85
        } catch {
                ^
    SyntaxError: Unexpected token {
        at createScript (vm.js:80:10)
        at Object.runInThisContext (vm.js:139:10)
        at Module._compile (module.js:617:28)
        at Object.Module._extensions..js (module.js:664:10)
        at Module.load (module.js:566:32)
        at tryModuleLoad (module.js:506:12)
        at Function.Module._load (module.js:498:3)
        at Module.require (module.js:597:17)
        at require (internal/module.js:11:18)
        at Object.<anonymous> (/Users/dk/.npm/_npx/25529/lib/node_modules/create-vite-app/node_modules/fs-extra/lib/mkdirs/index.js:3:44)

    初次执行报错如上，node版本8.16.0，切换至14.11.0，问题解决，输出如下：

    npx: 7 安装成功，用时 7.824 秒
    Scaffolding project in /Users/dk/Documents/workspace/self/my-first-vite-app...

    Done. Now run:

    cd my-first-vite-app
    npm install (or `yarn`)
    npm run dev (or `yarn dev`)

2. 创建仓库并上传至GitHub
   1. git init
   2. git add -A
   3. git commit -m "init"
   4. 在GitHub上面创一个空的仓库
   5. git remote add origin git@github.com:YingyingMas/my-first-vite-app.git
   6. git push -u origin 
   


### 回想一下webpack
1.  webpack 使用 map 存放模块 id 和路径，使用 webpack_require 方法获取模块导出，
2. 不管某个模块的代码是否执行到，这个模块都要打包到 bundle 里，
3. 随着项目越来越大打包后的 bundle 也越来越大。



### vite

1. ESM```<script type="module" src="/src/main.js"></script>```
   - script module 是 ES 模块在浏览器端的实现，
   - 在浏览器端使用 export、import 的方式导入和导出模块，
   - 浏览器将对其内部的 import 引用发起 http 请求获取模块内容，
   - 省略了对模块的组装，不需要生成 bundle，
   - ESM 天生按需加载，只有 import 的时候才会去按需加载。
   
2. 提供 web server，借用 koa 启动服务
   
3. 拦截浏览器对模块的请求并返回处理后的结果
   
    以往引用 node_modules 模块使用import xxx from 'xxx'，由 Webpack 等工具找到模块的具体路径进行打包。
    但浏览器不知道项目里有 node_modules，只能通过相对路径或绝对路径查找。

    vite：
    - 在 koa 中间件里获取请求体，
    - 通过 es-module-lexer 解析 import 内容
    - 将 import 的资源为绝对路径的视为 npm 模块
    - ```import { createApp } from 'vue'```变为```import { createApp } from '/@modules/vue.js'```
    - 判断路径是否以 /@module/ 开头
    - 去node_module找到这个库

4. 编译vue、css、ts等文件
   - vite 拦截对模块的请求并执行实时编译。 