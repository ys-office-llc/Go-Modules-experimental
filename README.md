# Go 遊び場
## Go Modules のはじめかた

### クイックスタート

1. 適当な箇所に Go Modules のルートとなるディレクトリを作成し、移動する
   1. `mkdir go-example && cd $_`
2. Go Modules 初期化処理を行う
   1. 外部公開しない場合は「1.」で作成したディレクトリ名などで良い
      1. `go mod init go-example`
   2. 外部公開する場合は github.com/{username} を含んだパスにする
      1. `go mod init github.com/{your-github-username}/go-example`
3. ルートディレクトリへ `main.go` ファイルを作成し、外部モジュールを利用するコードを書く（本リポジトリの `main.go` はそうなっている）
4. 外部モジュールを読み込む
   1. `go mod tidy`

## 参考資料
* [Go Modulesを利用してローカル環境でGo言語を実行する手順](https://nishinatoshiharu.com/go-modules-overview/)
