# GRUB theme (by kurami32)
This is a grub theme that I customized to my liking, all mostly from [this theme](https://github.com/Hitori-Laura/OsageChan_GRUB_theme) (thanks xd), if someone view this, I hope you like it! :D
![screenshot](./background.png)

If you want to have it you'll need to follow these steps first (I'm assuming that you have you OS functioning, so...)

### First clone the repository
```
git clone https://github.com/Kurami32/Kurami_GRUB_theme.git
```
### Then copy the repository to this directory
```
sudo cp -r Kurami_GRUB_theme /usr/share/grub/themes
```
### After this modify the grub config file
You can use you editor favorite, I'll use nvim.
```
sudo nvim /etc/default/grub
```
### Then search for this line
The line that says 'GRUB_THEME' should be there, uncomment it the route of the theme that we copied.
```
GRUB_THEME="/usr/share/grub/themes/Kurami_GRUB_theme/theme.txt"
```
### Lastly update grub
```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

