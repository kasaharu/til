## Storybook TypeScript configuration
- デフォルトだと Angular アプリケーションのトップの `tsconfig.json` しか見ないので Multiple projects の場合、個別の `tsconfig.app.json` で設定を上書きしていると設定が足りなくなったりする
- [Storybook TypeScript configuration](https://storybook.js.org/docs/guides/guide-angular/#step-4-storybook-typescript-configuration) にあるように `.storybook/tsconfig.json` で Storybook 用の上書きファイルを用意できるので不整合がある場合はここで頑張る。
