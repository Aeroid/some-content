# Ready for Helix on Windows

#### Summary

set up a Windows with WSL/git/Brackets to manage content for Helix

### Enable Windows-Subsystems for Linux (WSL)

[run PowerShell as admin][ms]
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

Install Ubuntu via Microsoft Store

[ms]: https://docs.microsoft.com/de-de/windows/wsl/install-win10

enable CTRL-SHIFT-C/V via WSL console properties

### Get Brackets to work from within WSL

Install [Brackets][b] on Windows
[b]: http://brackets.io/ 

set alias for editing WSL files in Brackets outside of WSL
```bash
echo "alias b='/mnt/c/Program\ Files\ \(x86\)/Brackets/Brackets.exe'" >>.bashrc
```

Add the [Brackets Markdown Preview extension][mdpe] to Brackets
[mdpe]: https://bitbucket.org/begue/brackets-markdown-preview/

### Install git in Ubuntu

```bash
sudo apt-get install git
```


### Edit some Markdown

```bash
cd git/some-content
b Ready\ for\ Helix.md
```

Write something in [Markdown][md]
[md]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet


### Publish

```bash
git add Ready\ for\ Helix.md
git commit -m "I'm ready"
git push
```
### Enjoy

render [this page][this] using Helix Pages
[this]: https://some-content-aeroid.project-helix.page/Ready%20for%20Helix.html