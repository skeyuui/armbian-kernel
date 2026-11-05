# armbian-kernel

Personal build. Armbian's `current` kernel for my Orange Pi Zero 3, with binder, binderfs, PSI and 32-bit compat switched on so Redroid runs on it. Everything else is stock Armbian. No support, use at your own risk.

Builds run from **Actions → build-kernel → Run workflow** and land in Releases.

## Usage

```bash
mkdir -p ~/kernel && cd ~/kernel
R=https://github.com/skeyuui/armbian-kernel/releases/latest/download
wget -q $R/kernel-debs.tar $R/SHA256SUMS
sha256sum -c --ignore-missing SHA256SUMS && tar -xf kernel-debs.tar
```