# NixOS Configuration

This is my personal NixOS configuration.  
The goal is to have a clean, versioned setup for both VMs and my main system.

---
![Neofetch on NixOS](/images/Neofetch.png)

---
## 🔹 Contents

- **configuration.nix** – main NixOS configuration
- **hardware-configuration.nix** – hardware-specific settings
- Optional installed packages & services:
  - Plasma 5 Desktop with SDDM
  - Neofetch for system info
  - QEMU Guest Agent & SPICE Clipboard Agent (bidirectional, Host ↔ VM)
  - Basic tools and utilities as needed

---

## 🔹 Installation / Usage

1. Install **NixOS** (latest version)
2. Replace or adjust `/etc/nixos/configuration.nix` and `/etc/nixos/hardware-configuration.nix`
3. Rebuild and activate system:

```bash
sudo nixos-rebuild switch
