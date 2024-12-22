# Go

## 公式集

### [識別子のエクスポート](https://go.dev/ref/spec#Exported_identifiers)

public/privateという表現はなく、識別子をパッケージの外にエクスポートするか否か

### [カンマOK慣用句（comma ok idiom）](https://go.dev/doc/effective_go#maps)

### [mapのイテレーションは順序不定](https://go.dev/ref/spec#For_statements)

> The iteration order over maps is not specified and is not guaranteed to be the same from one iteration to the next.

### [コメント](https://tip.golang.org/doc/comment)

エクスポートされた識別子はすべてコメントが必要である

> Every exported (capitalized) name should have a doc comment.

### [モジュールのバージョン](https://go.dev/doc/modules/version-numbers)

### [パッケージのバージョニング](https://cs.opensource.google/go/go/+/master:src/math/rand/v2/rand.go)

同一パッケージ名でバージョニング番号を付与したディレクトリ名でパッケージを新しく作る

### [internal package](https://go.dev/doc/go1.4#internalpackages)

親または兄弟のパッケージからしかインポートできない特殊なパッケージ

### [セキュリティ](https://go.dev/doc/security/)

公式が脆弱性の一覧やベストプラクティス、ツールなどを提供してくれている

### [プロジェクト構成](https://go.dev/doc/modules/layout) [(GitHub)](https://github.com/golang-standards/project-layout/blob/master/README_ja.md)

### [Table Driven Tests](https://go.dev/wiki/TableDrivenTests)

### [Testable Examples](https://go.dev/blog/examples)

ドキュメントにサンプルコードを示しつつ実行結果の確認ができる

## パッケージ集

### [embed](https://pkg.go.dev/embed)

ファイルを読み込んで利用する（バイナリに組み込む）

### [fsnotify](https://pkg.go.dev/github.com/fsnotify/fsnotify)

ファイルの変更を検知する

## リンク集

* [Google Style Guide](https://google.github.io/styleguide/go/)
* [Goのruntimeソースコードは仕様ですと言い切れるほどコメントが充実している](https://x.com/yuroyoro/status/1844317697275986225)

## コマンド

* `./...`はgoコマンド特有のものですべてのサブディレクトリとファイルを対象にする

### コマンド集

|コマンド|概要|補足|
|-|-|-|
|install|ホストマシンにパッケージをインストールする| |
|get|go.modの依存関係を更新する| |

### コンパイルが通るか試したい

`go build -o /hoge/fuga`

### `go.mod`のgoディレクティブをアップデートしたい

`go get go@patch`

`go mod tidy -go=1.x.y`
