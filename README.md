# dotfiles
## additional packages
 
stow
firefox\
bitwarden\
yubico-authenticator\
tailscale\
vlc\
[impala](https://github.com/pythops/impala)\
[bluetui](https://github.com/pythops/bluetui)\
jellyfin-media-player\
jellyfin-ffmpeg\
[wl-kbptr](https://github.com/moverest/wl-kbptr)\
[kmonad](https://github.com/kmonad/kmonad?tab=readme-ov-file)
 
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
sudo touch /lib/udev/rules.d/99-kmonad.rules
```
 
```shell
sudo echo "KERNEL=="uinput", MODE="0660", GROUP="uinput", OPTIONS+="static_node=uinput"">>/lib/udev/rules.d/99-kmonad.rules
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
