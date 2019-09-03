## プロセスの特定
- `lsof` コマンドを使って特定する
    - `-i` オプションでポートを指定できる
    - `-t` オプションで PID を特定できる
- 4200 ポートで動いているプロセスの PID を調べる
    ```
    $ lsof -t -i:4200
    ```