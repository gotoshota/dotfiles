# dotfiles

基本的な構成は以下の通り。
- zsh : Shell
- neovim : テキストエディタ
- rofi : ランチャー

## zsh
プラグインマネージャにsheldonを採用。rust製のため、`cargo`が実行可能がどうかをチェック。

### sheldon のインストール
まずはrustをインストールする。
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
cargoを使ってsheldonをインストールする。
```bash
mkdir -p ~/.cargo/bin
cargo install sheldon
```

## neovim
プラグインマネージャにlazy.nvimを採用。
また、init.luaは分割して管理。

## rofi
ランチャー。少しだけカスタマイズしている。
