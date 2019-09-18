## How to make it

### OS require
    Ubuntu 14.04 LTS x86_64 (16.04 LTS is OK)
    At least 2G RAM & 2 CPU Cores
    At least 25G HDD

### Install the necessary packages
```sudo apt-get -y install build-essential asciidoc binutils bzip2 gawk gettext git libncurses5-dev libz-dev patch unzip zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs git-core gcc-multilib g++-multilib p7zip p7zip-full msmtp libssl-dev texinfo libglib2.0-dev xmlto qemu-utils upx libelf-dev autoconf automake libtool autopoint ccache```

### Clone the source
```git clone https://github.com/coolsnowwolf/lede && cd lede```
```./scripts/feeds update -a && ./scripts/feeds install -a```

### Configure your firmware
```make menuconfig```

### Make it
```make -j1 V=s```

---

插件及参考 by https://github.com/project-openwrt
