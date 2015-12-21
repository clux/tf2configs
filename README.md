# tf2 configs
Personal binds, scripts, and settings that do not replicate over steam's cloud sync. This is for linux.

## Installation
First create a shortcut under `~/tf` to your tf directory with all the juicy stuff in it:

```bash
ln -sf .steam/steam/steamapps/common/Team\ Fortress\ 2/tf/ $HOME/tf
```

Clone repo, make bash shortcuts available:

```bash
echo "source $PWD/tf2rc" >> ~/.bash_profile
```

Then set steam launch options:

```
-novid -toconsole -nojoy +mat_forcehardwaresync 0
```

## Installing configs
Two ways (from repo pwd):

```bash
# force overwrite
cp cfgs/*.cfg ~/tf/cfg/

# symlink in place (changes version controlled)
find "$PWD" -name "*.cfg" -type f -print -exec ln -sfn {} ~/tf/cfg/ \;
```
