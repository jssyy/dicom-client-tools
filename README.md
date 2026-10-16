# 医学影像系统实施运维工具

客户端安装包、发布说明与更新清单下载。

- [Gitee 国内下载](https://gitee.com/amumu/dicom-client-tools-releases/releases/latest)
- [GitHub 下载](https://github.com/jssyy/dicom-client-tools/releases/latest)

## V1.1.0.43 双源自动更新

43 版支持 Gitee / GitHub 自动选择、同版本故障切换、分卷自动下载合并和 SHA256 校验。
打开「帮助 → 检查更新」，发布源选择「自动选择（Gitee 优先 / GitHub 备用）」。
旧默认设置会迁移，自定义内网更新源继续保留。

## 首次安装或从 42 版升级

GitHub 可下载完整 EXE 或 ZIP。EXE 单文件版可重命名为 DicomOpsTool.exe 使用；ZIP 解压后运行其中的 DicomOpsTool.exe。

Gitee 单附件限制 100MB。请下载 DicomOpsTool_V1.1.0.43.zip.001、DicomOpsTool_V1.1.0.43.zip.002 和 Merge_DicomOpsTool_V1.1.0.43.cmd，放在同一目录；双击合并脚本，校验通过后解压生成的 ZIP。
两个分卷都必须下载。也可用支持分卷的压缩工具打开 .zip.001。

升级前退出旧程序，保留原有配置和影像目录。请下载程序附件；Source code 自动快照仅包含本下载仓库的说明文件。
