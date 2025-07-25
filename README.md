# dotFiles


### Required packages
Assuming Hyprland is already installed, or you did an archinstall with the Hyprland config (which is what i did).

`sudo pacman -S kitty pipewire spotify-launcher waybar dunst starship zsh hyprlock hyprpaper discord bluez-utils fastfetch pavucontrol inetutils lazygit fzf fd rofi neovim git unzip less curl hyprpolkitagent --needed`

there's a possibility that there are some redundant things (like the hyprpolkitagent) but I haven't used this rice enough to know. Please post an issue and I'll take a look and remove/add packages from the readme.



install yay for rofi-bluetooth-git

`sudo pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si`
```
```

`yay -S rofi-bluetooth-git`

> [!IMPORTANT]
wallpapers must be stored in `~/Documents/wallpapers/`
configure the name of your wallpaper in `~/.config/hypr/hyprpaper.conf`

**The rest is optional**

`sudo pacman -S spotify-launcher discord` 

`yay -S termius visual-studio-code-bin`

(termius is an ssh client i use) (free for students)


#### TIPS:
If you're trying to debug the waybar,
do 
`killall waybar`
`waybar & disown`

this will output messages in that terminal when u click a button that doesn't work, for example.

### Design choices

I'm only listing notable changes to the original configuration. It's worth looking at `~/.config/hypr/hyprland.conf` for all changes to keybindings

This configuration was heavily influenced by `i3-wm`
use `$mainmod Return` for opening up your terminal (kitty in this case)
use `$mainMod HJKL` for moving focus l d u r respectively
use `$mainMod SHIFT hjkl` for moving windows

`$mainMod d` for rofi

`$mainMod r` to start resizing.
while resizing: `HJKL` to resize left down up or right 
also: `SHIFT HJKL` to resize MORE (covers more distance when you hold shift)


`nvim` is just a lazyvim config because I'm too lazy to configure my own dev env


