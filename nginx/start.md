### 1、安装包管理工具brew

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"


### 2、安装nginx

brew install nginx


### 3、启动nginx

sudo nginx


### 4、验证nginx配置文件

sudo nginx -t


### 5、进入本地nginx路径

cd /usr/local/etc/nginx/

open .

###  6、创建项目nginx配置文件，放置在servers文件夹内

mkdir servers && cd servers  // 创建servers文件夹存放配置文件

touch <11>.conf //  创建nginx配置文件

### 7、安装 Gas Mask 修改 mac 本机 host 文件

浏览器域名访问，通过host映射ip，请求对应ip，被nginx拦截，进行服务代理，解决跨域问题。

### 8、停止nginx
sudo nginx -s stop

### 9、重启：
sudo nginx -s reload

### 10、查看进程： 
ps aux|grep nginx

