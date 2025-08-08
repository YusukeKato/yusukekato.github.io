# swap

## show

```sh
$ swapon --show
NAME      TYPE SIZE USED PRIO
/swap.img file   4G   0B   -2
/swapfile file  16G   0B   -3
```

## how to

```sh
# スワップファイル作成
sudo fallocate -l 16G /swapfile
# sudo chmod 600 /swapfile
# スワップ領域の作成
sudo mkswap /swapfile
# スワップの有効化
sudo swapon /swapfile
# OS起動時に自動的にマウントする設定
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```

## set swappiness
- 0〜100（デフォルトは60）
- 0: なるべくスワップを使用しない
- 100: 積極的にスワップを使用する

```sh
# 確認
cat /proc/sys/vm/swappiness
# 設定
sudo sysctl vm.swappiness=30
# 自動的に設定
echo 'vm.swappiness=30' | sudo tee -a /etc/sysctl.conf
```

## test

```sh
sudo apt install stress-ng
stress-ng --vm 1 --vm-bytes 95% --timeout 60s
```

## remove

```sh
sudo swapoff /swapfile
sudo rm /swapfile
```

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
