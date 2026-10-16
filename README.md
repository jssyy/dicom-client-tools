# 医学影像系统实施运维工具

DICOM 联调、文件工具和现场诊断客户端的发行版下载仓库。

从 [最新发行版](https://github.com/jssyy/dicom-client-tools/releases/latest) 下载 Windows 客户端。ZIP 解压后运行 DicomOpsTool.exe，或使用 EXE 单文件版。

## 检查更新

在程序中打开「帮助 → 检查更新 → 发布源设置」，选择「内网清单 latest.json（共享目录 / 内网网址）」，填入以下地址并保存。这个选项同样支持公网 HTTPS 地址：

```text
https://github.com/jssyy/dicom-client-tools/releases/latest/download/latest.json
```

点击「检查更新」即可。当前版本等于最新版本时显示已是最新版本；以后发布更高版本后可下载并升级。升级时保留现场配置和影像目录。访问 GitHub 需要可用的网络连接。

本仓库当前用于分发客户端安装包和更新清单。
