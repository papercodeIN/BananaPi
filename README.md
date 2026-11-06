<img align="right" src="https://visitor-badge.laobi.icu/badge?page_id=papercodeIN.BananaPi" height="20" />

<h1 align="center">🌟 Banana Pi 🌟</h1>

<p align="center">
  <em>Banana Pi setup guides, scripts and OS resources for BPI-M4 Berry/Zero, P2 Pro, CM5 Pro and Forge1 — companion to our YouTube playlists</em>
</p>

<p align="center">
  <a href="https://www.youtube.com/@Fusion_Automate"><img src="https://img.shields.io/badge/YouTube-FusionAutomate-%23FF0000?style=for-the-badge&logo=youtube" alt="YouTube"></a>
  <a href="https://www.instagram.com/fusion_automate"><img src="https://img.shields.io/badge/Instagram-fusion__automate-%23E4405F?style=for-the-badge&logo=instagram" alt="Instagram"></a>
  <a href="https://x.com/fusion_automate"><img src="https://img.shields.io/badge/X-fusion__automate-000000?style=for-the-badge&logo=x" alt="X (Twitter)"></a>
  <a href="https://t.me/fusionautomate"><img src="https://img.shields.io/badge/Telegram-%40fusionautomate-%2326A5E4?style=for-the-badge&logo=telegram" alt="Telegram"></a>
  <a href="https://fusionautomate.in/"><img src="https://img.shields.io/badge/Website-fusionautomate.in-blueviolet?style=for-the-badge" alt="Website"></a>
</p>

---

## **Banana Pi SBC YouTube Playlist**

- 📺 **[Banana Pi BPI-P2 Pro](https://www.youtube.com/playlist?list=PLxrSjjYyzaaJf7wXYRMxTi6N13cYAuab-)**  
- 📺 **[Banana Pi BPI-M4 Berry](https://www.youtube.com/playlist?list=PLxrSjjYyzaaJXDh-iKOQY-EMEp0uqdyD2)**  
- 📺 **[Banana Pi BPI-M4 Zero](https://www.youtube.com/playlist?list=PLxrSjjYyzaaJ4cOlBL80YnnAXfSN2oSzT)**  
- 📺 **[Banana Pi Forge1](https://www.youtube.com/playlist?list=PLxrSjjYyzaaI9y954_VXcspIvGXz4ONaa)**  
- 📺 **[Banana Pi CM5 Pro](https://www.youtube.com/playlist?list=PLxrSjjYyzaaIJwhcOY5QQZcM9CcAJ7ojp)**  
---


## **Default Login Credentials**
Below are the default login credentials based on your Banana Pi model:

| **Login Option** | **Username** | **Password** |
|-----------------|-------------|-------------|
| Option 1        | `pi`        | `bananapi`  |
| Option 2        | `root`      | `bananapi`  |
| Option 3 (P2-Pro) | `linaro`  | `linaro`    |

---

## **Connecting to Wi-Fi**
To connect your Banana Pi to a Wi-Fi network:

1. **List Available Wi-Fi Networks:**
   ```bash
   nmcli dev wifi list
   ```

2. **Connect to a Wi-Fi Network:**
   ```bash
   sudo nmcli --ask dev wifi connect <network-ssid>
   ```
   **Example:**  
   ```bash
   nmcli --ask dev wifi connect Capgemini_4G
   ```

---

## **Clear SSH Host Entries (Windows)**
If you encounter SSH fingerprint errors, clear the known hosts file:

```cmd
echo. > %userprofile%\.ssh\known_hosts
```

---

## **Armbian Setup**
To set up Armbian on Banana Pi:

```bash
sudo armbian-install
```

---

## **Disk Operations & Formatting**
### **1. List Available Storage Devices**
```bash
lsblk
```

### **2. Wipe the Entire Storage Device**
```bash
sudo dd if=/dev/zero of=/dev/mmcblk0 bs=4M status=progress
```

> **Note:** This will erase all data on the device. Ensure you've selected the correct block device.

### **3. Partition and Format Storage**
1. **Create New Partitions:**
   ```bash
   sudo fdisk /dev/mmcblk0
   ```
2. **Format Partition as ext4:**
   ```bash
   sudo mkfs.ext4 /dev/mmcblk0p1
   ```

---

## **Node-RED Installation**

```bash
# Download the Installation Script
wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/Scripts/Node_RED_Installation.sh
# Make the Script Executable
chmod +x Node_RED_Installation.sh   
# Run the Installation Script
./Node_RED_Installation.sh
```

---

---

## 📞 Contact

| 📞 Method | 🔗 Details |
|-----------|-----------|
| Call / WhatsApp | [+91-9974477759](https://wa.me/919974477759) |
| Telegram | [@fusionautomate](https://t.me/fusionautomate) |
| Email | [eng.innovativ@gmail.com](mailto:eng.innovativ@gmail.com) |

## 💖 Support My Work

<p align="center">
  <a href="https://buymeacoffee.com/pylin" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" style="height: 50px; width: 180px;">
  </a>
</p>

<p align="center">
  ⭐ Star this repo if it helped you · 🔔 <a href="https://github.com/papercodeIN">Follow Fusion Automate</a>
</p>
