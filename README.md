# dotfiles
## additional packages
### * requires AUR
stow\
firefox\
bitwarden\
yubico-authenticator-bin*\
pcsclite*\
nextcloud-client\
tailscale\
vlc\
[impala](https://github.com/pythops/impala)\
[bluetui](https://github.com/pythops/bluetui)\
jellyfin-media-player*\
jellyfin-tui*
jellyfin-ffmpeg\
[wl-kbptr*](https://github.com/moverest/wl-kbptr)\
[kmonad](https://github.com/kmonad/kmonad?tab=readme-ov-file)
[caligula](https://github.com/ifd3f/caligula)\
 
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
sudo cp ~/99-kmonad.rules /lib/udev/rules.d/
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
