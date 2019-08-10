## XSRF プロテクション
- Angular の interceptor がデフォルトで Cookie に保存されている XSRF-TOKEN を読み取り、変更リクエスト(POST, DELETE)の request header に X-XSRF-TOKEN という名前で付与する
    - そのため、GET リクエストなどでサーバー側が XSRF-TOKEN を Cookie に保存する必要がある
