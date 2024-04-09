# はじめに

これは､自分がlinuxを触る際に使うコマンドやプログラムである｡
必須や便利だと思ったコマンドを､備忘録として残しておく｡

OSはdebian系を使っている｡シェルはbash｡



# コマンド一覧

## ◎ ufw

ファイヤーウォールの設定を簡単に出来るようにするコマンド

### インストール

```
sudo apt install ufw
```

### 使い方

```
ファイヤーウォールを無効化
$ sudo ufw disable

デフォルトを拒否に設定
$ sudo ufw default deny

LANないからのみ､SSHを受ける
$ sudo ufw allow proto tcp from 192.168.10.0/24 to any port 22

8080の通信を許可(v4+v6)
$ sudo ufw allow 8080

80の通信を許可(v4+v6)
$ sudo ufw allow 80

ファイヤーウォールを有効化
$ sudo ufw enable
```

## ◎ Midnight Commander (mc)

CUIでGUI(エクスプローラーなど)のように､ファイル観覧・編集が出来るソフト
マウス操作も使えるため､操作が簡単｡使用感は､windowsのエクスプローラーに似ている｡

### インストール

```
sudo apt install mc
```

### 使い方

```
mc
```

上記のコマンドを実行すると､コマンド実行時のディレクトリを開く｡

## tmux

ターミナル内で､画面分割をするコマンド

### インストール

```
sudo apt install tmux
```

## zx

圧縮ファイルを解凍するコマンド

## ◎python

プログラミング言語､pythonの本体

### インストール

```
sudo apt install python3
```

```
sudo apt install pip
```

## glances

linuxサーバーのリソース管理アプリケーション

### インストール

```
pip install glances
```



