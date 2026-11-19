# 21BenchMixIndex

编码模型混合指数（Coding Model Mixture Index）。把 AA Coding Agent、AA Intelligence、VALS、CursorBench、FrontierSWE、ProgramBench 的公开数据压成一个可复算、可修改的编码模型决策工具。

这是一个指数，不是榜单。

## 打开

- 直接打开 `index.html`：单文件、零外部依赖，字体使用本机 Sarasa Mono / 更纱黑体等宽。
- GitHub Pages：把仓库根目录设为 Pages 源，`index.html` 即入口页。
- 数据版本：见 `index.html` 的 `meta[name="release-date"]`（YY/MM/DD）。更新数据时只改这一处。

## 页面内容

- 主表默认只显示原始 8 项中 **≤2 项缺分** 的模型；可切到“全部”查看参考池。
- 缺分处理：CB 缺失走公式回退；PB / VCB100 / FSWE 缺失按“推荐拟合 / 保守地底 / 按 0 计”处理，也可在抽屉里逐项手填。
- 归一化：`Fable 5.2 = 1` / `最高分 = 1` / `原始分`。
- AA 对照：与 **AA Intelligence Index v5.0.1** 做同锚点刻度与缺口比较。
- 实际分布：MIN / P25 / MEDIAN / P75 / MAX + 点阵直方图，不预设分档阈值。
- 明暗双主题；柱状图按实验室品牌色区分。
- 支持 CSV 导出、添加自定义模型、拟合明细、复制引用。

## 数据来源

- [AA Coding Agent Index v2.1](https://artificialanalysis.ai/agents/coding-agents)
- [AA Intelligence Index v5.0.1](https://artificialanalysis.ai/leaderboards/models)
- [VALS VCB 1-100 v1.1](https://www.vals.ai/benchmarks/vcb-1-100-v1-1)
- [VALS Vibe Code Bench v1.1](https://www.vals.ai/benchmarks/vibe-code)
- [VALS ProgramBench](https://www.vals.ai/benchmarks/programbench)
- [CursorBench 4.1](https://cursor.com/cursorbench)
- [FrontierSWE v2](https://www.frontierswe.com/)
- [Terminal-Bench 4.1](https://www.tbench.ai/)

底层 benchmark 数据与商标归各发布方所有；本仓库只做聚合与可视化。

## 许可

本作品采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 国际许可协议。署名、非商业、相同方式共享。商用授权请联系作者。

## 反馈

- GitHub Issue / PR
- Bilibili：<https://space.bilibili.com/334394212>
- GitHub：<https://github.com/2youg1>

显示效果在作者本机的 LibreWolf 浏览器上表现不错；不保证 100% 全配置兼容。
