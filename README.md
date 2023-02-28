# React + TypeScript 最小構成

## 環境構築メモ

- コンテナに乗り込みReactのプロジェクトを作成
  ```bash
  docker-compose run --rm --no-deps react /bin/bash
  npm install -g npm
  npm install -g create-react-app
  npx create-react-app . --template typescript
  ```
- ポートに8080を使いたかったので、package.jsonのscriptsにポート番号を指定
  - `"start": "PORT=8080 react-scripts start"`
- 不要なファイルを削除
- 削除したファイルを参照している箇所を修正

## 起動方法

- 起動
  - `docker-compose up`
- テスト
  - `docker-compose  run --rm --no-deps web npm run test`