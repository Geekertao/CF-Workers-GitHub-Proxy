# CF-Workers-GitHub-Proxy
#### 2025.5.25修改，现已支持github api加速！🎉🎉🎉
## 桌面端预览
![desktop](src/desktop.png)
## 移动端预览
![mobile](src/mobile.png)
## 简介
github release、archive以及项目文件的加速项目，支持clone，github api，Cloudflare Workers 版本

## 使用

直接在copy出来的url前加`https://ghfile.geekertao.top/`,`https://github.dpik.top/`或`https://gh.felicity.ac.cn/`即可

也可以直接访问，在input输入

***大量使用建议自行部署，以上域名仅为演示使用，可以轻量使用。***

访问私有仓库可以通过

`git clone https://user:TOKEN@ghfile.geekertao.top/https://github.com/xxxx/xxxx`，`git clone https://user:TOKEN@github.dpik.top/https://github.com/xxxx/xxxx`，`git clone https://user:TOKEN@gh.felicity.ac.cn/https://github.com/xxxx/xxxx` [#71](https://github.com/hunshcn/gh-proxy/issues/71)

以下都是合法输入（仅示例，文件不存在）：

- 分支源码：https://github.com/hunshcn/project/archive/master.zip

- release源码：https://github.com/hunshcn/project/archive/v0.1.0.tar.gz

- release文件：https://github.com/hunshcn/project/releases/download/v0.1.0/example.zip

- 分支文件：https://github.com/hunshcn/project/blob/master/filename

- commit文件：https://github.com/hunshcn/project/blob/1111111111111111111111111111/filename

- gist：https://gist.githubusercontent.com/cielpy/351557e6e465c12986419ac5a4dd2568/raw/cmd.py

- api：https://api.github.com/repos/Geekertao/CF-Workers-GitHub-Proxy
## Workers 部署方法
### 部署 Cloudflare Worker：

   - 在 Cloudflare Worker 控制台中创建一个新的 Worker。
   - 将 [index.js](./index.js)  的内容粘贴到 Worker 编辑器中。

## 项目文件说明

-  **`index.js`**  ：基于 [gh-proxy](https://github.com/hunshcn/gh-proxy) 项目的 [`index.js`](https://github.com/hunshcn/gh-proxy/blob/master/index.js) 修改，已将 `ASSET_URL` 配置为我的 GitHub Pages 地址。
- **自定义配置**：如需修改 GitHub Pages 地址，请前往 [Geekertao.github.io](https://github.com/Geekertao/Geekertao.github.io/tree/main/gh-proxy) 仓库下载源码后编辑。
- **页面代码**：HTML 部分参考自 [CF-Workers-GitHub](https://github.com/cmliu/CF-Workers-GitHub/) 项目的 [`_worker.js`](https://github.com/cmliu/CF-Workers-GitHub/blob/main/_worker.js) 文件。

# 致谢
[gh-proxy](https://github.com/hunshcn/gh-proxy)、[jsproxy](https://github.com/EtherDream/jsproxy/)、[CF-Workers-GitHub](https://github.com/cmliu/CF-Workers-GitHub/)

# 赞助
<a href="https://afdian.com/a/Geekertao" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/💵_爱发电-FF4D4D?style=flat-square&logo=usd&logoColor=white" alt="爱发电" style="max-height: 50px;">
    </a>


