# iSH Pre-Built VNC Environment — v7 ("Tasfia's Hacker Lab")

**File:** `kali-vnc-prebuilt-ish.tar.gz` (~745 MB)
**Base:** Alpine Linux 3.14 x86 (i386, musl) — official Alpine packages
**Packages:** ~420+ (all dependencies pre-resolved, zero install steps)

---

## What's new in v7?

| Category | Tools |
|---|---|
| System monitoring | `htop`, `atop`, `sysstat` (iostat/sar/mpstat), `procps` |
| New editors | `neovim (nvim)`, `nano`, `micro`, `joe`, `vis`, `mg`, `bvi` (binary vim) |
| New shells | `zsh`, `fish`, `tcsh`, `dash` |
| Text tools | `jq` (JSON), `yq`, `cloc` (code counter), `tokei`, `figlet` |
| Packet / network | `sshpass`, `ltrace`, `tcpflow`, `zmap`, `mtr`, `bind-tools` (dig/nslookup), `openvpn`, `wireguard-tools` (wg), `sshfs`, `rdesktop` |
| Audio / media | `sox`, `lame`, `flac`, `opus-tools`, `vorbis-tools`, `cmus`, `moc`, `mpd`, `alsa-utils` |
| Fun | `cmatrix` (matrix rain!), `asciinema` (record terminal), `xeyes`, `xclock`, `xcalc`, `xscreensaver` |
| Development | `lua5.3`, `tcl`, `expect`, `meson`, `swig`, `doxygen`, `ccache`, `distcc`, `cppcheck`, `flawfinder`, `subversion` |
| Python extras | `psutil`, `pyyaml`, `flask`, `tornado`, `pytest`, `pexpect`, `pyserial`, `requests`, and more |
| **Banner** | A colored "Tasfia's Hacker Lab" box on every login! |

All previous tools are still included: `nmap`, `masscan`, `sqlmap`, `tshark`, `radare2`, `gcc`, `node`/`npm`, `python3`, `tmux`, `emacs`, `ffmpeg`, `lynx`, `smbclient`, `7z`, `htop`, and more.

---

## How to use

1. iSH → **Settings → Filesystems** → **Delete** the old rootfs
2. **Import** → select the new `kali-vnc-prebuilt-ish.tar.gz` → Mount = `/`
3. In the terminal, run: `startvnc xvfb`
4. In bVNC: **Host = 127.0.0.1, Port = 5900** (in separate fields), keep iSH in the foreground
5. To stop: `startvnc stop`

> ⚠️ Keep ~4 GB of free space on your device (extracted size ≈ 2.6 GB)

---

## Tasfia's Banner

You will see this on every login:

```
  ╔═══════════════════════════════════════════╗
  ║  ★  Tasfia's Hacker Lab ★                  ║
  ║  Kali-style • VNC ready                   ║
  ╚═══════════════════════════════════════════╝
  VNC:  startvnc xvfb     Tools: tools     Update: update
```

To change the colors, edit `/root/.tasfia_banner` (it uses ANSI color codes).
To generate your own banner: `figlet -f slant "your name"`
