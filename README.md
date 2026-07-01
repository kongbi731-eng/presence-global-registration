# 出海项目多策略落地日历甘特看板

一个开箱即用的单文件前端看板，用原生 JavaScript 渲染月视图日历甘特图，支持按发布策略自动过滤并重排任务时间线。

## 功能

- 发布策略切换：双端齐发、仅 Google Play、仅 App Store
- 点击日期设置项目 Day 1
- 按任务依赖自动计算开始日期和结束日期
- 日历格内跨日期甘特条展示
- 任务完成度 0%-100% 调整
- 顶部指标和右侧任务列表实时刷新

## 使用

直接打开 `index.html` 即可使用。

## GitHub Pages 部署

1. 新建一个 GitHub 仓库
2. 上传 `index.html` 和 `README.md`
3. 进入仓库 `Settings` -> `Pages`
4. Source 选择 `Deploy from a branch`
5. Branch 选择 `main`，目录选择 `/root`
6. 保存后等待 GitHub 生成访问链接

## 数据说明

当前版本的数据保存在浏览器本地 `localStorage` 中。上传到 GitHub Pages 后，所有人都可以访问页面，但每个人填写的 Day 1、策略和完成度只保存在自己的浏览器里。

如果需要多人共享填写，需要接入云端数据源，例如 Supabase。
