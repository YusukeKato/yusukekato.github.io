# How to use tmux
- tmuxの使い方メモ
- Document: [github.com/tmux/tmux/wiki](https://github.com/tmux/tmux/wiki)

## Install
```sh
sudo apt install tmux
```

## How to use
- 端末を開いてtmuxコマンドを実行
- プレフィックスキーを押して一度離してから各キーを押して操作
- デフォルトのプレフィックスキーは「Ctrl+b」

## Keybinds
- Ctrl+b -> ?: キーバインド一覧を表示
- Ctrl+b -> ": 上下に分割
- Ctrl+b -> %: 左右に分割
- Ctrl+b -> 矢印キー: ペイン移動

## ~/.tmux.conf
```sh
vim ~/.tmux.conf
```

マウスクリックでペイン切り替え
```
set-option -g mouse on
```

[参考](https://www.tohoho-web.com/ex/tmux.html)

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
