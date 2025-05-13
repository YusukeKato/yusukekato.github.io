# How to use Git
- gitコマンドの使い方のメモ書き
- GitHubのSSHの設定方法

## SSH
```sh
cd ~/.ssh
ssh-keygen -t rsa # ex: RSA
# Register id_rsa.pub on GitHub
```

[Qiita - GitHubでssh接続する手順](https://qiita.com/shizuma/items/2b2f873a0034839e47ce)

## Config
```sh
git config --global user.name "name"
git config --global user.email "email"
```

## Update commit message
```sh
# コミット
git commit -m "old message"
# コミットメッセージを更新
git commit --amend -m "new message"
```

[Qiita - Git commit メッセージの変更方法](https://qiita.com/kenose0328/items/185f7e8634d816c85a84)

## Tag
```sh
# add
git tag 1.0.0
# delete
git tag -d 1.0.0
# push to remote
git push --tags origin
```

[Qiita - Git tagの更新](https://qiita.com/kuroneco/items/61cd14ed475519d20748)

## 変更を戻す
```sh
git clean -fd
git checkout -- .
```

[Qiita - Gitでの変更を戻す方法](https://qiita.com/ys-office-llc/items/2a65193fd19894d8e4df)

## 特定のファイルを特定のコミットまで戻す
```sh
git restore --source=<commit-id> -- <file-name>
```

[Zenn - Gitで特定のファイルを過去のコミットに戻す方法](https://zenn.dev/ktrszk/articles/7bac6384b108d6)

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
