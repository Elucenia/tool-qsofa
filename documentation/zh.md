<!-- ELUCENIA technical documentation · qsofa · zh · no clinical/professional/rights approval -->

# qSOFA（快速 SOFA）

[条件、来源与许可](https://elucenia.org/zh/tools/qsofa)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 呼吸频率 ≥ 22 irpm

`fr`

### 精神状态改变（Glasgow \< 15）

`mental`

### 收缩压 ≤ 100 mmHg

`pas`

## 方法版本

qSOFA/Sepsis-3/Seymour 2016：呼吸≥22/收缩压≤100/意识改变，0–3；SSC 2021不建议单独筛查

## 已记录的公式

各1分：呼吸频率≥22/min、意识状态改变、收缩压≤100 mmHg。2分及以上为阳性。

## 限制与适用人群

qSOFA2016是用于疑似感染成人的风险评估工具，并非诊断方法，也不是可单独用于排除脓毒症的检测。低分不能消除临床怀疑。SSC2021建议不要将qSOFA作为唯一的筛查工具；SSC2026官方指导仍优先推荐其他医院筛查工具。急诊评估和治疗不应等待评分结果。这一成人阈值不能确立其在儿童中的适用性。

## 参考文献

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

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
