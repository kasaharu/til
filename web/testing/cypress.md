## Cypress
- E2E テスティングフレームワーク

## Cypress Dashboard
- CI で実行したテストを記録できる
- `$ cypress open` をして開いたウィンドウから設定できる

## CI で実行
- CI などで実行する場合は `$ cypress run` を使うが対象のサーバーが起動している必要がある
   - CircleCI の場合は `background: true` で dev-server を起動し wait-on を使って起動を待ちつつテストを実行するとよい
