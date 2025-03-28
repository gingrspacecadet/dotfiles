Hello!
======
These are my dotfiles for hyprland.<br>
I started with Typecraft's [dotfiles](https://github.com/typecraft-dev/dotfiles) and expanded on them.

Dependencies
===========
* `Hyprland` (this should be obvious)<br>
* `Hyprpaper`<br>
* `Hyprlock`<br>
* `Hypridle`<br>
* `Kitty`<br>
* `Starship`<br>
* `Waybar`<br>
* `Wofi`<br>
* `Pipewire`<br>
* `Pipewire-pulse`<br>
* `Pavucontrol`<br>
* `Font Awesome`<br>
* `Jetbrains Mono`<br>
* `Meslo Nerd Font`

How to install
==============
This section assumes you are on a basic install of [Arch Linux](https://archlinux.org/) with hyprland. If you don't have hyprland, follow the [wiki](https://wiki.hyprland.org/Getting-Started/Installation/)

Yay
===
To install the dependencies, you will require yay.<br>
<br>It is a package manager for the [Arch User Repository](https://aur.archlinux.org)<br>
<br>From the beginning:
<br>Login as root **or** run `su` as a non-priviledged user (if you have set up `sudo`, add it to the beginning of the next command).<br>
<br>Run `pacman -S git base-devel` and follow the instructions.<br>
<br>Then, run `git clone https://aur.archlinux.org/yay.git` to clone the repository.<br>
<br>`cd yay` then `makepkg -si` to install yay.<br>
<br>`cd ..` and `rm -rf yay` to delete the folder.<br>
<br>And now you have yay!

Now for the fun bit
===================
Install the dependencies with<br>
<br>`yay -S hypridle hyprlock hyprpaper kitty starship waybar wofi pipewire pipewire-pulse pavucontrol ttf-meslo-nerd-font-powerlevel10k ttf-jetbrains-mono-git ttf-font-awesome`<br>
<br>Install `stow` with `yay -S stow`<br>
<br>Change directory to where you want the dotfiles to be saved (in my case, `~`)<br>
<br>Run `git clone https://github.com/gingrspacecadet/dotfiles.git` to clone the repo.<br>
<br>`cd dotfiles` to enter the new directory.<br>
<br>Now run `for dir in */; do [ -d "$dir" ] && stow "$dir"; done` to copy my config!<br>
(alternatively you can run `stow *dir name*` to only copy specific configs, where `dir name*` is the name of the config you want to copy).








