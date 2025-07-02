# personal-dev-journal

日々の開発活動や学習内容を記録できる個人用日記アプリケーションです。Remix + TypeScript で構築した SPA で、GitHub 認証によるユーザー管理、GitHub リポジトリでのデータ保存、GitHub Pages でのホスティングを実現しています。完全に GitHub エコシステム内で完結するシンプルな設計により、面倒な設定は不要。個人の成長を振り返ったり、過去の活動を思い出すのに便利な開発ログツールです。

## Development

Run the dev server:

```sh
npm run dev
```

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying Node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `npm run build`

- `build/server`
- `build/client`

## Styling

This template comes with [Tailwind CSS](https://tailwindcss.com/) already configured for a simple default starting experience. You can use whatever css framework you prefer. See the [Vite docs on css](https://vitejs.dev/guide/features.html#css) for more information.
