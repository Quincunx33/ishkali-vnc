# Tasfia's Hacker Lab — টুলিস্ট (v7)

**rootfs:** Alpine Linux 3.14 x86 (i386) — Alpine Linux 3.14 অফিসিয়াল রিপো
**মোট:** ২২৫+ প্যাকেজ | ৯২৫+ executable command | missing dependency: 0

---

## 🕵️ Pentest / Network Security

| Tool | কাজ |
|---|---|
| `nmap` | Network scan, port discovery, OS detection |
| `masscan` | আল্ট্রা-ফাস্ট পুরো ইন্টারনেট স্ক্যান |
| `sqlmap` | SQL Injection automation |
| `nikto` | Web server vulnerability scanner |
| `zmap` | এক সময়ে সমগ্র নেট স্ক্যান |
| `tcpdump` / `tshark` | Packet capture (live ও file analyze) |
| `radare2` | Reverse engineering, binary analysis |
| `strace` / `ltrace` | System/library call tracing |
| `netcat` / `socat` / `stunnel` | Port listen, tunnel, TCP/UDP relay |
| `tcpflow` / `tcpflow-doc` | TCP stream reassembly |
| `dnsrecon` / `dig` / `whois` | DNS recon |
| `macchanger` | MAC address change |
| `proxychains-ng` | Tor/proxy দিয়ে যেকোনো app চালানো |
| `tor` | Anonymous browsing/traffic |
| `sshpass` | Non-interactive SSH login |
| `iperf` / `iperf3` | Network speed test |
| `net-tools` | ifconfig, netstat, route |
| `arping` | ARP-level network discovery |

## 💻 Dev Tools

| Tool | কাজ |
|---|---|
| `gcc` / `g++` | C/C++ compiler |
| `node` / `npm` / `node-gyp` | JavaScript + build tools |
| `python3` + `pip3` | Python + package installer |
| `ruby` + `bundler` | Ruby |
| `perl` | Perl scripting |
| `lua5.3` / `tcl` / `expect` | Scripting + automation |
| `erlang` / `elixir` / `zig` (build from src) | Modern languages |
| `gcc` / `make` / `cmake` / `meson` | Build systems |
| `bison` / `flex` / `automake` / `autoconf` | Compiler tools |
| `gdb` / `valgrind` | Debugging + memory check |
| `yasm` / `nasm` | Assembler |
| `git` / `subversion` | Version control |
| `patch` / `diffutils` | Code patches |
| `doxygen` / `cppcheck` / `flawfinder` | Docs + static analysis |
| `ccache` / `distcc` | Fast/distributed compilation |
| `swig` | Binding generator |
| `sqlite3` | Local database |
| `emacs` / `micro` / `nano` | Advanced editors |

## ✏️ Editors (নতুন)

| Tool | বিশেষত্ব |
|---|---|
| `neovim (nvim)` | Modern vim — plugin-rich |
| `vim` / `gvim` | Classic vim |
| `nano` | সহজ editor |
| `micro` | Modern সহজ editor, mouse support |
| `joe` / `mg` / `vis` / `bvi` | পুরনো-স্টাইল lightweight editors |
| `ed` / `hexedit` | Terminal এবং binary editing |
| `xxd` | Hex dump |

## 🐚 Shells (নতুন)

`bash` (default), `zsh`, `fish`, `tcsh`, `dash` + `bash-completion` (Tab completion)

## 🌐 Network / File Transfer

| Tool | কাজ |
|---|---|
| `curl` / `wget` / `curlie` | Web download |
| `lynx` / `w3m` / `links` | Text-mode web browser |
| `rsync` | Fast file sync |
| `smbclient` | Windows share access |
| `sshfs` | SSH remote folder mount |
| `openvpn` / `wireguard-tools` | VPN |
| `rdesktop` / `freerdp` | Windows RDP client |
| `aria2` / `lftp` | Fast multi-source downloader |
| `nfs-utils` / `cifs-utils` | NFS/SMB mount tools |
| `mtr` / `iftop` / `nethogs` | Ping path + network monitor |

## 📦 Archive / Compression

`zip` / `unzip` / `7z` (p7zip) / `xz` / `zstd` / `tar` / `gzip` / `bzip2` / `cabextract`

## 📊 System / Monitor

`htop` / `atop` / `sysstat` (iostat, sar) / `procps` (ps, top, free) / `ncdu` / `dust` / `tree` / `tig` (git TUI) / `lsof` / `pv` / `bc` / `colordiff` / `jq` / `yq` / `cloc` / `tokei` (code counter)

## 🎵 Media

`ffmpeg` / `mpv` / `mplayer` / `imagemagick` / `graphicsmagick` / `sox` / `lame` / `flac` / `opus-tools` / `vorbis-tools` / `cmus` / `moc` / `mpd` / `scrot` (screenshot) / `feh` (image viewer)

## 🖥️ X11 / VNC

`x11vnc` + `x11vncfull` / `Xvfb` / `xterm` / `twm` / `openbox` / `xauth` / `xdpyinfo` / `xeyes` / `xclock` / `xcalc` / `xscreensaver` / `xset` / `dialog` + `startvnc` script

## 🎭 Fun / TUI

`cmatrix` / `asciiquarium` / `sl` / `fortune` / `figlet` / `asciinema` (record) / `neofetch` / `tmux` / `screen`

## 🐍 Python Packages (pre-installed)

`scapy` / `impacket` / `pyftpdlib` / `pysocks` / `psutil` / `requests` / `lxml` / `paramiko` / `cryptography` / `flask` / `tornado` / `pytest` / `pyyaml` / `beautifulsoup4` / `jinja2` / `pexpect` / `pyserial` / `virtualenv` + `pip3` available for more

---

## ⚠️ যা এখনো নেই (Alpine 3.14-এ নেই / বড়)

- `john` (JtR), `gobuster`, `ffuf`, `hydra` — ৩.১৪ রিপোতে নেই
- `java` / `metasploit` / `Burp Suite` — iSH-এ অসম্ভব
- `php` (light) — চাইলে v8-এ যোগ করা যায়

**বাকি থাকা যোগ করার উপযোগী tool (v8-এ):** `aircrack-ng`, `httpie`, `man` pages, `psmisc` (fuser/pstree), `freerdp`, `elinks`, `aria2`, `lftp`, `dropbear`, `neofetch`, `xdotool`, `xclip`, `erlang`, `elixir`, `lua5.4`, `gifsicle`, `optipng`, `pngcrush`, `audacious`, `openssh-server`

চাইলে বলুন — v8 বানিয়ে দেব! 😊
