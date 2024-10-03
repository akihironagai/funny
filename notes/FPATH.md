# FPATH

`zsh` で `brew` と `nix` について **補完 (completion)** させる:

```bash
FPATH="$(brew --prefix)/share/zsh/site-functions:$FPATH"
FPATH="$HOME/.nix-profile/share/zsh/site-functions:$FPATH"
```
