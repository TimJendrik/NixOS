# NixOS Configuration

Dies ist meine persönliche NixOS-Konfiguration.  
Ziel ist es, ein sauberes, versioniertes Setup für den Einsatz in VMs und auf meinem Hauptsystem zu haben.

---

## 🔹 Inhalt

- **configuration.nix** – Hauptkonfiguration von NixOS
- **hardware-configuration.nix** – Hardware-spezifische Einstellungen
- Optional installierte Pakete & Services:
  - Plasma 5 Desktop mit SDDM
  - Neofetch für Systeminfo
  - QEMU Guest Agent & SPICE Clipboard Agent (bidirektional, Host ↔ VM)
  - Grundlegende Tools und Utilities nach Bedarf

---

## 🔹 Installation / Verwendung

1. **NixOS installieren** (aktuelle Version)
2. `/etc/nixos/configuration.nix` und `/etc/nixos/hardware-configuration.nix` überschreiben oder anpassen
3. System neu bauen und aktivieren:

```bash
sudo nixos-rebuild switch
