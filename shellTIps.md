# ShellのTips

## bash

### bash_profileとbashrcの違い

#### bash_profile

ログイン時にのみ実行に実行される。用途としては環境変数を設定する (exportする変数)

環境変数はプロセス間で勝手に受け継がれる。

#### bashrc

対話モードの bash を起動する時に毎回実行される

- 環境変数でない変数を設定する (exportしない変数)
- エイリアスを定義する
- シェル関数を定義する
- コマンドライン補完の設定をする

bash を起動する度に毎回設定する必要

### ログイン起動、対話起動

- ログイン起動  
CUIモードやsshでログインしたとき
- 対話起動  
GUIからターミナルを開いたときや、bashをコマンドで直接実行したとき

```
# ログイン時
Last login: Sat Apr 18 21:42:52 on ttys001
bash_profile読み込まれたよ
bashrc読み込まれたよ

# bashをコマンドで直接実行
$ bash
bashrc読み込まれたよ
```
### 参考URL

- [本当に正しい .bashrc と .bash_profile の使ひ分け](https://qiita.com/magicant/items/d3bb7ea1192e63fba850)
- [bash起動時の設定ファイル実行順序](https://qiita.com/tatesuke/items/88629e9550b813109964)