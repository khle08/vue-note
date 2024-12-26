
`Node.js` 与 `npm` 的关系非常类似 `python` 与 `pip` 的关系，只不过 `npm` 除了包管理功能之外还可以用来参与项目的开发，而 `pip` 只是单纯的包管理工具。下载方法只需要根据官网步骤即可顺利完成。

修改 `npm` 镜像的方法：
```bash
# 淘宝
npm config set registry https://registry.npmmirror.com/
```

查看是否修改成功：
```bash
npm config get registry
```

除了官方的 `npm` 之外，还有另外以下两种工具可以用来开发前端应用：
```bash
npm install -g pnpm  # ... (1)
npm install -g yarn  # ... (2)
```

其中 `-g` 表示 global 全局安装，如果要通过 yarn + vite 的方法来开发项目，通过以下指令实现：
```bash
yarn create vite
yarn
yarn dev
```


