# Times tables & Notice board

値の範囲を変えられる九九表(problem1)と掲示板(problem2)のコードです
 
# DEMO
 
* problem1

![image](https://user-images.githubusercontent.com/64777602/124928603-b1c2f100-e03a-11eb-8a8e-bb41a5070980.png)

* problem2

![image](https://user-images.githubusercontent.com/64777602/124928780-e2a32600-e03a-11eb-8ff9-4e55b3dde07c.png)

 problem1では`index.html`をブラウザで開くことで上のような九九表を得られます。

# Features
 
* problem1 (Times tables)

`START`(default 1)と`GOAL`(default 9)に値(半角)を入力し`Run`をクリックことで、(GOAL-START+1)x(GOAL-START+1)の掛け算の表を作ることができます。範囲はありませんが現実的な計算量では200x200程度なら10秒ほどで出力されます。

また、`Delete table`(default 0)に値を入力すれば、その段を出力結果での表示をなくすことができます。

`Only multiples of N`(default 1)は入力値Nの倍数のみを出力できるようになり、`Except multiples of N`(default -1)では入力値Nの倍数を出力結果で空白にすることができます。

※注意

`Run`をリロードせずに二回連続で押すと表をうまく出力できません。値を変更したい場合はブラウザをリロードするか、`Reset`ボタンをクリックすることで初期化してください。

それぞれの値は複数入力することはできません。1つずづ入力してください。

`main.py`では`START`と`GOAL`以外の値で複数入力が可能です。しかし、ブラウザでは出力することはできないのでご了承ください。

* problem2 (No71c3 8o4rD 1337)

Notice board(掲示板)です。`N4M3`(NAME)に名前、`CH47`(CHAT)にコメントを入力すると投稿日時とともにComments以下に表示される。

pタグの2番目には、https://openweathermap.org/api から取得した現在の東京の天気のデータを表示し、最高1時間でデータが更新される。

pタグの3番目には、https://connpass.com/about/api/ から取得したその日のconnpassで行われるイベントを時間の早い順に5つ表示している。

# Requirement

* Python 3.9.6
* Go 1.16.5
 
# Usage

* problem1

`index.html`をブラウザで開く

* problem2

```
❯ go run main.go
server - http://localhost:8080 // サーバーURLをクリック
```
 
# Author
 
* 二宮直也
 
