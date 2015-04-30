# visualstudiocode-usersetting


## 設定方法(Windows)

コマンドプロンプトを管理者権限で実行し、下記コマンドでUserディレクトリにシンボリックリンクを貼る

```
cd "C:\Users\ユーザ名\AppData\Roaming\Code" 
cmd /c mklink /D User "C:\Users\ユーザ名\Documents\git\visualstudiocode-usersetting\User" 
```
