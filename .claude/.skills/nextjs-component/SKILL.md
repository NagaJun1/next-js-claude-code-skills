---
name: nextjs-component
description: Next.js の App Router 向けコンポーネントを生成する。
  Server/Client Component の使い分け、Tailwind CSS、TypeScript を考慮。
---

## ルール
- TypeScript を使用する
- Tailwind CSS を使用する
- デフォルトは 'use client' で React の hook が使用できる実装とする
- 入力のバリデーションは zod を使用する

- tanstack
  - useQueryの`queryKey`は、依存先のデータソースが同じ場合、同じキーを含める必要がある
    - キーのバリエーションとして、`user`, `users`の様な複数形の名前のキーは使わず、この場合はいずれも`user`を`queryKey`に含める実装にする
  - useQueryの`queryKey`は、各クエリ毎で一意である必要がある
    - 例：特定のユーザーを取得する ... `queryKey: ["user", id]`
    - 例：ユーザー一覧を取得する ... `queryKey: ["user", "list"]`
