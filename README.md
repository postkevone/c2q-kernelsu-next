# KernelSU Next integration for the Note20 Ultra Snapdragon variant (c2q)

This kernel was built for the `SM-N986N` (Korean variant), with firmware `N986NKSSAHYH1`.

<img src="https://i.imgur.com/O4wGqMo.jpeg" width="300" />

# How to install

Flash the latest `c2q_ksunext.zip` from the release page with TWRP.

# How to build
This repo was tested on Ubuntu 22.04 LTS (Jammy Jellyfish).

## Install the dependencies

```sh
sudo apt install -y build-essential libncurses5 libncurses5-dev flex bison libssl-dev \
zlib1g-dev lz4 cpio git wget bc python2 python3 openssh-client android-tools-mkbootimg p7zip-full
```

## Clone the repo

```sh
git clone --recursive https://github.com/postkevone/c2q-kernelsu-next.git
cd c2q-kernelsu-next
```

## Set python2 as default
```sh
sudo ln -sf python2 /usr/bin/python
```
## Run the build script
```sh
./build_kernel.sh
```
