Arch Management v5

Arch Management v5 is an all-in-one **Arch Linux system maintenance and network management script**.  
It allows you to perform full system updates, cleanups, health checks, network monitoring, VPN management, and more—all from a single interactive menu.  

This script also automatically checks for required packages and installs missing dependencies from both official repositories and the AUR (via `paru`).

---

## Features

### System Maintenance
- Full system update (official repos + AUR + Flatpak + firmware updates)
- Cleanup package cache, logs, and orphaned packages
- `.pacnew` files management (`pacdiff`)
- Optional snapshots via Btrfs or Timeshift
- Kernel and service health checks
- Optional weekly auto-maintenance via systemd timer

### Network & Internet Management
- View network status and devices
- List and connect to Wi-Fi networks
- Ping test and public IP display
- Speedtest support (`speedtest-cli`)
- VPN management (OpenVPN / WireGuard)
- Firewall status monitoring (UFW)
- Remote hosts placeholder for future SSH/monitoring features

### Health Dashboard
- CPU and RAM ASCII usage graphs
- Disk usage display
- Network device status
- Failed services overview
- SMART disk health checks

### Auto-Installation of Dependencies
- Installs missing packages from official repos
- Installs AUR-only packages using `paru`
- Warns if AUR helper is missing
- Fully modular—add more packages easily

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/arch-management.git
cd arch-management
```
Copy the script to your local bin:
cp arch-management ~/.local/bin/
chmod +x ~/.local/bin/arch-management
Run the script:
~/.local/bin/arch-management
Optional Setup

To enable weekly auto-maintenance:

Select option 4 in the main menu
The script sets up a systemd user timer to automatically run updates, cleanup, and health checks weekly.
Requirements
Arch Linux or Arch-based distributions
bash 5+
sudo privileges
Internet connection for updates
Optional: paru (for automatic AUR package installation)
Screenshots

(Optional: Add screenshots of menus, dashboard, and network menu here.)

Contributing

Contributions are welcome! Feel free to open issues, suggest features, or submit pull requests.

License

This project is released under the MIT License.

Author

Created by MarkoCeko – Arch Linux enthusiast and automation fan.
