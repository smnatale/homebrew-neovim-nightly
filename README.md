# Neovim nightly

A Homebrew tap for installing Neovim nightly on Apple Silicon and Intel Macs.

## Install

If you have the stable `neovim` formula installed, unlink it first so the nightly cask can provide `nvim`:

```sh
brew unlink neovim
```

Update Homebrew, then install from this fork:

```sh
brew update
brew tap smnatale/neovim-nightly
brew install --cask smnatale/neovim-nightly/neovim-nightly
```

Launch Neovim with `nvim`.

## Update

```sh
brew update
brew upgrade --cask --greedy smnatale/neovim-nightly/neovim-nightly
```

This cask uses `version :latest`. The [`--greedy` option](https://docs.brew.sh/Manpage#upgrade-options-installed_formulainstalled_cask-) includes these casks when checking for upgrades.

To force a fresh installation of the nightly build:

```sh
brew reinstall --cask smnatale/neovim-nightly/neovim-nightly
```
