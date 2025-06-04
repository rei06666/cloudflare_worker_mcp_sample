# cloudflare_worker_mcp_sample
## 環境構築
```
npm install
```

## ローカルでの実行
```
npm run dev
```

## 動作確認
```
npx @modelcontextprotocol/inspector
```

- http://127.0.0.1:6274をブラウザで開く
- TransportTypeを「Streamable HTTP」、URLに http://localhost:8787/mcp 入力し、connect

## Cloudflareへのデプロイ
```
npm deploy
```
- ブラウザが表示されるためログインする  
- デプロイが成功すると「https://<サブドメイン>.workers.dev」の形式でURLが表示される
- 表示されたURLの/mcpパスで、動作確認を行う
