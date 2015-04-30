# visualstudiocode-usersetting

[Visual Studio Code](https://code.visualstudio.com/) の設定ファイル

## 設定方法

Userディレクトリにシンボリックリンクを貼る

### Windowsの例

コマンドプロンプトを管理者権限で実行し下記コマンドを実行

```
> cd "C:\Users\ユーザ名\AppData\Roaming\Code" 
> cmd /c mklink /D User "C:\Users\ユーザ名\Documents\git\visualstudiocode-usersetting\User" 
```

### Macの例

ターミナルを起動し下記コマンドを実行

```
$ cd /Users/ユーザ名/Library/Application\ Support/Code/
$ ln -s /Users/ユーザ名/git/visualstudiocode-usersetting/User ./User
```