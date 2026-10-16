# Fed-Watch

美联储流动性监测面板（Fed Liquidity & Market Stress Monitor）。

## 面板

- **在线访问**：https://666677778888.github.io/Fed-Watch/ （GitHub Pages，每个交易日更新）

- **文件**：[`fed_monitor.html`](./fed_monitor.html)（单文件、离线可用，浏览器直接打开）
- **数据源**：St. Louis Fed FRED API（31 系列）+ OFR Financial Stress Index + Yahoo Finance (^MOVE)
- **更新频率**：每个交易日自动更新并推送（数据日频/周频/月频混合，页面内标注各系列日期）

## 内容

| 板块 | 指标 |
|---|---|
| 美联储流动性 | Fed 总资产 (WALCL)、TGA、逆回购 ONRRP、净流动性（=总资产−TGA−ONRRP）、M2 及同比 |
| 风险与价格 | VIX、MOVE、Broad USD、TIPS 实际收益率 5Y/7Y/10Y/20Y/30Y、名义 10Y/30Y、30Y 房贷利率 PMMS |
| 信用与中介 | HY/IG OAS、银行准备金、银行现金缓冲、OFR FSI |
| 融资与管道 | SOFR、IORB、联邦基金目标上限、EFFR、SRF、SOFR−IORB 利差 |

每个 KPI 卡片附带 **5 年滚动窗口分位数**（按月对齐更新）。

## 说明

- 面板为静态 HTML（数据内嵌），无后端依赖
- Chart.js 4.4 via CDN，离线打开时图表区不渲染，数据卡片仍可读
