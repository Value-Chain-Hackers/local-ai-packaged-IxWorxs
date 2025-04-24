
# 🖥️ AI Sandbox Server Environment Report

**Hostname:** `AISandbox`  
**Public IP:** `95.99.112.224`  
**Date:** `Thu Apr 24 2025`

---

## 🧰 OS & Kernel

| Key           | Value                               |
|---------------|-------------------------------------|
| Distro        | Debian GNU/Linux 12 (bookworm)      |
| Kernel        | 6.8.12-8-pve                         |
| Boot Mode     | systemd-boot (ZFS root, Proxmox VM) |

---

## 💾 Filesystem & Boot

- Root on: `ZFS` (`rpool/ROOT/pve-1`)
- Boot mode: `EFI`, kernel command line includes:  
  `boot=zfs quiet intel_iommu=on video=efifb:off`
- Filesystem: `zfs`
- Proxmox kernel: `6.8.12-8-pve`

---

## 🔌 Network Configuration

| Interface | Address         | Notes             |
|-----------|------------------|-------------------|
| `eth0`    | `192.168.129.10` | Private LAN       |
| `docker0` | `172.17.0.1`     | Docker internal   |
| `Public`  | `95.99.112.224`  | External IP (you provided) |

Default route: via `192.168.129.1` on `eth0`

---

## 🐳 Docker Environment

- **Docker version**: 28.0.4
- **Docker Compose**: v2.34.0
- **Docker Runtimes**: `runc`, `nvidia`, `io.containerd.runc.v2`
- **Storage Driver**: overlay2 on ZFS
- **Cgroup Version**: v2
- **GPU Runtime**: `nvidia` installed

---

## 🎮 GPU Hardware

| Device | Model                       | Bus       |
|--------|-----------------------------|-----------|
| GPU 0  | NVIDIA RTX 3060 (12GB VRAM) | 81:00.0   |

### `nvidia-smi`:
- **Driver**: 570.133.07
- **CUDA**: 12.8
- GPU in use: ✅ (330MiB used)

---

## 🧠 Python & Dev Tools

| Tool   | Version    |
|--------|------------|
| Python | 3.11.2     |
| pip    | 23.0.1     |
| git    | Installed  |
| jq     | Installed  |
| curl   | Installed  |
| nano   | Installed  |
| docker | Installed  |
| wget   | Installed  |

---

## 🔐 SSH & Access

- SSH Port: **22**
- Root login: **enabled**
- Password auth: **enabled**
- Users with shell access: `root`
- Sudo access group: `sudo`

---

## 🌀 System Services

| Service              | Status   |
|----------------------|----------|
| `docker`             | active ✅ |
| `ssh`                | active ✅ |
| `cron`               | active ✅ |
| `containerd`         | active ✅ |
| `systemd-networkd`   | active ✅ |
| `postfix`            | active ✅ |
| `polkit`             | active ✅ |

---

Let me know if you want to save this to a file like `AISandbox_Report.md`, or move on to file transfer or deployment steps.