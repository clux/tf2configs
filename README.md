# tf2 configs
Personal binds, scripts, and settings that do not replicate over steam's cloud sync. This is for linux.

# Installation
Fetch TF2 from Steam, then clone and link from tf2 directory:

```bash
# copy or link into:
~/.steam/steam/SteamApps/common/Team\ Fortress\ 2/tf/cfg/

```

Then set steam launch options:

```
-novid -toconsole -nojoy +mat_forcehardwaresync 0
```