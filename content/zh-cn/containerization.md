---
title: 容器化
status: Completed
category: 技术
tags: ["应用程序", "", ""]
---

## 是什么

容器化是将一个应用程序及其依赖关系捆绑到 [容器图像](/zh-cn/container-image/) 中的过程。
容器构建过程需要遵守 [开放容器倡议](https://opencontainers.org)(OCI) 标准。
只要输出的是一个符合这个标准的容器镜像，使用哪种容器化工具并不重要。

## 解决的问题 

在容器盛行之前，企业依靠虚拟机 (VMs) 在一台 [裸机](/bare-metal-machine/) 上协调多个应用程序。
虚拟机比容器大得多，需要一个管理程序来运行。由于这些较大的虚拟机模板的存储、备份和传输，创建虚拟机模板也很慢。
此外，虚拟机可能会出现配置漂移，这违反了 [不变性](/immutable-infrastructure/) 的原则。

## 如何帮助

容器图像是轻量级的（与传统的虚拟机不同），容器化过程需要一个带有依赖性列表的文件。
这个文件可以被版本控制，构建过程也可以自动化，允许一个组织在自动化过程中关注其他优先事项。
容器镜像由一个唯一的标识符来存储，该标识符与它的确切内容和配置相联系。
当容器被安排和重新安排时，它们总是被重置为其初始状态，从而消除了配置漂移。
