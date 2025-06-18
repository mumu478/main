# Linux系统部署和核心命令

---

# 一、Ubuntu系统安装

# Linux系统部署和核心命令

---

# 一、Ubuntu系统安装

官方下载地址：https://cn.ubuntu.com/server

国内镜像下载地址：https://mirrors.aliyun.com/ubuntu-releases

> 现最新稳定版本为：24.04.2   偶数开头版本为稳定版本

![image-20250617101444621](E:\hmlinux\day02\笔记\assets\image-20250617101444621.png)

Ubuntu Server 是一个广受欢迎的开源操作系统，基于 Linux 内核，由 Canonical 公司维护和发布。它以其稳定性、易用性和广泛的社区支持而闻名，特别适合用于构建服务器、云计算和容器化应用。

主要特性: 

- **开源免费**：任何人都可以免费下载、安装和使用。
- **定期更新**：每两年发布一个长期支持 (LTS) 版本，提供 5 年的更新和支持。
- **广泛的硬件支持**：支持主流服务器硬件和架构，包括 x86、ARM、PowerPC 等。
- **轻量级**：相比桌面版，Server 版不包含图形界面（GUI），资源占用低。

版本种类

- **LTS（长期支持）版本**：如 Ubuntu Server 24.04.2 LTS，是生产环境的推荐版本。
- **非 LTS 版本**：每 6 个月发布一次，支持时间较短，适合测试或实验。

![image-20250615223429500](E:\hmlinux\day02\笔记\assets\image-20250615223429500.png)

>  详细安装步骤见 资料目录 下的《Ubuntu Server操作系统安装与配置.pdf》文件

# 二、服务器基础配置

> 以centos图形界面来操作，后期都为命令字符下完成。

## 2.1、设置主机名

- 主机名配置：
  - 配置服务器的主机名，确保符合公司命名规范。
- 网络配置（静态IP地址配置）
  - 配置静态IP地址，保证服务器的网络连通性。
    <img src="E:\hmlinux\day02\笔记\assets\image-20250615223704257.png" style='zoom:.5'/>
    <img src="E:\hmlinux\day02\笔记\assets\image-20250615223720463.png" style='zoom:.4'/>

## 2.2、网络配置（静态IP地址配置）

先关机服务器系统，再到虚拟机中选择编辑，进行网络配置

![image-20250617145403875](E:\hmlinux\day02\笔记\assets\image-20250617145403875.png)

虚拟网络编辑器中选中Nat

![image-20250617145553563](E:\hmlinux\day02\笔记\assets\image-20250617145553563.png)

修改子网ip的第3个位置的网段为88，可以不修改，但为了后续的实验统一在一个网段名称一致。

![image-20250617150156145](E:\hmlinux\day02\笔记\assets\image-20250617150156145.png)

修改网关

![image-20250617150302966](E:\hmlinux\day02\笔记\assets\image-20250617150302966.png)

在宿主机中打开网络设置

![image-20250617150406994](E:\hmlinux\day02\笔记\assets\image-20250617150406994.png)

<img src="E:\hmlinux\day02\笔记\assets\image-20250615223807218.png" style='zoom:.5'/>
<img src="E:\hmlinux\day02\笔记\assets\image-20250615223816540.png" style='zoom:.4'/>
<img src="E:\hmlinux\day02\笔记\assets\image-20250615223826926.png" style='zoom:.4'/>

# 三、远程连接工具

