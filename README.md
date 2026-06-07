# YOLO React

这是一个部署在 GitHub Pages 上的前端目标检测演示项目。项目使用 React 构建页面，并在浏览器端加载 ONNX Runtime Web 相关资源，用于运行 YOLO/ONNX 模型推理演示。

在线访问：

[https://aqwddda.github.io/yolo-react/](https://aqwddda.github.io/yolo-react/)

## 功能

- 浏览器端运行目标检测演示
- 使用 ONNX Runtime Web 的 WASM 文件进行推理支持
- 前端静态页面部署到 GitHub Pages
- 无需后端服务即可访问演示页面

## 技术栈

- React
- JavaScript
- ONNX Runtime Web
- WebAssembly
- GitHub Pages

## 仓库结构

```text
yolo-react/
├── index.html
├── app.bundle.js
├── app.bundle.js.LICENSE.txt
├── ort-wasm.wasm
├── ort-wasm-simd.wasm
├── ort-wasm-threaded.wasm
└── ort-wasm-simd-threaded.wasm
```

## 如何访问

直接打开在线页面：

```text
https://aqwddda.github.io/yolo-react/
```

## 本地预览

如果想在本地预览静态文件，可以使用任意静态服务器，例如：

```bash
python -m http.server 8000
```

然后访问：

```text
http://127.0.0.1:8000/
```

## 说明

当前分支主要保存 GitHub Pages 部署后的静态构建产物。如果后续继续维护，建议保留源码分支，例如 `main` 或 `dev`，将 React 源代码、模型加载逻辑和构建脚本放在源码分支中，`gh-pages` 分支只用于部署。