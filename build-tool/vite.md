1. 由原生 ESM 驱动
2. 基于浏览器原生 ES imports 开发
3. 在服务器端按需编译返回，完全跳过了打包这个概念
4. 在生产环境下基于 Rollup 打包
   

### run up

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
   6. git push -u origin master