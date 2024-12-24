
# Lesgooo 
* Install i3wm with archinstall select i3 in profiles section and for audio select pipewire

* Then install these

  ```
  sudo pacman -S git nitrogen polybar kitty viewnior rofi nwg-look pavucontrol thunar tumbler btop neovim xcolor xclip dunst maim autotiling 

* Install these fonts
  ```
  sudo pacman -S ttf-cascadia-code-nerd ttf-cascadia-mono-nerd ttf-fira-code ttf-fira-mono ttf-fira-sans ttf-firacode-nerd ttf-iosevka-nerd ttf-iosevkaterm-nerd ttf-jetbrains-mono-nerd ttf-jetbrains-mono ttf-nerd-fonts-symbols ttf-nerd-fonts-symbols ttf-nerd-fonts-symbols-mono noto-fonts-cjk
  ```
* Then clone this repo
  ```
  git clone https://github.com/zistro/dotfiles.git
  ```
  * Then copy folders in the .config folder and replace all. You should cut and paste the default config folder in a backup folder before copying my config files incase you get into some trouble. Make all the .sh file executable with
     ```
     chmod +x filename.sh
     ```
  
  * Copy theme.rasi to ~/.local/share/rofi/themes/ and change the rofi theme theme from rofi themes option in the rofi menu and save the new theme with alt+a
* You're done and now reboot
# About screen tearing in i3wm 
* i3wm package does not include a compositor so you will get screen tearing. In order to fix this issue you can do two things
* One is install a picom(compositor) and and use my config
  ```
  sudo pacman -S picom
  ```
* Second one is if you have nvdia card and proprietary driver install nvidia-settings and enable force full composition pipeline in X server display configuration part
  and disable flipping in opengl setting
  ```
  sudo pacman -S nvidia-settings
  ```   
  
