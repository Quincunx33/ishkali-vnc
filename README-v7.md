# iSH Pre-Built VNC Environment — v7 ("Tasfia's Hacker Lab")

**File:** `kali-vnc-prebuilt-ish.tar.gz` (~745 MB)
**Base:** Alpine Linux 3.14 x86 (i386, musl) — official Alpine packages
**Packages:** ~420+ (all dependencies pre-resolved, zero install steps)

---

## নতুন কী আছে v7-তে? (What's new)

| ক্যাটাগরি | Tools |
|---|---|
| সিস্টেম মনিটর | `htop`, `atop`, `sysstat` (iostat/sar/mpstat), `procps` |
| নতুন এডিটর | `neovim (nvim)`, `nano`, `micro`, `joe`, `vis`, `mg`, `bvi` (binary vim) |
| নতুন শেল | `zsh`, `fish`, `tcsh`, `dash` |
| টেক্সট টুল | `jq` (JSON), `yq`, `cloc` (code counter), `tokei`, `figlet` |
| প্যাকেট/নেট | `sshpass`, `ltrace`, `tcpflow`, `zmap`, `mtr`, `bind-tools` (dig/nslookup), `openvpn`, `wireguard-tools` (wg), `sshfs`, `rdesktop` |
| অডিও/মিডিয়া | `sox`, `lame`, `flac`, `opus-tools`, `vorbis-tools`, `cmus`, `moc`, `mpd`, `alsa-utils` |
| মজা | `cmatrix` (matrix rain!), `asciinema` (record terminal), `xeyes`, `xclock`, `xcalc`, `xscreensaver` |
| ডেভ | `lua5.3`, `tcl`, `expect`, `meson`, `swig`, `doxygen`, `ccache`, `distcc`, `cppcheck`, `flawfinder`, `subversion` |
| পাইথন extra | `psutil`, `pyyaml`, `flask`, `tornado`, `pytest`, `pexpect`, `pyserial`, `requests` ইত্যাদি |
| **ব্যানার** | লগইন করলেই রঙিন "Tasfia's Hacker Lab" বক্স দেখাবে! |

সব আগের tool-ও আছে: `nmap`, `masscan`, `sqlmap`, `tshark`, `radare2`, `gcc`, `node`/`npm`, `python3`, `tmux`, `emacs`, `ffmpeg`, `lynx`, `smbclient`, `7z`, `htop`...

---

## কীভাবে ব্যবহার করবেন (How to use)

1. iSH → **Settings → Filesystems** → আগের rootfs **Delete** করুন
2. **Import** → নতুন `kali-vnc-prebuilt-ish.tar.gz` সিলেক্ট → Mount = `/`
3. Terminal-এ: `startvnc xvfb`
4. bVNC: **Host = 127.0.0.1, Port = 5900** (আলাদা ফিল্ডে), iSH foreground-এ
5. বন্ধ করতে: `startvnc stop`

> ⚠️ ফোনে ~4 GB খালি জায়গা রাখুন (extract = ~2.6 GB)

---

## Tasfia's Banner

লগইন করলেই দেখাবে:

```
  ╔═══════════════════════════════════════════╗
  ║  ★  Tasfia's Hacker Lab ★                  ║
  ║  Kali-style • VNC ready                   ║
  ╚═══════════════════════════════════════════╝
  VNC:  startvnc xvfb     Tools: tools     Update: update
```

রঙ বদলাতে চাইলে `/root/.tasfia_banner` ফাইল এডিট করুন (ANSI color code দিয়ে)।
নিজের নামে banner বানাতে: `figlet -f slant "আপনার নাম"`
