# virtualBoxのTips

## インストール(Mac)

- [インストーラをダウンロード](https://www.virtualbox.org/wiki/Downloads)
- インストーラからインストール
  - [【macOS 10.15 Catalina】Oracle VM VirtualBox がインストールできない対応](https://www.yokoweb.net/2020/01/19/macos-catalina-virtualbox-install-error/)
- virtulBoxに新規追加
  - [VirtualBoxにUbuntu16.04をインストール
](https://qiita.com/ykawakami/items/4bae371932110b2e25e3)
  - [Ubuntu 18.04.4 LTS (Bionic Beaver)](http://releases.ubuntu.com/bionic/)
  - [VirtualBoxをリサイズさせる設定の仕方](https://www.gekkoseisaku.com/blog/web-design/2716/)

## VirtualBoxにssh接続

色々苦戦しましたが、下記手順どおりやったらうまく行った

- [VirtualBox上ゲストOSにssh接続する＆ゲストOSからインターネット接続できるようにする。](https://qiita.com/Yoshiki-Takahashi/items/7274dff15dbafee5b118)
  - [VirtualBox上のUbuntuにSSHで接続するための設定](http://smys0515.hatenablog.com/entry/2016/02/29/080000)  
  SSHサーバのインストールをした
- host側から接続  
  `ssh nsuzuki@192.168.151.100`

## その他設定

- [UbuntuでMacのUSキーボードに対応させる[VirtualBox]](https://noumenon-th.net/programming/2018/11/10/ubuntu-us/)

## 用語集

- スタンドアローン  
機器やソフトウェア、システムなどが、外部に接続あるいは依存せずに単独で機能している状態のこと
- ネットワークアダプタ
コンピュータなどの機器を通信ネットワーク（LAN）に接続するための装置

## 参考URL

- [Virtual Boxのネットワーク設定](http://3ka2w.blog.fc2.com/blog-entry-42.html)