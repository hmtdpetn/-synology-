# -synology-

本仓库提供了一份详尽的群晖 (Synology) NAS 数据恢复指南，旨在帮助用户在 NAS 发生故障时，利用 PC 和 Linux 环境安全地找回宝贵数据。包含详细步骤、截图示例及实际操作中的踩坑经验。

## 从故障群晖 NAS 中恢复数据：一份基于 PC 和 Ubuntu 的详细指南

当您的群晖 (Synology) NAS 突然无法访问，数据安全受到威胁时，不要绝望！本仓库提供了一份经过实践检验的数据恢复方案，指导您如何使用一台个人电脑和 Ubuntu 虚拟机环境，尝试从故障 NAS 的硬盘中找回您的宝贵数据。

### 本指南的核心恢复策略包括：

1.  在 VMware Workstation (或其他虚拟机软件) 中正确安装和配置 Ubuntu 18.04 LTS。
2.  解决将 NAS 硬盘（通过 USB 硬盘盒）稳定连接并被 Ubuntu 虚拟机识别的各种技术细节（包括关键的 VMware USB 控制器设置调整）。
3.  使用 Linux 下的 `mdadm` 工具来识别和组装 Synology 的 RAID 阵列。
4.  利用 `lvm2` 工具来激活和访问 Synology 的 LVM 逻辑卷。
5.  安全地挂载数据卷并进行数据备份。

### 详细操作指南及经验总结：

完整的图文教程、每一步的命令、我们在此次恢复过程中遇到的挑战（例如 VMware 共享文件夹的自动挂载、特定系统错误的排查等）以及最终的解决方案，都已整理成 PDF 文档 **`群晖NAS故障后使用PC恢复数据详细教程.pdf`**，存放于本仓库中，供您下载参考。

### 参考资料：

* **群晖官方恢复指南：** [当我的 Synology NAS 出现故障时，如何使用 PC 恢复数据？](https://kb.synology.cn/zh-cn/DSM/tutorial/How_can_I_recover_data_from_my_DiskStation_using_a_PC)

希望这份努力能帮助到更多需要的人！
