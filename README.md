# ULI-COLOR｜構造思考色彩モデル

**ULI-COLOR（User-Led Inference Color Model）**は、GPTなどの生成AIにおける「思考構造」をRGB＋明度（Lightness）の4次元で評価・可視化し、ユーザーが色彩的に対話構造を再設計・制御するための構造モデルです。

## 🎯 目的

- GPTの出力に含まれる【仮説性／構造性／事実性／テンション】の比重を、色で可視化する。
- ユーザーが色を通じて「思考構造のフィードバック」を行う新しいUI/UXモデルを提案。
- 言語だけでなく、視覚的・構造的にAIと対話を編集する方法を実験的に探る。

## 🧠 構想モデル（ULI-COLOR）

| 色成分 | 概要 |
|--------|------|
| 🔴 Red | 仮説性・直感・飛躍的展開（Hypothesis / Intuition） |
| 🟢 Green | 構造性・論理整理・因果連結（Structure / Logic） |
| 🔵 Blue | 事実性・根拠重視・データ依拠（Factual / Evidence） |
| ⚪ Lightness | テンション・軽妙さ・思考の軽重（Tension / Tone） |

## 🔁 フィードバック・ループ構造

ユーザーの問い → GPT出力（＋RGBL構造評価）  
→ ユーザーが「もっと青く」「もう少し軽く」と色でフィードバック  
→ GPTが構造を調整して再出力（このループが繰り返される）

🌀 詳細は `images/github_diagram.png` を参照。

## 🧪 実装試作（GPTs）

- 評価プロンプト → `prompts/base_prompt.txt`
- 色誘導例 → `prompts/sample_feedback.txt`
- 実際の出力例 → `samples/example_output_1.md`

## ✨ 副産物：自己比較能力の発現

この構造評価を導入した結果、GPTが自分の出力の構造的変化を自己言及するという副産物が観察されました。

## 📜 ライセンス

本プロジェクト「ULI-COLOR」は、Creative Commons 表示-非営利-継承 4.0 国際ライセンス（CC BY-NC-SA 4.0）のもとで公開されています。

- ✅ 非営利目的での使用、引用、改変、共有が可能です。
- ✍️ 二次利用時にはクレジット（著者名・リンク）の明示をお願いします。
- 🔁 派生作品も同じライセンス（CC BY-NC-SA 4.0）で公開してください。
- 💼 商用利用をご希望の方は、別途ご連絡ください。

🔗 [ライセンス詳細はこちら](https://creativecommons.org/licenses/by-nc-sa/4.0/)


## 📚 設計ノート・今後の展望

詳細な構想背景や思想的展開については `docs/design_notes.md` に記載。
