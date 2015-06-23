Eric's XMonad config.

To use in Ubuntu:

1. Install XMonad and related packages: `sudo apt-get install xmonad libghc-xmonad-contrib-dev xcompmgr hsetroot`.
1. Make sure you can compile the `xmonad.hs` config: `xmonad --recompile`.
1. Log out then back in, choosing Gnome 2.x as your desktop environment.
1. Start XMonad with `xmonad --replace`.
  1. If you have graphics jittering issues, replace Compiz with Xcompmgr: `xcompmgr -n`.
  1. Set the wallpaper with: `hsetroot -center $PATH_TO_IMAGE`.
