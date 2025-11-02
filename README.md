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
jellyfin-tui*
 
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
