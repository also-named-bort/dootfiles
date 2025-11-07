# dotfiles for omarchy
## additional packages
### walker->install->services
[tailscale](https://github.com/tailscale/tailscale)\
[bitwarden](https://github.com/bitwarden/clients)
Chromium Account
### walker->install->terminal
[kitty](https://github.com/kovidgoyal/kitty)
### packages
[kmonad (see below)](https://github.com/kmonad/kmonad?tab=readme-ov-file)\
```shell
sudo groupadd --system uinput
```
```shell
sudo usermod -aG input john
```
```shell
sudo usermod -aG uinput john
```
```shell
sudo cp ~/dootfiles/99-kmonad.rules /lib/udev/rules.d/
```
[stow](https://www.gnu.org/software/stow/)\
[firefox](https://github.com/mozilla-firefox/firefox)\
[nextcloud-client](https://github.com/nextcloud/desktop)\
[vlc](https://github.com/videolan/vlc)\
[bluetui](https://github.com/pythops/bluetui)\
[jellyfin-ffmpeg](https://github.com/jellyfin/jellyfin-ffmpeg)\
[jrnl](https://jrnl.sh/en/stable/usage/)
### AUR
[wl-kbptr](https://github.com/moverest/wl-kbptr)\
[jellyfin-media-player](https://github.com/jellyfin/jellyfin-media-player)\
[jellyfin-tui](https://github.com/dhonus/jellyfin-tui)\
[caps-log](https://github.com/NikolaDucak/caps-log)\
[yazi (see below)](https://github.com/sxyazi/yazi)
```shell
sudo pacman -S yazi ffmpeg 7zip jq poppler fd ripgrep fzf zoxide resvg imagemagick
```
[yubico-authenticator-bin (see below)](https://github.com/Yubico/yubioath-flutter)
```shell
sudo pacman -S pcsclite ccid
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
