# 粒子流体实验室 · Particle Fluid Lab

二维 Position-Based Fluids（PBF）粒子流体实验台。单文件 HTML，双击即用，无需构建、无外部依赖。

## 在线体验

- 发布版：https://4mdwqmzrj60qt.doubao.link/app/app_17hzwhvt34k
- GitHub Pages：根目录已有 `index.html`，可在仓库 Settings → Pages 中选择 **Deploy from a branch → main → / (root)** 启用。

## 仓库结构

| 路径 | 说明 |
| --- | --- |
| `index.html` | 可直接运行的完整页面，也是 GitHub Pages 入口 |
| `src/粒子流体实验室.html` | 原始源码归档，与 `index.html` 内容一致 |
| `src/README.md` | 源码与运行说明 |
| `THIRD_PARTY_NOTICES.md` | 第三方依赖与许可说明 |

## 功能

- PBF 密度约束 + XSPH 粘性 + 涡量约束 + 表面张力
- 逐粒子动力粘度 ν、壁面摩擦 μw、流体组别
- 清水 / 蜂蜜 / 轻油 / 水银 / 双流体五种材料预设
- 液体 / 粒子 / 速度 / 压力 / 粘性 / 摩擦六种视图
- 搅拌、吸引、排斥、注入、障碍五种交互工具
- 自动滴落、表面风、振动台、摇晃、注水、重置、PNG 导出
- 响应式中文界面，桌面与手机均可操作

## 运行

直接用 Chrome / Edge 打开 `index.html` 或 `src/粒子流体实验室.html`（需要 WebGL2）。也可以在本目录启动任意静态服务器后访问。

## 说明

浏览器端实时模拟，不是工程级 CFD；参数用于交互演示与教学观察。云主机软件渲染实测约 25–45 FPS，真实 GPU 通常更高；密度误差约 1.6%–2.4%。
