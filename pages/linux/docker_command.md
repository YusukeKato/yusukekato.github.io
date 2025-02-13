# Docker command

## 確認

```sh
# イメージ一覧
docker images
# コンテナ確認
docker ps
# すべてのコンテナ確認
docker ps -a
```

## コンテナを起動

```sh
# コンテナを起動して中で作業
docker run -it イメージID
# バックグラウンドで起動
docker run -itd イメージID
```

## 起動中のコンテナに入る

```sh
docker exec -it コンテナID bash
```

## コンテナにコマンドを実行させる

```sh
docker exec -it コンテナID コマンド
```

## 削除

```sh
docker rm -f コンテナID
docker rmi イメージID
```

[参考：Qiita - Dockerコマンド よく使うやつ](https://qiita.com/Esfahan/items/52141a2ad741933d7d4c)

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
