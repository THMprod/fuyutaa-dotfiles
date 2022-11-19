# fuyutaa's dotfiles!

These are used in this video on my channel, fuyutaa - hacking et cybersec.
![rice preview](./PREVIEW-DEMONDICE-RICE-2.png)

## Description

These are the dotfiles for my DEMONDICE Arch Linux rice!
There are hotkeys, Window animations and more!
I tried to keep the configuration simple: for example, I did not used EWW (Elkowar's Wacky Widgets) but Polybar(one package, easier to configure...).

In the README.md, I present you the project, but if you want a full tutorial, look in the full-guide.md!

## If you like my dotfiles !

Feel free to give me a star on this repo 🙂!

### Dependencies

This rice uses the following packages/wm/etc... :

| Package             | Role                    |
| --------------------|-------------------------|
| bspwm               | Window manager          |
| sxhkd               | Hotkeys daemon          |
| lightdm             | GUI: Desktop and login  |
| lightdm-gtk-greeter | lightdm tool            |
| st                  | Suckless terminal       |
| picom               | Compositor (fork)       |
| bash                | The shell               |
| feh                 | Background handler      |
| dunst               | Custom notifications    |
| bat                 | Improved cat            |
| exa                 | Improved ls             |
| rofi                | App Launcher            |
| starship            | Custom icons for files  |
| polybar             | The B A R               |
| neovim              | Text editor             |
| git                 | Github repo cloner      |

> These packages may need other depedencies that will be installed udring the package installation.
> You will also need yay to install some of the stuff.

### Installing
* Install all the depedencies with pacman
```shell
sudo pacman -S bspwm sxhkd lightdm lightdm-gtk-greeter picom feh dunst bat exa rofi starship polybar neovim git
```
#### ATTENTION ⚠️: st is not downloadable with pacman. It will come with included in this repository's files.

* Make the .config folder and subfolders
```shell
mkdir .config
mkdir .config/bspwm
mkdir .config/sxhkd
mkdir .config/polybar
```

* Clone the repository

* Execute the following commands to set-up dotfiles:
```shell
cp -r ./config/* ~/.config
cp -r ./home/bashrc ~/.bashrc
cp -r ./home/Xresources ~/.Xresources
cp -r ./bin/* ~/.local/bin
```

* Compile my version of st:
```shell
cd ~/.config/st
./rebuild.sh
```

Done! Easy right?

## Shortcuts (sxhkd)

| Shortcut                 | What it does                |
| -------------------------| ----------------------------|
| super + w                | Close window                |
| super + shift + return   | Open rofi (app launcher)    |
| super + return           | Open st terminal            |
| super + b                | Open firefox                |
| super + tab              | Switch monocle/tiled mode   |
| super + t                | Switch to tiled mode        |
| super + f                | Switch to fullscreen mode   |
| super + space            | Switch to floating mode     |
| super + ctrl + {h,j,k,l} | Move a floating window      |
| super + alt + {h,j,k,l}  | Resize active window        |
| super + escape           | Reload sxhkd config file    |


## Version History

* 1.0
    * First version. Polybar needs to be improved.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Credits
For this project, I mixed dotfiles from different people, customized, re-edited, removed scripts and added mine.
As for the original dotfiles, thanks to:
* [AlphaTechnolog, sxhkd and other](https://github.com/AlphaTechnolog/dotfiles)
* [Ruturajn, starship.toml](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* DEMONDICE for the wallpaper. I improved the quality and upscaled the image with AI to make it fit.