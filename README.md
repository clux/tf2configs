# tf2 configs
Personal binds, scripts, and settings that do not replicate over steam's cloud sync. This is for linux.

## Installation
Create a convenience symlink, link all your configs into `cfg` directory, and add shell helpers:

```bash
ln -sf .steam/steam/steamapps/common/Team\ Fortress\ 2/tf/ $HOME/tf
find "$PWD" -name "*.cfg" -type f -print -exec ln -sfn {} ~/tf/cfg/ \;
# alternatively: cp cfgs/*.cfg ~/tf/cfg/
```

Then set steam launch options:

```conf
-novid -console -nojoy +mat_forcehardwaresync 0
```

Remember to turn of vsync + tweak timers in nvidia settings for better performance.

## Useful stuff

```bash
# last demos
find ~/tf/ -name "*.dem" -printf "%Tx %p\n" | sort -r | ccze -A | less -RX
```
