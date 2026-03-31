# dotfiles

Meus arquivos de configuracao do terminal.

## Starship Prompt

Prompt customizado com tema **Catppuccin Mocha** e icones Nerd Font.

### Requisitos

- [Starship](https://starship.rs/)
- Uma [Nerd Font](https://www.nerdfonts.com/) (ex: JetBrains Mono Nerd Font)

### Instalacao

```bash
# Instalar Starship
curl -sS https://starship.rs/install.sh | sh

# Instalar Nerd Font (macOS)
brew install --cask font-jetbrains-mono-nerd-font

# Copiar config
cp starship/starship.toml ~/.config/starship.toml

# Adicionar no ~/.zshrc
echo 'eval "$(starship init zsh)"' >> ~/.zshrc

# Reiniciar terminal
source ~/.zshrc
```
