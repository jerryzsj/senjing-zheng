# Windows10 + Ubuntu22.04 双硬盘双系统安装指南（UEFI/GPT）
## 环境
- 双硬盘：Disk0=Windows10；Disk1=Ubuntu22.04
- 启动模式：UEFI + GPT；独立引导、互不覆盖

## 1. 前期准备
### 1.1 检查启动模式
Win+R → msinfo32 → BIOS模式=UEFI

### 1.2 准备U盘
- Ubuntu22.04 ISO
- Rufus制作：GPT + UEFI(non-CSM)

### 1.3 Windows设置
- 关闭BitLocker、关闭快速启动

## 2. BIOS设置
- Boot Mode: UEFI Only
- Secure Boot: Disable
- 启动顺序：U盘→Win盘→Ubuntu盘

## 3. 安装Ubuntu（Disk1）
1. U盘启动→Install Ubuntu→其他选项（手动分区）
2. Disk1分区：
   - /boot/efi: 512MB FAT32
   - swap: 8G(内存8G)
   - /: 剩余全部 ext4
3. 引导器安装位置：**整个Disk1**（不是Disk0）
4. 完成重启，拔掉U盘

## 4. 双系统引导
- 进入Ubuntu执行：sudo update-grub → 自动识别Windows
- 开机GRUB菜单选择系统
