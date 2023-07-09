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

```
# C:\Users\Admin\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1

# color UI
# add `Meslo LGM NF Font`, in VSCode Setting -> go to File -> Preferences -> Settings, in Windows Terminal: Settings -> ... -> font face: `Meslo LGM NF Font`
# search for @feature:terminal font -> fill: Meslo LGM NF
oh-my-posh init pwsh --config 'C:\Users\QT-PC\AppData\Local\Programs\oh-my-posh\themes\powerlevel10k_rainbow.omp.json' | Invoke-Expression

# Terminal-Icons Github: Icon
Import-Module Terminal-Icons

# PSReadLine Github: Suggestion
Import-Module PSReadLine
Set-PSReadLineOption -EditMode Windows
Set-PSReadLineOption -PredictionViewStyle ListView
Set-PSReadLineOption -PredictionSource History
```
