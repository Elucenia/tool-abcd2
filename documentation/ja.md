<!-- ELUCENIA technical documentation · abcd2 · ja · no clinical/professional/rights approval -->

# ABCD²スコア

[条件・出典・許諾](https://elucenia.org/ja/tools/abcd2)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 年齢 ≥ 60 歳

`idade`

### 初回評価の血圧 ≥ 140/90 mmHg

`pa`

### 臨床症状

`clinica`

- `0` — その他の症状
- `1` — 脱力を伴わない言語障害
- `2` — 片側の脱力

### 症状の持続期間

`duracao`

- `0` — \< 10 min
- `1` — 10 ～ 59 min
- `2` — ≥ 60 min

### 糖尿病

`dm`

## 方法の版

ABCD²/Johnston 2007：年齢/血圧/所見/持続/糖尿病、合計0–7

## 記載された計算式

A年齢≥60：1、B血圧≥140/90：1、C臨床：片側脱力2・脱力なしの言語障害1、D持続≥60 min：2・10～59 min：1、D糖尿病1。合計0～7。

## 限界・対象集団

一過性脳虚血発作（TIA）の診断後に用いる予後スコアで、主に2日以内の脳卒中リスクが研究され、7日および90日についても追加解析されました。TIAの診断を確定するものではありません。原コホートで観察された確率は、普遍的な個人の予測を表すものではありません。

## 参考文献

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

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
