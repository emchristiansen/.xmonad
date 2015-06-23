Eric's XMonad config.

To use in Ubuntu:

1. Clone this repo to your home folder: `git clone https://github.com/emchristiansen/.xmonad.git ~/.xmonad`.
1. Install XMonad and related packages: `sudo apt-get install xmonad libghc-xmonad-contrib-dev xcompmgr hsetroot`.
1. Make sure you can compile the `xmonad.hs` config: `xmonad --recompile`.
1. Log out then back in, choosing Gnome 2.x as your desktop environment.
1. Start XMonad with `xmonad --replace`.
  1. If you have graphics jittering issues, replace Compiz with Xcompmgr: `xcompmgr -n`.
  1. Set the wallpaper with: `hsetroot -center $PATH_TO_IMAGE`.

This will create workspaces labeled [0 .. 9] and [q, w, e, r, a, s, d, f, z, x, v].

Basic commands:

1. Move view to workspace: `<Super>-$WORKSPACE`, e.g. `<Super>-1`.
1. Move window to workspace: `<Super>-<Shift>-$WORKSPACE`, e.g. `<Super>-<Shift>-1`.
1. New terminal: `<Super>-<Shift>-<Enter>`.
1. Close window: `<Super>-<Shift>-c`.

All of this is configurable via the `xmonad.hs` file.
In fact, XMonad is just a library, so by changing `xmonad.hs` you are actually writing your own window manager.
You can do pretty much anything you want.
