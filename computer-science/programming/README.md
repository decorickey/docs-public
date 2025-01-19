# プログラミング

## リンク集

* [「良いコードとは何か」で消耗するのはもうやめよう](https://developersblog.dmm.com/entry/2024/11/01/110000)
* [生焼けオブジェクト](https://krkadev.blogspot.com/2010/05/half-baked-objects.html)
* [貧血ドメインモデル](https://www.martinfowler.com/bliki/AnemicDomainModel.html)

## 格言

### コードは理解しやすくなければならない

* リーダブルコード

### Early Return

* リーダブルコード

## SOLID原則

### Single Responsibility Principle

* 単一責任の原則
* 単一責任とは単一目的である
  * 変更のタイミングや理由が同じである

### Dependency Inversion Principle

* 依存関係逆転の原則
* 下位レベルが上位レベルに依存すべきである
* レベルとは入出力からの距離である
  * レベルが高いとは入出力から遠いということである
  * レベルが高いとは抽象度が高いということである

## ノウハウ

### Closure

* 定義時のスコープにある外部変数（引数以外）をキャプチャして保持し続ける関数
* Closureごとに独立している
