# ABS on Go2

陈聪的四足机器人项目展示页：Go1 → Go2 跨平台适配、仿真训练与真机部署。

这是基于 Agile But Safe 的个人复现与工程实践展示，不是原论文官方项目页，也不是完整训练代码仓库。

## 页面结构

- `index.html`：独立静态首页，实机演示在前，仿真演示在后。
- 实机区：4 个竖屏位置，桌面端一行四列；平板和手机端两列。
- 仿真区：4 个横屏位置，桌面端 2 × 2；手机端单列。
- 点击已加载素材可放大，Escape 或关闭按钮退出。
- 缺失素材显示占位卡，不伪装成已完成的演示。
- `engineering-notes.html`：保留改版前的完整原页面，包含未完善的工程记录。

## 添加 8 个 GIF

把文件复制到 `static/gifs/`，使用以下文件名，顺序从左到右、从上到下：

```text
static/gifs/
├── real-01.gif
├── real-02.gif
├── real-03.gif
├── real-04.gif
├── sim-01.gif
├── sim-02.gif
├── sim-03.gif
└── sim-04.gif
```

`real` 为实机；`sim` 为仿真。保留 GIF 原始画幅，页面不会裁剪主体。文件名区分大小写。当前仓库已预留全部展示位，正式 GIF 尚未导入。

Mac 上的 `/Users/...` 是本机路径，不能直接用作网站图片地址。请复制文件到仓库中的上述目录并提交。先复制后重命名即可，不必改动原文件。

场景标题暂用中性编号。确认完整演示内容后，可在 `index.html` 中修改对应 `h3`、`data-title`、`aria-label` 和 `alt`。实机、仿真编号不代表同条件的对照实验；演示本身不证明统计成功率或性能提升。

## 本地预览

首页无需构建工具或第三方 CDN。可用浏览器打开 `index.html`；也可在仓库根目录执行 `python3 -m http.server 8000`，访问 `http://localhost:8000`。没有正式 GIF 时看到占位图是正常情况。

## 来源与许可

- ABS 原项目：https://agile-but-safe.github.io/
- ABS 官方代码：https://github.com/LeCAR-Lab/ABS
- 原网页模板：Nerfies，https://nerfies.github.io/

原站点基于 Nerfies 模板；本版重新整理首页布局并保留来源致谢。网站沿用 [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) 许可说明。原算法和原项目的权利归其各自作者所有。
