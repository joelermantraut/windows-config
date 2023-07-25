# windows-config
A guide to config Windows system like I use it.

Steps
1. Install [Tabby Terminal](https://tabby.sh/).
2. Open Tabby. Go to last option (Config File). Select "Show Config File". 
3. Copy - paste config.yaml file in Tabby directory.
4. Install [Git](https://gitforwindows.org/).
5. Install [PowerToys](https://learn.microsoft.com/en-us/windows/powertoys/). It is a set of tools provided by Windows, with great integration with system. Not forget to review its configuration to select useful tools for you.
6. You can install any password manager. I prefer to use the simpler one, I use [pass-winmenu](https://github.com/geluk/pass-winmenu).
7. Copy - paste "pass-winmenu.yaml" in pass-winmenu root folder.
8. Install [GPG](https://www.phildev.net/pgp/gpginstall#windows).
9. Copy or download your own password directory. Then follow pass-winmenu [setup instructions](https://github.com/geluk/pass-winmenu#creating-a-new-password-store).
10. I use a 60% keyboard, so I need to change my keyboard layout. To that, I use [Microsoft Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134). Then config it, it is really simple to use.
11. Install Node.JS from [this link](https://nodejs.org/en/download).
12. Install [NeoVIM](https://neovim.io/).
13. Config NeoVIM. For that, first copy you neovim config in "C:\Users\User\AppData\Local\nvim". After that, run this command in Windows Powershell:
```
$uri = 'https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
(New-Object Net.WebClient).DownloadFile(
  $uri,
  $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath(
    "~\AppData\Local\nvim\autoload\plug.vim"
  )
)
```
14. Open NeoVIM running `nvim` command, press ':' and run `PlugInstall` to install all needed plugins.
15. Download and config [ContextMenuManager](https://github.com/BluePointLilac/ContextMenuManager) to delete any unwanted option added to you Windows Context Menu.
16. Don't forget to user personal accounts in software like Google Chrome and Visual Studio Code to automatically sync preferences.

Other useful tools:

- [XtremeDownloadManager](https://xtremedownloadmanager.com/)
- [Google Chrome](https://www.google.com/intl/es-419/chrome/)
- [Visual Studio Code](https://code.visualstudio.com/)
