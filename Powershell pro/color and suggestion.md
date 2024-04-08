## Các công cụ chính:
- Làm đẹp: oh-my-posh (yêu cầu tải và cài thêm font), Terminal-Icons
- Suggestion: PSReadLine

## Setting for Windows Terminal and VS Code

Link:
- [oh-my-pod Official](https://ohmyposh.dev/docs/installation/windows)
- [Install oh-my-posh for vscode](https://dev.to/badgamerbad/oh-my-posh-on-all-windows-terminals-vs-code-integrated-terminal-too-3jg8#:~:text=open%20the%20terminal%20and%20run%20the%20following%20command,pwsh%20--config%20~%2F.1_shell.omp.json%20%7C%20Invoke-Expression%20restart%20the%20terminal)
- [Terminal-Icons](https://github.com/devblackops/Terminal-Icons)
- [PSReadLine](https://github.com/PowerShell/PSReadLine)

- Tác giả recommend dùng font [Meslo LGM NF](https://github.com/kalaschnik/meslolgs-nf-template)
- Một số dev dùng icon khác có chứa icon của Nerd Font như [Hack Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/Hack.zip)

## Step 1: Cài đặt modules
- Tổng hợp CMD:
```
winget install JanDeDobbeleer.OhMyPosh -s winget
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/amro.omp.json" | Invoke-Expression
oh-my-posh font install

Install-Module PowerShellGet -Force
Install-Module PSReadLine -Force
Install-Module Terminal-Icons -Repository PSGallery -Force
```

## Step 2: Tạo file PROFILE thông qua VSCode:
- `code $PROFILE`
- Copy code sau đây rồi lưu lại

```
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/amro.omp.json" | Invoke-Expression
Import-Module Terminal-Icons
Import-Module PSReadLine
Set-PSReadLineOption -EditMode Windows
Set-PSReadLineOption -PredictionViewStyle ListView
Set-PSReadLineOption -PredictionSource History
```
