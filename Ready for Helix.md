#### Enable Windows-Subsystems for Linux (WSL)

[run PowerShell as admin][ms]
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

Install Ubuntu via Microsoft Store

[ms]: https://docs.microsoft.com/de-de/windows/wsl/install-win10

Install [Brackets][b] on Windows
[b]: http://brackets.io/ 

set alias for editing WSL files in Brackets outside of WSL
```bash
echo "alias b='/mnt/c/Program\ Files\ \(x86\)/Brackets/Brackets.exe'" >>.bashrc
```

Add the [Brackets Markdown Preview extension][mdpe] to Brackets
[mdpe]: https://bitbucket.org/begue/brackets-markdown-preview/

```bash
cd git/some-content
b Linux\ on\ Windows.md
```

Write something in [Markdown][md]
[md]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

render [this page][hp] using Helix Pages
[hp]: https://some-content-aeroid.project-helix.page/