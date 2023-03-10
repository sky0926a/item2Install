# iTerm 2 install step
## 1.install cask
```
brew Tap homebrew/cask
```
## 2. install iTerm2
```
brew instal --cask iterm2 
```
## 3. install cask font
```
brew Tap homebrew/cask-fonts
```
## 4. install font-sourcecodepro-nerd-font
```
brew install --cask font-sauce-code-pro-nerd-font
```
## 5. change text style
```
iTerm2 > Preferences > Profiles -> Text -> Font 
```
choose `SauceCodePro Nerd Font`
## 6. change color
```
iTerm2 > Preferences > Profiles -> Colors -> Color Presets
```
choose color and import style
## 7. install on-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
## 8. install powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
## 9. edit .zshrc
add into .zshrc file
```
ZSH_THEME="powerlevel10k/powerlevel10k"

POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(dir dir_writable vcs vi_mode)
POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(status time)

POWERLEVEL9K_VI_MODE_INSERT_BACKGROUND='grey30'
POWERLEVEL9K_COLOR_SCHEME='light'
POWERLEVEL9K_VCS_MODIFIED_BACKGROUND='darkgreen'
POWERLEVEL9K_DIR_ETC_BACKGROUND='032'
POWERLEVEL9K_DIR_DEFAULT_BACKGROUND='032'
POWERLEVEL9K_DIR_HOME_BACKGROUND='032'
POWERLEVEL9K_DIR_HOME_SUBFOLDER_BACKGROUND='032'
POWERLEVEL9K_PROMPT_ON_NEWLINE=true
POWERLEVEL9K_PROMPT_ADD_NEWLINE=true
POWERLEVEL9K_RPROMPT_ON_NEWLINE=true
POWERLEVEL9K_MULTILINE_FIRST_PROMPT_PREFIX=""
POWERLEVEL9K_MULTILINE_LAST_PROMPT_PREFIX="\u0024 "
```
## 10 apply style
```
source ~/.zshrc
```
