### 这是什么？

hztl-ui 是 ERP 使用的 ui 框架,基于 element-ui。对 ERP 常用的功能和业务进行了封装.

ERP 中使用的 hztl-ui 由两部分构成:1.远程的 hztl 项目,2.components 中的 hztl。在 components 中的 hztl 中引入和远程的 hztl，并注册了组件,再在 main.ts 中引入并使用。

### 如何使用？

```javascript
import HztlUi from "hztl-ui";

Vue.use(hztl);
```

### 如何维护

远程地址: [https://gitlab.threesoft.cn/three-front/hztl-ui](https://gitlab.threesoft.cn/three-front/hztl-ui)

### 更新 UI 框架,怎么做？

1. 首先,将 hztl 的远程仓库 clone 下来
2. `npm start` 启动项目,开发并调试
3. 调试完成后`npm run build`,打包项目
4. 提交代码到远程仓库
5. `git log`查看最新一次 commit 的 hash 值
6. 到 ERP 项目中,编辑`package.json`中的 hztl 插件,将 hash 值替换为第 5 步中的最新的 hash 值。
7. ERP 项目`yarn`,安装最新的 hztl-ui
