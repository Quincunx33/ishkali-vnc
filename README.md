<p align="center">
  <img src="images/banner.png" alt="Tasfia's Hacker Lab" width="100%">
</p>

# Tasfia's Hacker Lab 🐉

> **কালি-স্টাইল আলপাইন লিনাক্স — iPhone/iPad-এ VNC সহ রেডি-টু-রান**
> *Kali-style Alpine Linux on iPhone/iPad — pre-built rootfs with VNC, zero install steps.*

<div align="center">

| ⚙️ বেস | 📦 প্যাকেজ | 🖥️ কমান্ড | 🔓 missing deps |
|---|---|---|---|
| Alpine 3.14 x86 (musl) | 225+ APK | 925+ executable | **0** |

[![iOS](https://img.shields.io/badge/iOS-iSH%20App-black?logo=apple&logoColor=white)](https://ish.app)
[![VNC](https://img.shields.io/badge/VNC-RFB%20003.008-green)]()
[![Size](https://img.shields.io/badge/tar.gz-746%20MB-blue)]()

</div>

---

## ✨ কেন এটা স্পেশাল?

iSH অ্যাপে সাধারণত `apk install` খুব ধীর (এমুলেশনের কারণে)। এই প্রজেক্টে **সবকিছু আগে থেকে build করা** — আপনি শুধু tar.gz extract করবেন, বাকি সব রেডি। VNC server-ও pre-installed, এক কমান্ডে iPad-এ পুরো ডেস্কটপ!

<p align="center">
  <img src="images/terminal_demo.png" alt="Terminal with Tasfia banner" width="70%">
</p>

## 🚀 ৫ মিনিটে সেটআপ (Setup)

| ধাপ | কাজ |
|---|---|
| 1️⃣ | iSH-এ **Settings → Filesystems** যান |
| 2️⃣ | আগের rootfs **Delete** করুন |
| 3️⃣ | **Import** → `kali-vnc-prebuilt-ish.tar.gz` সিলেক্ট করুন |
| 4️⃣ | Mount point = `/` রাখুন |
| 5️⃣ | টার্মিনালে লিখুন: `startvnc xvfb` |
| 6️⃣ | bVNC অ্যাপে **Host = 127.0.0.1**, **Port = 5900** (আলাদা ফিল্ডে) |

> 💡 **মনে রাখবেন:** iSH অ্যাপ foreground-এ রাখুন (background-এ করলে VNC ঘুমায়ে যায়)। বন্ধ করতে: `startvnc stop`
> ⚠️ ফোনে ~4 GB খালি জায়গা রাখুন (extract = ~2.6 GB)

<p align="center">
  <img src="images/vnc_demo.png" alt="VNC desktop on iPad" width="70%">
</p>

## 🛠️ কী কী Tool আছে? (925+ commands)

<p align="center">
  <img src="images/tools_collage.png" alt="Tools grid" width="90%">
</p>

বিস্তারিত লিস্ট দেখুন: [`TOOLS-v7.md`](TOOLS-v7.md)

| ক্যাটাগরি | নমুনা Tool |
|---|---|
| 🕵️ পেনটেস্ট | `nmap` • `masscan` • `sqlmap` • `nikto` • `zmap` • `tshark` • `tcpdump` • `radare2` • `strace` • `ltrace` • `dnsrecon` • `macchanger` • `proxychains` • `tor` • `sshpass` |
| 💻 ডেভ | `gcc` • `g++` • `node`/`npm` • `python3`/`pip3` • `ruby` • `perl` • `lua5.3` • `tcl`/`expect` • `make` • `cmake` • `meson` • `gdb` • `valgrind` • `git` |
| ✏️ এডিটর | `vim` • `neovim` • `nano` • `micro` • `emacs` • `joe` • `vis` • `mg` • `bvi` • `hexedit` |
| 🐚 শেল | `bash` (+completion) • `zsh` • `fish` • `tcsh` • `dash` |
| 📊 মনিটর | `htop` • `atop` • `sysstat` • `iftop` • `nethogs` • `ncdu` • `tmux` |
| 🎵 মিডিয়া | `ffmpeg` • `mpv` • `sox` • `lame` • `flac` • `cmus` • `mpd` • `imagemagick` |
| 🌐 নেটওয়ার্ক | `curl` • `wget` • `lynx` • `w3m` • `links` • `smbclient` • `sshfs` • `openvpn` • `wireguard` • `rdesktop` • `aria2` • `lftp` |
| 🖥️ X11/VNC | `Xvfb` • `xterm` • `x11vnc` • `twm` • `openbox` • `xeyes` • `xclock` • `cmatrix` |

## 🐍 Python Packages (pre-installed)

`scapy` • `impacket` • `pyftpdlib` • `pysocks` • `psutil` • `requests` • `flask` • `tornado` • `pytest` • `pyyaml` • `beautifulsoup4` • `paramiko` • `cryptography` + `pip3`

## 🎨 Tasfia's Banner

লগইন করলেই রঙিন বক্স দেখায়:

```
  ╔═══════════════════════════════════════════╗
  ║  ★  Tasfia's Hacker Lab ★                  ║
  ║  Kali-style • VNC ready                   ║
  ╚═══════════════════════════════════════════╝
```

রঙ/নাম বদলাতে চাইলে `/root/.tasfia_banner` এডিট করুন। ASCII art বানাতে `figlet -f slant "নাম"` ব্যবহার করুন (376 fonts available)।

## 🔧 স্টার্টআপ মোড

| মোড | কমান্ড | কাজ |
|---|---|---|
| Raw framebuffer | `startvnc` | সরাসরি x11vnc rawfb — সবচেয়ে দ্রুত, কোনো X server ছাড়া |
| Full X server | `startvnc xvfb` | Xvfb + xterm + x11vnc — ডেস্কটপ এক্সপেরিয়েন্স |
| বন্ধ | `startvnc stop` | সব প্রসেস বন্ধ |

## ⚠️ জানা সীমাবদ্ধতা (Known Limits)

- iSH = x86 user-mode emulator — GPU নেই, JIT নেই — কিছু জিনিস ধীর হতে পারে
- `java` / `metasploit` / `Burp Suite` / Debian-ভিত্তিক OS iSH-এ **অসম্ভব**
- কার্নেল access নেই — `john`, `hydra`, `ffuf`, `gobuster` আলপাইন 3.14 রিপোতে নেই
- VNC password দিয়ে রাখাভালো হয় public network-এ (`startvnc xvfb --pass YOURPASS`)

## 📦 File Structure

```
kali-vnc-prebuilt-ish.tar.gz     # প্রি-বিল্ট rootfs (extract + run)
TOOLS-v7.md                      # সম্পূর্ণ টুল তালিকা
README.md                        # এই ফাইল
images/                          # ব্যানার ও ডেমো ছবি
```

---

<div align="center">

**Made for Tasfia** 💚 — *Explore. Exploit. Elevate.*

</div>
