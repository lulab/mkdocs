# Basic Settings of MacOS

## Schedule Shutdown/Sleep/Wake

```bash
# Schedules a repeating sleep to occur each day, Monday through Sunday, at 8pm.
sudo pmset repeat sleep MTWRFSU 20:00:00

# Schedules a repeating shutdown to occur each Saturday at 7:30pm;
# and a repeating wake or power on event every Monday at 7:30am.
sudo pmset repeat shutdown S 19:30:00 
sudo pmset repeat shutdown S 19:30:00 wakeorpoweron M 7:30:00 
sudo pmset schedule shutdown "04/30/2025 19:30:00"

# Check
pmset -g sched
# Cancel schedled
sudo pmset repeat cancel

```

## File Sharing

### Turn off Volume and Home Sharing

```bash
###Turn off Volume shares (on by default)
sudo defaults write /Library/Preferences/SystemConfiguration/com.apple.smb.server VirtualAdminShares -bool NO
###Turn off User shares (on by default)
sudo defaults write /Library/Preferences/SystemConfiguration/com.apple.smb.server VirtualHomeShares -bool NO
```

## Clean Time Machine Backups

```bash
alias tmlist="tmutil listbackups -t > tm.list"
vim tm.list  -- only keep the ones we need to remove
alias tmrm="for i in `cat tm.list`; do sudo tmutil delete -d /Volumes/Silver\ -\ Time\ Machine  -t $i; done" 
```

