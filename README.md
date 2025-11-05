# dotfiles
## additional packages
### * requires AUR
### ** from walker->install->services
tailscale**\
bitwarden**\
stow\
[kmonad](https://github.com/kmonad/kmonad?tab=readme-ov-file)\
firefox\
nextcloud-client\
vlc\
[bluetui](https://github.com/pythops/bluetui)\
jellyfin-ffmpeg\
[wl-kbptr*](https://github.com/moverest/wl-kbptr)\
yubico-authenticator-bin*\
jellyfin-media-player*\
jellyfin-tui*\
[yazi](https://github.com/sxyazi/yazi)

```shell
sudo pacman -S yazi ffmpeg 7zip jq poppler fd ripgrep fzf zoxide resvg imagemagick
```


## App specific setup
 
### kmonad permissions
 
```shell
sudo groupadd --system uinput
```
 
```shell
sudo usermod -aG input username
```
 
```shell
sudo usermod -aG uinput username
```
 
```shell
sudo cp ~/dootfiles/99-kmonad.rules /lib/udev/rules.d/
```

 
### yubico-authenticator setup
 
```shell
sudo pacman -S pcsclite
```
 
```shell
sudo pacman -S ccid
```
 
```shell
sudo systemctl enable pcscd.service
```
 
```shell
sudo systemctl start pcscd.service
```
 
 
## Omarchy post install
 
[clean up script](https://github.com/maxart/omarchy-cleaner/)
```shell
curl -fsSL https://raw.githubusercontent.com/maxart/omarchy-cleaner/main/omarchy-cleaner.sh | bash
```

## Themes
```shell
https://github.com/JJDizz1L/aetheria.git
```
```shell
https://github.com/vale-c/omarchy-arc-brueberry.git
```
```shell
https://github.com/davidguttman/archwave.git
```
```shell
https://github.com/bjarneo/omarchy-aura-theme.git
```
```shell
https://github.com/catlee/omarchy-dracula-theme.git
```
```shell
https://github.com/bjarneo/omarchy-monokai-theme.git
```
```shell
https://github.com/sc0ttman/omarchy-one-dark-pro-theme.git
```
```shell
https://github.com/bjarneo/omarchy-pulsar-theme.git
```
```shell
https://github.com/omacom-io/omarchy-synthwave84-theme.git
```
```shell
https://github.com/monoooki/omarchy-torrentz-hydra-theme.git
```
```shell
https://github.com/leonardobetti/omarchy-tycho.git
```
