# Customize ZSH on MacOS

- Install ohmyzsh 
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
code ~/.zshrc
ZSH_THEME="avit"
```

- Install autosuggestions plugin
```
cd ~/.oh-my-zsh/custom/plugins
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
code ~/.zshrc
plugins=(
  zsh-autosuggestions
  git
)
```

- Install Brew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
code ~/.zshrc
# Brew
export PATH="/opt/homebrew/bin:$PATH"
```

- Install FNM
```
brew install fnm
code ~/.zshrc
# Fnm
eval "$(fnm env --use-on-cd)"
```

- Install Fig
```
brew install fig
fig login
fig doctor
```
