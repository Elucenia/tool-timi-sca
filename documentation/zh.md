<!-- ELUCENIA technical documentation · timi-sca · zh · no clinical/professional/rights approval -->

# TIMI 评分（非 ST 段抬高型急性冠脉综合征）

[条件、来源与许可](https://elucenia.org/zh/tools/timi-sca)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 年龄 ≥ 65 岁

`idade`

### ≥ 3 项冠状动脉疾病危险因素

`fr`

### 已知冠状动脉狭窄 ≥ 50%

`dac`

### 过去 7 天使用阿司匹林

`aas`

### 24 小时内 ≥ 2 次心绞痛发作

`angina`

### ST 段偏移 ≥ 0.5 mm

`st`

### 坏死标志物升高

`marc`

## 方法版本

TIMI UA/NSTEMI/Antman 2000：7因素各0–1，总计0–7；不含TIMI STEMI

## 已记录的公式

每项存在的项目1分（总分0至7）。

## 限制与适用人群

此TIMI版本为不稳定型心绞痛和非ST段抬高型心肌梗死中14天复合结局而开发，并非用于ST段抬高型心肌梗死（STEMI）的TIMI版本。因素有特定的时间及临床定义。没有对应评估与指南时，历史试验中的发生率不能确定个体风险或当前治疗。

## 参考文献

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

早期侵入性策略获益

| 结果详情 | |
| --- | --- |
| 14 天内死亡、心肌梗死或紧急血运重建 | 13.2% |


### 2

早期侵入性策略获益

| 结果详情 | |
| --- | --- |
| 14 天内死亡、心肌梗死或紧急血运重建 | 26.2% |


### 3

低风险

| 结果详情 | |
| --- | --- |
| 14 天内死亡、心肌梗死或紧急血运重建 | 4.7% |

