# Tour of Ruby

###### Rubyでつくる静的＆動的Webサイト勉強会(仮)

#### MATSUBARA Nobutada

---

# Ruby

+++

## プログラミング言語 Ruby

* 作者: Matz
* 1994年生まれ(発表は1995年)
    * Javaが1995年
* 純粋オブジェクト指向言語
* 動的型付け言語
* 国産言語で初めて国際規格になった言語(2012)
* [インタビュー](http://web-engineer.buyuden.net/interview/matz/)

+++

## History

参考 : [Ruby(Programming Language) - wikipedia](https://en.wikipedia.org/wiki/Ruby_programming_language)

* 1993/02 : Ruby 作り始める
* 1994/10 : 内輪に公開
* 1995/12 : Ruby 0.95 (first public release)
* 1996/12 : Ruby 1.0
* 1998/12 : Ruby 1.2
* 1999/08 : Ruby 1.4
    * ピッケル本発売
* 2000/09 : Ruby 1.6

+++

## History

* 2003/08 : Ruby 1.8
    * Ruby on Rail 登場 (2005)
* 2007/12 : Ruby 1.9
    * 1.8とは部分的にしか互換性が無い
    * YARV登場！
* 2013/02 : Ruby 2.0
* 2013/12 : Ruby 2.1
* 2014/12 : Ruby 2.2
* 2015/12 : Ruby 2.3
* 2016/12 : Ruby 2.4

+++

## History

2020年に Ruby3 を予定しているが...

---

# 設計思想

+++

### 言語は十人十色

### 目的があって作られる

+++

### Ruby は
### 「たのしくプログラミングする」ため

+++

## そのため
### 書き方はたくさんある

* `{ ... }` と `begin ... end`
* `if` と `unless`
* `Array#length` と `Array#size`

---

## ココからは半分趣味

---

## 純粋オブジェクト指向

+++

##### オブジェクト指向プログラミングとは

プログラムをオブジェクト間のメッセージパッシングでモデル化する手法

+++

#### C言語と何が違うか

* 機能的には値(フィールド)と操作(メソッド)がセットになっている
  * C言語では関数(手続き)に値を与える
  * Rubyではオブジェクトのメソッドを呼ぶ

+++

#### Rubyでのデータは全てがオブジェクト

* 組み込み型は無い
* クラスもモジュールもオブジェクト
* トップレベルもオブジェクト
* メソッドやブロックはオブジェクトじゃないがオブジェクト化できる

データはどんなオブジェクトかと考える
(としっくりくると思うけど)

---

## 動的型付け言語

+++

## 型はある

+++

## しかし、実行時に決まる

* もちろん実行する前に確定してるものもある
* しかし処理系は決めつけない(最適化の関係でしてる可能性はあるかも)

+++

#### 対して
## 静的型付け言語

* 実行する前に型は決まってる
    * というか決めないといけない
    * ので分からないところを明示する必要がある
* 決まってるため検査ができる(静的型検査)
    * **いくつかのバグ** を未然に防げる
* 型の明示や検査を煩わしいと思う人も居る

どっちが好きかというのは趣味の問題

+++

##### ただし
#### 世の中的には(なんらかの)型検査を導入する傾向

* Pythonは型ヒントを導入
* MSは静的型付きJSとしてTypeScriptを開発
* Elixirも型検査の導入を表明した

Rubyも3系で型検査を導入するとは言ってる...

---

# More Ruby !
#### ｵﾇﾇﾒの書籍など

+++

##### 注意

とある趣向に偏ってる！

+++

#### Rubyの古典的な中身を知る

[Rubyソースコード完全解説](http://amzn.asia/eAPla6c)

![](https://images-na.ssl-images-amazon.com/images/I/51MQAYG70TL.jpg)

+++

#### Rubyの古典的な中身を知る

[Rubyソースコード完全解説](http://amzn.asia/eAPla6c)

[Web版もある](http://i.loveruby.net/ja/rhg/book/)

+++

#### Rubyの中身(YARV)

[Rubyのしくみ -Ruby Under a Microscope-](http://amzn.asia/hgKzjPp)

![](https://images-na.ssl-images-amazon.com/images/I/71KrmcyShVL.jpg)

+++

#### Rubyの黒魔術集(嘘)

[メタプログラミングRuby](http://amzn.asia/amF1FgK)

![](https://images-na.ssl-images-amazon.com/images/I/81eBueseIcL.jpg)

+++

#### その他

* [アンダースタンディング コンピュテーション](https://www.oreilly.co.jp/books/9784873116976/)
    * 計算理論の話なので情報系の方々はどうぞ(実装はRuby)
* [リファクタリング:Rubyエディション](http://amzn.asia/gjoEeXE)
    * Rubyじゃない方(Javaだったかな)はすごい名著と聞くのできっとこれも
* [あなたの知らない超絶技巧プログラミングの世界](https://gihyo.jp/book/2015/978-4-7741-7643-7)
    * 最高に面白いよ
* [RubyでつくるRuby ゼロから学びなおすプログラミング言語入門](https://www.lambdanote.com/collections/frontpage/products/ruby-ruby)
    * とても丁寧で初級者向け
    * [Web版もあります](http://ascii.jp/elem/000/001/230/1230449/)

---

### まとめ

* RubyはJavaと同じ頃に日本で生まれた
    * そのせいか日本人コミッタが多い
* 楽しくプログラミングするための言語
* データは全てオブジェクト
* 実行時まで型を決めつけない
    * ~~型検査が欲しくなったらHaskellにおいでよ~~

---

# おしまい
