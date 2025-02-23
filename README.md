# CF-Workers-GitHub-Proxy
![img](./desktop.png)
![img](./mobile.png)
## 简介
github release、archive以及项目文件的加速项目，支持clone，Cloudflare Workers 版本

## 使用

直接在copy出来的url前加`https://ghfile.geekertao.top/`即可

也可以直接访问，在input输入

***大量使用建议自行部署，以上域名仅为演示使用，可以轻量使用。***

访问私有仓库可以通过

`git clone https://user:TOKEN@ghfile.geekertao.top/https://github.com/xxxx/xxxx` [#71](https://github.com/hunshcn/gh-proxy/issues/71)

以下都是合法输入（仅示例，文件不存在）：

- 分支源码：https://github.com/hunshcn/project/archive/master.zip

- release源码：https://github.com/hunshcn/project/archive/v0.1.0.tar.gz

- release文件：https://github.com/hunshcn/project/releases/download/v0.1.0/example.zip

- 分支文件：https://github.com/hunshcn/project/blob/master/filename

- commit文件：https://github.com/hunshcn/project/blob/1111111111111111111111111111/filename

- gist：https://gist.githubusercontent.com/cielpy/351557e6e465c12986419ac5a4dd2568/raw/cmd.py

## Workers 部署方法
### 部署 Cloudflare Worker：

   - 在 Cloudflare Worker 控制台中创建一个新的 Worker。
   - 将 [index.js](https://github.com/Geekertao/gh-proxy/blob/main/index.js)  的内容粘贴到 Worker 编辑器中。

## [index.js](https://github.com/Geekertao/gh-proxy/blob/main/index.js)根据[gh-proxy](https://github.com/hunshcn/gh-proxy)中的[gh-proxy](https://github.com/hunshcn/gh-proxy/blob/master/index.js)修改为我的github pages地址，页面代码由[CF-Workers-GitHub](https://github.com/cmliu/CF-Workers-GitHub/)中的代码修改而来。

# 致谢
[gh-proxy](https://github.com/hunshcn/gh-proxy)、[jsproxy](https://github.com/EtherDream/jsproxy/)、[CF-Workers-GitHub](https://github.com/cmliu/CF-Workers-GitHub/)
