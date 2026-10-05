<!-- ELUCENIA technical documentation · timi-sca · ja · no clinical/professional/rights approval -->

# TIMIスコア（非ST上昇型急性冠症候群）

[条件・出典・許諾](https://elucenia.org/ja/tools/timi-sca)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 年齢 ≥ 65 歳

`idade`

### 冠動脈疾患の危険因子 ≥ 3項目

`fr`

### 既知の冠動脈狭窄 ≥ 50%

`dac`

### 過去7日間のアスピリン使用

`aas`

### 24時間で狭心症発作 ≥ 2回

`angina`

### ST偏位 ≥ 0.5 mm

`st`

### 壊死マーカー上昇

`marc`

## 方法の版

TIMI UA/NSTEMI/Antman 2000：7因子0–1，合計0–7；TIMI STEMIを含まない

## 記載された計算式

該当する各項目1点（合計0～7）。

## 限界・対象集団

このTIMI版は、不安定狭心症とST上昇を伴わない心筋梗塞における14日の複合転帰について開発されたもので、STEMI用のTIMI版ではありません。各因子には具体的な時間的・臨床的定義があります。歴史的な試験の率だけでは、対応する評価とガイドラインなしに個人のリスクや現在の治療は決まりません。

## 参考文献

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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
