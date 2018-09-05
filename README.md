# visualstudiocode-usersetting

[Visual Studio Code](https://code.visualstudio.com/) の設定ファイル

## 設定方法

Userディレクトリにシンボリックリンクを貼る

### Windowsの例

Windows PowerShellを管理者権限で実行し下記コマンドを実行
※`\Documents\git\`にcloneされている場合。

```PowerShell
> cd "C:\Users\$(Get-Content env:username)\AppData\Roaming\Code"
> rm .\User\
> cmd /c mklink /D User "C:\Users\$(Get-Content env:username)\Documents\git\visualstudiocode-usersetting\User"
```

またはコマンドプロンプトを管理者権限で実行し下記コマンドを実行

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

## 参考
テキスト用の設定と推奨される拡張機能は[VSCode workspace setting for text writing](https://gist.github.com/s2terminal/12b376c844a4f72f89ab94df83a75ea5#file-settings-json)に記載
