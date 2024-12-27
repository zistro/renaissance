# Basic commands of pacman 

* sync and upgrade system > sudo pacman -Syu
* force sync > sudo pacman -Syy
* force sync and upgrade > sudo pacman -Syyu
* clear cache > pacman -Scc
  * alternatively you can use "paccache-hook" from aur to do this job auto
* my own installed package count > pacman -Qe | wc -l
* total package count > pacman -Q | wc -l
* to downgrade you will need certain package for aur "downgrade"
* default pacman config location "/etc/pacman.conf"
* add the pacman animation by adding "ILoveCandy" in pacman config
* enable parallel download to increase download speed

