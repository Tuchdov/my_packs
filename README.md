# my_packs
My package lists to make reinstalling linux faster. <br />
To make those packs I used the following commands on manjaro: <br />
 1. flatpak list --columns name > flat_packs.txt <br />
 2. pacman -Qqem > aur_packs.txt <br />
 3. pacman -Qqen > native_packs.txt <br />


The > is a shortcut to make the output of the commands into a text file <br />
To install use this command:
sudo pacman -Sy --needed - < native_packs.txt && yaya


