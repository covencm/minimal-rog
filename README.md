## How to use this theme 

+ For debian based distros

```bash

#  copy the selected theme to plymouth/themes
sudo cp -r minimal-rog /usr/share/plymouth/themes/

#register new theme
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/minimal-rog/rog.plymouth 100

# select minimal-rog theme
sudo update-alternatives --config default.plymouth

sudo update-initramfs -u


```

+ For arch based distros 

```bash

sudo cp -r minimal-rog /usr/share/plymouth/themes/

# check if theme exist in dir
sudo plymouth-set-default-theme -l

# now set the theme  and rebuilt the initrd
sudo plymouth-set-default-theme -R minimal-rog

```

![rog](./rog_logo.png)
