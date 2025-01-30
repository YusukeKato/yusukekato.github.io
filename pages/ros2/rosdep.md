# rosdep
- rosdepのメモ書き
- [公式ドキュメントのコマンドリファレンス](https://docs.ros.org/en/independent/api/rosdep/html/commands.html)

# インストール

```sh
sudo apt install python3-rosdep
sudo rosdep init
rosdep update
```

# 使用方法
- `package.xml`に記載されている依存関係のパッケージのインストールする

```sh
cd ~/ros2_ws/src
rosdep install -r -y -i --from-paths .
```

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
