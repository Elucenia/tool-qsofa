<!-- ELUCENIA technical documentation · qsofa · ja · no clinical/professional/rights approval -->

# qSOFA（簡易SOFA）

[条件・出典・許諾](https://elucenia.org/ja/tools/qsofa)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 呼吸数 ≥ 22 irpm

`fr`

### 精神状態の変化（Glasgow \< 15）

`mental`

### 収縮期血圧 ≤ 100 mmHg

`pas`

## 方法の版

qSOFA/Sepsis-3/Seymour 2016：呼吸数≥22/収縮期≤100/意識変容、0～3、SSC 2021は単独スクリーニング非推奨

## 記載された計算式

各1点：呼吸数≥22/min、意識変容、収縮期血圧≤100 mmHg。2点以上で陽性。

## 限界・対象集団

qSOFA2016は、感染が疑われる成人のリスク評価のための指標です。診断そのものでも、単独で敗血症を除外する検査でもありません。低スコアでも臨床的な疑いは否定されません。SSC2021は、qSOFAを唯一のスクリーニング指標として使用しないことを推奨しています。SSC2026の公式ガイダンスでも、病院でのスクリーニングには他の指標が優先されています。緊急の評価と治療を、スコアの算出まで待ってはいけません。この成人の閾値は、小児への適用を確立するものではありません。

## 参考文献

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

qSOFA陰性（< 2）

敗血症を除外するものではありません。引き続き再評価し、臓器障害が疑われる場合はSOFAを算出してください。


### 2

qSOFA陽性（≥ 2）：院内死亡リスクが高い

臓器障害（SOFA）を調べ、敗血症バンドルを開始し、ICUを検討してください。


### 3

qSOFA陽性（≥ 2）：院内死亡リスクが高い

臓器障害（SOFA）を調べ、敗血症バンドルを開始し、ICUを検討してください。

