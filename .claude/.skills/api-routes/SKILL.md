---
name: api-routes
description: Next.js の Route Handlers (app/api/) を生成する。
---

## ルール
- TypeScript を使用する
- route.ts は配線のみとする
  - 認証・バリデーション・DB操作などの実処理はすべて別関数に切り出す
  - route.ts を配線専用にすることで責務が明確になり、ロジックを単独でテストできる
