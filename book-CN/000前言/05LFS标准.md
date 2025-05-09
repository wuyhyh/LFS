LFS 的结构尽可能遵循 Linux 标准。主要标准包括：

POSIX.1-2008。

文件系统层次结构标准 (FHS) 版本 3.0

Linux 标准库 (LSB) 版本 5.0 (2015)

LSB 有四个独立的规范：核心规范、桌面规范、语言规范和图像规范。核心规范和桌面规范的某些部分是特定于体系结构的。此外还有两个试用规范：Gtk3
和图形规范。LFS 尝试遵循上一节中讨论的 IA32（32 位 x86）或 AMD64（x86_64）体系结构的 LSB 规范。

[笔记] 笔记
许多人并不认同这些要求。LSB 的主要目的是确保专有软件能够在兼容的系统上安装和运行。由于 LFS 是基于源代码的，用户可以完全控制所需的软件包；您可以选择不安装
LSB 指定的某些软件包。

虽然可以“从零开始”创建一个能够通过 LSB 认证测试的完整系统，但这离不开许多超出 LFS 手册范围的附加软件包。部分附加软件包的安装说明可在
BLFS 中找到。

LFS 提供的满足 LSB 要求的软件包
LSB核心：

Bash、Bc、Binutils、Coreutils、Diffutils、File、Findutils、Gawk、GCC、Gettext、Glibc、Grep、Gzip、M4、Man-DB、Procps、Psmisc、Sed、Shadow、SysVinit、Tar、Util-linux、Zlib

LSB 桌面：

没有任何

LSB 语言：

Perl

LSB成像：

没有任何

LSB Gtk3 和 LSB Graphics（试用）：

没有任何

BLFS 提供的满足 LSB 要求的软件包
LSB核心：

At、Batch（At 的一部分）、BLFS Bash 启动文件、Cpio、Ed、Fcrontab、LSB-Tools、NSPR、NSS、Linux-PAM、Pax、Sendmail（或 Postfix 或
Exim）、时间

LSB 桌面：

Alsa、ATK、Cairo、桌面文件实用程序、Freetype、Fontconfig、Gdk-pixbuf、Glib2、GLU、图标命名实用程序、Libjpeg-turbo、Libxml2、Mesa、Pango、Xdg-utils、Xorg

LSB 语言：

Libxml2、Libxslt

LSB成像：

CUPS、Cups 过滤器、Ghostscript、SANE

LSB Gtk3 和 LSB Graphics（试用）：

GTK+3

LFS 或 BLFS 未提供或可选提供的组件，需要满足 LSB 要求
LSB核心：

install_initd， libcrypt.so.1（可以为 LFS Libxcrypt 包提供可选说明），libncurses.so.5 （可以为 LFS Ncurses
包提供可选说明），libncursesw.so.5（但libncursesw.so.6由 LFS Ncurses 包提供）

LSB 桌面：

libgdk-x11-2.0.so（但 libgdk-3.so由 BLFS GTK+-3 包提供），libgtk-x11-2.0.so（但libgtk-3.so由libgtk-4.soBLFS GTK+-3 和 GTK-4
包提供），libpng12.so（但libpng16.so由 BLFS Libpng 包提供），libQt*.so.4 （但libQt6*.so.6由 BLFS Qt6
包提供），libtiff.so.4（但libtiff.so.6由 BLFS Libtiff 包提供）

LSB 语言：

/usr/bin/python（LSB 需要 Python2，但 LFS 和 BLFS 仅提供 Python3）

LSB成像：

没有任何

LSB Gtk3 和 LSB Graphics（试用）：

libpng15.so（但libpng16.so由 BLFS Libpng 包提供）

