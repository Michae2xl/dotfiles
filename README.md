# dotfiles

My terminal configuration files.

## Starship Prompt

Custom prompt with **Catppuccin Mocha** theme and Nerd Font icons.

### Preview

```
ᙇ  ~  Projects/my-app   main  +1   v20.11.0   01:34
❯
```

| Segment     | Description       |
| ----------- | ----------------- |
| `ᙇ`         | Custom macOS icon |
| `~`         | Current directory |
| ` main`     | Git branch        |
| ` v20.11.0` | Node.js version   |
| `01:34`     | Current time      |

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

### Customization

The macOS icon `ᙇ` is defined in `starship/starship.toml`:

```toml
[os.symbols]
Macos = "ᙇ "
```

You can replace it with any Nerd Font icon or emoji.
