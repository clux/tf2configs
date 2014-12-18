# tf2 configs
Personal binds, scripts, and settings that do not replicate over steam's cloud sync. This is for linux.

## Installation
First create a shortcut under `~/tf` to your tf directory with all the juicy stuff in it:

```bash
cd ~
ln -s ~/.steam/steam/SteamApps/common/Team\ Fortress\ 2/tf/
```

Clone repo, make bash shortcuts available:

```bash
cd tf2configs
echo ". `pwd`/tf2rc" >> ~/.bashrc
```

Then set steam launch options:

```
-novid -toconsole -nojoy +mat_forcehardwaresync 0
```

## Updating
Edit the configs that are wrong then:

```bash
./sync.sh
```

To overwrite configs from repo to `~/tf/cfg`
