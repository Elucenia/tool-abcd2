<!-- ELUCENIA technical documentation · abcd2 · zh · no clinical/professional/rights approval -->

# ABCD² 评分

[条件、来源与许可](https://elucenia.org/zh/tools/abcd2)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 年龄 ≥ 60 岁

`idade`

### 初次评估血压 ≥ 140/90 mmHg

`pa`

### 临床表现

`clinica`

- `0` — 其他症状
- `1` — 言语障碍，无无力
- `2` — 单侧无力

### 症状持续时间

`duracao`

- `0` — \< 10 min
- `1` — 10 至 59 min
- `2` — ≥ 60 min

### 糖尿病

`dm`

## 方法版本

ABCD²/Johnston 2007：年龄/血压/临床/时长/糖尿病，总分0–7

## 已记录的公式

A年龄≥60：1 · B血压≥140/90：1 · C临床：单侧无力2，无无力的言语障碍1 · D时长≥60 min：2，10至59 min：1 · D糖尿病1。总分0至7。

## 限制与适用人群

这是在诊断短暂性脑缺血发作（TIA）后使用的预后评分，主要研究2天内卒中风险，并对7天及90天风险作了额外分析。它不能确认TIA诊断。原始队列中观察到的概率并非普遍适用的个体预测。

## 参考文献

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
