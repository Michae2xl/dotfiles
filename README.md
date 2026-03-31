# dotfiles

My terminal configuration files.

## Starship Prompt

Custom prompt with **Catppuccin Mocha** theme and Nerd Font icons.

### Requirements

- [Starship](https://starship.rs/)
- A [Nerd Font](https://www.nerdfonts.com/) (e.g. JetBrains Mono Nerd Font)

### Setup

```bash
# Install Starship
curl -sS https://starship.rs/install.sh | sh

# Install a Nerd Font (macOS)
brew install --cask font-jetbrains-mono-nerd-font

# Copy config
cp starship/starship.toml ~/.config/starship.toml

# Add to ~/.zshrc
echo 'eval "$(starship init zsh)"' >> ~/.zshrc

# Restart terminal
source ~/.zshrc
```
