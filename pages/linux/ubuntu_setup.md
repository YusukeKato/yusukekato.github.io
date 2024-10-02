# Ubuntu setup
- Ubuntuの初期セットアップ方法のメモ書き

## Install
- Google Chrome
- Visual Studio Code

```sh
sudo apt -y update
sudo apt -y upgrade
# よく使う
sudo apt -y install git
sudo apt -y install vim
sudo apt -y install tmux
sudo apt -y install curl
sudo apt -y install wget
# ssh
sudo apt -y install ssh
sudo apt -y install sshpass
# 画像関連
sudo apt -y install ffmpeg
sudo apt -y install imagemagick
sudo apt -y install gimp gimp-gmic
```

## Rename directory
```sh
LANG=C xdg-user-dirs-update --force
rm -rf デスクトップ ダウンロード テンプレート 公開 ドキュメント ミュージック ピクチャ ビデオ
sudo reboot
```
参考：https://qiita.com/peachft/items/fde3bebd356c17c1cef6

## Setup git
```sh
git config --global user.name "name"
git config --global user.email "email"
# 必要ならsshの設定なども。
```

## Others
- 日本語入力の確認
- アプリのピン留めの整理
- nvidiaドライバの確認

![](../../images/BlueTreeIcon_200x200.jpg)
