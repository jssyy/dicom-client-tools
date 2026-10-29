# 医学影像系统实施运维工具

客户端安装包、更新日志与自动更新清单下载。当前发行版：**V1.1.0.63（2026-10-29）**。

- [Gitee 国内下载](https://gitee.com/amumu/dicom-client-tools-releases/releases/latest)
- [GitHub 下载](https://github.com/jssyy/dicom-client-tools/releases/latest)
- [本版更新日志](https://github.com/jssyy/dicom-client-tools/releases/tag/V1.1.0.63)

## 选择对应系统的版本

| 系统 | 安装包 | 启动方式 |
| --- | --- | --- |
| Windows 10 / 11，64 位 | `DicomOpsTool_V1.1.0.63.zip` | 完整解压后运行 `DicomOpsTool.exe` |
| Windows 10 / 11，64 位，单文件 | `DicomOpsTool_V1.1.0.63.exe` | 直接运行，可改名为 `DicomOpsTool.exe` |
| Windows 7 SP1，64 位 | `DicomOpsTool_win7_V1.1.0.63.zip` | 完整解压后运行 `DicomOpsTool_win7.exe` |

Win7 与 Win10 分别打包，不能混用。Win7 需 SP1、KB3063858（或 KB2533623）、KB2999226。
兼容包使用独立 PythonWin7 / Qt5；本轮通过运行环境测试、打包启动和静态 API 检查，未作新的 Win7 实机复测。

## 已安装用户更新

打开“帮助 → 检查更新”，选择“自动选择（Gitee 优先 / GitHub 备用）”。
程序按当前运行包类型选择对应平台，下载后校验 SHA256；支持同版本备用源和失败恢复，保留现场配置、影像和任务历史。
更新窗口显示当前版本及 Win7 / Win10 程序类型。自定义内网更新清单继续保留。

## 手动下载

GitHub 提供完整 EXE 与 ZIP。Gitee 提供分卷；把同一包的 `.001`、`.002`、`.003` 全部下载，
与对应的 `Merge_*.cmd` 放在同一目录。双击脚本合并并校验，ZIP 再完整解压。
程序自动更新会自行完成分卷下载、合并和校验。

请下载程序附件；“Source code” 自动快照仅是本下载仓库的说明文件，不是安装包。
发布包不包含现场账号配置、源影像、任务记录或报告；升级前保留现有数据。

## 本版主要更新

- SVS、KFB、NDPI 转 DICOM WSI，保留金字塔和物理分辨率；CSP 为实验支持，尚缺真实样本验证。
- 五种无损语法：JPEG 2000、JPEG-LS、JPEG Lossless SV1、JPEG Lossless Process 14、RLE。
- HTTP/HTTPS 接口测试、Token 获取、cURL 导入复制、JSON 折叠与文件上传。
- SCP 本地 / Windows 共享 / S3 存储、影像库查询取图、复制删除。
- 并发重试、逐检查性能报告、实时进度、就地结果提示及任务历史管理。
