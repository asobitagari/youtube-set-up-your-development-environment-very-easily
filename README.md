# 開発環境最短構築

## 手順
### Scoopのインストール
PowerShellを開き、下記のコマンドを実行する。
```PowerShell
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
```
もし、ポリシー等で起こられるようであれば、下記のコマンドを実行し、再び上記のコマンドを実行する。
```PowerShell
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```

### ScoopのBacketの追加
PowerShellを開き、下記のコマンドを実行する。
```PowerShell
scoop bucket add extras
```

### パッケージのインストール
PowerShellを開き、下記のコマンドを実行する。
```PowerShell
 scoop install git anaconda3 php php-xdebug go rustup dart vscode
 ```