# Tasfia's Hacker Lab — Tool List (v7)

**Rootfs:** Alpine Linux 3.14 x86 (i386) — official Alpine 3.14 repositories
**Total:** 225+ packages | 925+ executable commands | missing dependencies: 0

---

## 🕵️ Pentest / Network Security

| Tool | Purpose |
|---|---|
| `nmap` | Network scan, port discovery, OS detection |
| `masscan` | Ultra-fast full-internet port scan |
| `sqlmap` | SQL injection automation |
| `nikto` | Web server vulnerability scanner |
| `zmap` | Whole-network scan in one pass |
| `tcpdump` / `tshark` | Packet capture (live and file analysis) |
| `radare2` | Reverse engineering, binary analysis |
| `strace` / `ltrace` | System / library call tracing |
| `netcat` / `socat` / `stunnel` | Port listening, tunnels, TCP/UDP relay |
| `tcpflow` / `tcpflow-doc` | TCP stream reassembly |
| `dnsrecon` / `dig` / `whois` | DNS reconnaissance |
| `macchanger` | MAC address spoofing |
| `proxychains-ng` | Run any app through Tor / proxies |
| `tor` | Anonymous browsing and traffic |
| `sshpass` | Non-interactive SSH login |
| `iperf` / `iperf3` | Network speed testing |
| `net-tools` | `ifconfig`, `netstat`, `route` |
| `arping` | ARP-level network discovery |

## 💻 Development Tools

| Tool | Purpose |
|---|---|
| `gcc` / `g++` | C / C++ compilers |
| `node` / `npm` / `node-gyp` | JavaScript + build toolchain |
| `python3` + `pip3` | Python + package installer |
| `ruby` + `bundler` | Ruby + dependency manager |
| `perl` | Perl scripting |
| `lua5.3` / `tcl` / `expect` | Scripting + automation |
| `gcc` / `make` / `cmake` / `meson` | Build systems |
| `bison` / `flex` / `automake` / `autoconf` | Compiler toolchain utilities |
| `gdb` / `valgrind` | Debugging + memory checking |
| `yasm` / `nasm` | Assemblers |
| `git` / `subversion` | Version control |
| `patch` / `diffutils` | Code patching |
| `doxygen` / `cppcheck` / `flawfinder` | Documentation + static analysis |
| `ccache` / `distcc` | Fast / distributed compilation |
| `swig` | Binding generator |
| `sqlite3` | Local database engine |
| `emacs` / `micro` / `nano` | Advanced editors |

## ✏️ Editors

| Tool | Highlights |
|---|---|
| `neovim (nvim)` | Modern vim — plugin-rich |
| `vim` / `gvim` | Classic vim |
| `nano` | Simple editor |
| `micro` | Modern simple editor, mouse support |
| `joe` / `mg` / `vis` / `bvi` | Old-school lightweight editors |
| `ed` / `hexedit` | Terminal and binary editing |
| `xxd` | Hex dumps |

## 🐚 Shells

`bash` (default), `zsh`, `fish`, `tcsh`, `dash` + `bash-completion` (tab completion)

## 🌐 Network / File Transfer

| Tool | Purpose |
|---|---|
| `curl` / `wget` / `curlie` | Web downloads |
| `lynx` / `w3m` / `links` | Text-mode web browsers |
| `rsync` | Fast file synchronization |
| `smbclient` | Windows share access |
| `sshfs` | Mount remote folders over SSH |
| `openvpn` / `wireguard-tools` | VPN clients |
| `rdesktop` / `freerdp` | Windows RDP clients |
| `aria2` / `lftp` | Fast multi-source downloaders |
| `nfs-utils` / `cifs-utils` | NFS / SMB mount tools |
| `mtr` / `iftop` / `nethogs` | Traceroute + bandwidth monitoring |

## 📦 Archive / Compression

`zip` / `unzip` / `7z` (p7zip) / `xz` / `zstd` / `tar` / `gzip` / `bzip2` / `cabextract`

## 📊 System / Monitoring

`htop` / `atop` / `sysstat` (iostat, sar) / `procps` (ps, top, free) / `ncdu` / `dust` / `tree` / `tig` (git TUI) / `lsof` / `pv` / `bc` / `colordiff` / `jq` / `yq` / `cloc` / `tokei` (code counters)

## 🎵 Media

`ffmpeg` / `mpv` / `mplayer` / `imagemagick` / `graphicsmagick` / `sox` / `lame` / `flac` / `opus-tools` / `vorbis-tools` / `cmus` / `moc` / `mpd` / `scrot` (screenshots) / `feh` (image viewer)

## 🖥️ X11 / VNC

`x11vnc` + `x11vncfull` / `Xvfb` / `xterm` / `twm` / `openbox` / `xauth` / `xdpyinfo` / `xeyes` / `xclock` / `xcalc` / `xscreensaver` / `xset` / `dialog` + the `startvnc` launcher script

## 🎭 Fun / TUI

`cmatrix` / `asciiquarium` / `sl` / `fortune` / `figlet` / `asciinema` (terminal recording) / `neofetch` / `tmux` / `screen`

## 🐍 Pre-installed Python Packages

`scapy` / `impacket` / `pyftpdlib` / `pysocks` / `psutil` / `requests` / `lxml` / `paramiko` / `cryptography` / `flask` / `tornado` / `pytest` / `pyyaml` / `beautifulsoup4` / `jinja2` / `pexpect` / `pyserial` / `virtualenv` + `pip3` ready for more

---

## ⚠️ Not included (missing from Alpine 3.14 repos or too heavy)

- `john` (JtR), `gobuster`, `ffuf`, `hydra` — not available in the 3.14 repositories
- `java` / `metasploit` / `Burp Suite` — impossible on iSH
- `php` (lightweight) — can be added on request

**Good candidates for a future v8 release:** `aircrack-ng`, `httpie`, `man` pages, `psmisc` (fuser/pstree), `freerdp`, `elinks`, `aria2`, `lftp`, `dropbear`, `neofetch`, `xdotool`, `xclip`, `erlang`, `elixir`, `lua5.4`, `gifsicle`, `optipng`, `pngcrush`, `audacious`, `openssh-server`
