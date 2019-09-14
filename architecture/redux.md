## Ducks
- [Redux Reducer Bundles](https://github.com/erikras/ducks-modular-redux)
- Action, Action Creator, Reducer を一つのファイルで管理する
  - 複数の機能をまたいで actions/ とか reducers/ みたいな役割でディレクトリを分けるのは理にかなっていないのはわかる
  - 大抵の場合は action を更新すると reducer にも何かしらの変更が入る → つまり密結合になっている
  - 密結合になっているなら同じファイルにあったほうが修正時のコストが抑えられる
- ルールとしては下記
  - reducer を `export default` にする
