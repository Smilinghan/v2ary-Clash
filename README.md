#下载安装

#V2Ray 在以下平台中可用：

Windows 7 及之后版本（x86 / amd64 / arm32）；

macOS 10.10 Yosemite 及之后版本（amd6 / arm64）；

Linux 2.6.23 及之后版本（x86 / amd64 / arm / arm64 / mips64 / mips / riscv64）；

包括但不限于 Debian 7 / 8、Ubuntu 12.04 / 14.04 及后续版本、CentOS 7 / 8、Arch Linux 等；

FreeBSD (x86 / amd64)；

OpenBSD (x86 / amd64)；

Dragonfly BSD (amd64)；

#下载 V2Ray

预编译的二进制 ZIP 格式压缩包可在 Github Releases (opens new window)中找到。下载对应平台的压缩包，解压后即可使用。

#验证安装包

#V2Ray 提供两种验证方式：

ZIP 压缩包的 SHA1 / SHA256 摘要，在每个安装包对应的 .dgst 文件中可以找到。使用方式：v2ray verify --sig=Release /path/to/your/downloaded/v2ray/zip/file

可复现构建：github.com/v2fly/reproducible-builds(opens new window)


#Windows 安装方式

在 Github Releases (opens new window)下载适用于 Windows 平台的 ZIP 压缩包，解压后可得到可执行文件 v2ray.exe，然后通过命令行带参数运行即可

通过 Scoop (opens new window)包管理器安装：scoop install v2ray


#macOS 安装方式

在 Github Releases (opens new window)下载适用于 macOS 平台的 ZIP 压缩包，解压后可得到可执行文件 v2ray，然后通过命令行带参数运行即可

通过 Homebrew (opens new window)包管理器安装：brew install v2ray，随命令一起下载的 geosite.dat 和 geoip.dat 放置在 /usr/local/share/v2ray/ 目录下


#Linux 安装方式

#安装脚本

请查看 GitHub 仓库：https://github.com/v2fly/fhs-install-v2ray

#Linux 发行版包管理器

Linux 发行版提供的 V2Ray 包（可通过发行版相应的包管理器安装）：

Debian：https://tracker.debian.org/pkg/golang-v2ray-core

Arch Linux：https://tracker.debian.org/pkg/golang-v2ray-core

#更新软体仓库并安装 V2Ray：

apt update

apt install v2ray

注意：由于该包在 v2ray.service 中使用了 DynamicUser=true，如果你想向 /var/log/v2ray/ 目录档中写入 Log，请执行并写入：

#Linuxbrew 包管理器


Linuxbrew (opens new window)包管理器的使用方式与 Homebrew 一致：brew install v2ray

#Docker 安装方式


V2Ray 为 Linux 平台提供了预编译的 Docker image：v2fly/v2fly-core(opens new window)

GitHub 仓库：github.com/v2fly/docker(opens new window)


#Docker image 的文件结构：


/etc/v2ray/config.json：配置文件

/usr/bin/v2ray：V2Ray 主程序

/usr/bin/v2ctl：V2Ray 辅助工具

/usr/local/share/v2ray/geoip.dat：IP 数据文件

/usr/local/share/v2ray/geosite.dat：域名数据文件
