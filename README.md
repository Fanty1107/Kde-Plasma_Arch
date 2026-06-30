# KDE Plasma Arch Configuration

This repository contains my personal KDE Plasma desktop environment configuration, exported and managed using [Konsave](https://github.com/Prayag2/konsave). 

Due to the size of the configuration assets (such as custom themes, icon packs, and wallpapers), this repository utilizes Git Large File Storage (LFS) to host the backup file (`kdeconfig-murasaki.knsv`).

---

## Prerequisites

Before restoring this backup on a new Arch Linux installation, ensure you have the following dependencies installed on your system:

1. **KDE Plasma** (Desktop Environment)
2. **Konsave** (Configuration manager)
3. **Git LFS** (To properly download the large configuration file)

You can install the required packages using your preferred package manager:

```bash
# Install Git LFS
sudo pacman -S git-lfs
git lfs install

# Install Konsave (using an AUR helper like yay)
yay -S konsave
```

## 1. Clone the repository
Since this repository uses Git LFS, cloning it normally will automatically fetch the large .knsv file as long as you have Git LFS installed on your system.
```bash
git clone https://github.com/Fanty1107/Kde-Plasma_Arch.git
cd Kde-Plasma_Arch
```
## 2. Import config
Load the backup file into Konsave:
```bash
konsave -i kdeconfig-murasaki.knsv
```
## 3 Apply the profile

```bash
konsave -a kdeconfig-murasaki.knsv
```
Note: Depending on the changes applied, you may need to log out and log back into your user session, or restart Plasma, for all visual modifications and widgets to take full effect.


