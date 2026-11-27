## ルール
- 実装の指示を受けた際、事前に方針を確認する
  - 指示・指摘内容が事実に則しているか確認する
    - 事実に則していないなら修正は行わず、なぜ則していないかを出力する
  - 方針を出す前に `.agents/skills/minimal-structure/SKILL.md` の規約に従い、足すものごとに今の使い手を確かめる
  - 編集ツール（Edit/Write）を呼び出す前に、必ず方針をテキストで説明しユーザーの確認を取る
  - ドキュメントを作る際は`/docs`に出力する
  - 方針の確定後に実装を行う
  - 実装後に不要な要素が混じっていないか確認する

## コミュニケーション
- 日本語で行う

## 置き場所
- 状態・処理・判定・コメントをどの関数・コンポーネント・ファイルに置くかは `.agents/skills/responsibility-split/SKILL.md` の規約に従う。

## 分岐
- 関数・型・引数の形を決めるとき、分岐を書くときは `.agents/skills/no-unnecessary-branches/SKILL.md` の規約に従う。

## unit test
- jest の単体テストの実装は `.agents/skills/jest/SKILL.md` の規約に従う。

## backend
- backend の実装は `.agents/skills/api-routes/SKILL.md` の規約に従う。

## frontend
- frontend の実装は `.agents/skills/nextjs-component/SKILL.md` の規約に従う。
