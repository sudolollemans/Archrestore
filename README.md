A system restoration script for Arch Linux that reinstalls packages, restores configuration backups, and re-enables system services.

---

# Features

- Installs base and user packages from saved lists
- Restores `/etc` and `/home` from backup
- Reapplies systemd service states
- Supports both official and AUR package restoration

---

# Expected Backup Files


~/pkglist.txt
~/aurlist.txt
~/services_state.txt
/mnt/backup/etc/
/mnt/backup/home/


---

# Usage

sudo ./restore.sh

What it restores
Pacman packages
AUR packages (via helper)
System configuration (/etc)
User data (/home)
systemd service states

Warning
This script can overwrite system configuration and user data.
Only use on a prepared or recovery system.


---

