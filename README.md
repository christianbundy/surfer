# Surfer

Simple keyboard based web browser. No tabs.

Based on Webkit2GTK and GTK3. Inspired by Lariza, Epiphany, and Surf.

No xlibs dependency -- works on Wayland, Weston, and Sway.

## Adblock

1. Install https://github.com/jun7/wyebadblock

2. `sudo ln -s /usr/lib/wyebrowser/adblock.so  /usr/lib/surfer`

Otherwise, you can use an `/etc/hosts` block list from sites like:

- https://someonewhocares.org
- (to be continued, add yours here)

## Compile and install:

```
sudo make install
```

On Arch Linux you can install with `yaourt surfer`, or manually with:

```
git clone https://github.com/christianbundy/surfer.git
cd surfer
makepkg -si
```

## Hotkeys:

`Ctrl + click` link -- open link in new window

`Ctrl + n` -- new window

`Ctrl +  s` -- go back

`Ctrl +  d` -- go forward

`Ctrl + q` -- quit

`Esc` -- stop loading

`Ctrl + h` -- home (bookmarks list)

`Ctrl + b` -- bookmark site (to remove just edit file with links: .fav in your home dir)

`Ctrl + l` -- toogle location (URL) bar

`Ctrl + /` -- find word

`Ctrl + r` -- reload page

`Ctrl + =` -- zoom in

`Ctrl + -` -- zoom out

`Ctrl + j` -- scroll down

`Ctrl + k` -- scroll up

`Ctrl + Shift + u` -- page up

`Ctrl + Shift + d` -- page down

`Ctrl + i` -- web inspector (page source)

`Ctrl + Shift + s` -- toogle user style black theme 
(/usr/share/surfer/black.css)

`Ctrl + Shift + r` -- show history (.hist file in HOME dir), to 
enable history 
change HISTORY_ENABLE to 1 in surfer.c

`F11` -- toogle fullscreen

**Edit `surfer.c` to change hotkeys**
