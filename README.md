# japanese-writing-gemini

[GitHub](https://github.com/MetamoL/japanese-writing-gemini)

人が通読するまとまった日本語文章をGeminiへ委任するための、汎用エージェント向けスキルです。小説、README、技術文書、記事、ブログ、紹介文などを広く対象にします。

## すること

- 対象となる文章作業でGeminiへの委任を提案する
- 元の会話やリポジトリが見えなくても執筆できる、自己完結した依頼文を作る
- 正本から必要な事実、変更不可事項、創作可能範囲、文体、納品形式を一つにまとめる
- 小説では必須展開の列挙だけで終えず、場面がドラマとして閉じる条件と、意味のある肉付けを行える範囲を依頼へ含める

短い文言、コードコメント、誤字修正、AI向け内部文書、作業報告は対象外です。Geminiへの送信、完成本文の反映・公開、受領稿の採否判断も行いません。

## 使い方

自動発火に対応する環境では、小説やREADMEなどの新規執筆・大幅改稿で候補になります。明示的に使う場合は次のように指定します。

```text
$japanese-writing-gemini この小説本文をGeminiへ依頼するブリーフを作ってください。
```

正本は [SKILL.md](SKILL.md) です。`agents/openai.yaml` はCodex向けメタデータです。本リポジトリはGemini APIやMCPへの通信機能を含みません。

## ライセンス

[LICENSE](LICENSE) に定めるsource-available条件で提供します。
