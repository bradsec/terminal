# terminal
MacOS and Linux Terminal related files and dotfiles

## MacOS Usage
> kdark.terminal colour scheme combined with the kdark.zshrc for a zsh prompt and appearance in MacOS terminal similar to Kali linux.  

![kdark.terminal](/previewmacos.png)

`kdark.terminal` is a colour scheme for the default MacOS terminal application.  
- Download [kdark.terminal](https://github.com/bradsec/terminal/blob/main/kdark.terminal) and open to import. 
  - Alternatively open the terminal.app and go into the preferences and import the kdark.terminal color scheme. 
- Make the imported colour scheme the Default.  
- Download [kdark.zshrc](https://github.com/bradsec/terminal/blob/main/kdark.zshrc) and rename as `.zshrc` in the user home path `~/.zshrc`.  

#### `.zshrc` uses `zsh-syntax-highlighting`, `zsh-autosuggestions` and `Fira Code font`.

These can be installed manually or using Homebrew:

```sh
brew install zsh-syntax-highlighting
brew install zsh-autosuggestions
brew tap homebrew/cask-fonts
brew install --cask font-fira-code

source ~/.zshrc
```
## Debian Console Usage (No xDesktop)
Install zsh shell, zsh-syntax-highlighting and zsh-autosuggestions
```sh
sudo apt -y install zsh zsh-syntax-highlighting zsh-autosuggestions

chsh -s $(which zsh)
```
- Download [debian.zshrc](https://github.com/bradsec/terminal/blob/main/debian.zshrc) and rename as `.zshrc` in the user home path `~/.zshrc`.  
```sh
source ~/.zshrc
```
#### Change console font
`sudo dpkg-reconfigure console-setup` try `TerminusBold` `10x20`

![debian.console](/previewdebian.png)
