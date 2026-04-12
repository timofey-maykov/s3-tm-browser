# S3 TM Browser

Русская версия: [README.md](README.md)  
English version: [README.en.md](README.en.md)

S3 TM Browser 是一个跨平台的桌面应用，用于管理 S3 对象存储。  
支持 AWS S3 和兼容 S3 的服务。  
支持的平台包括 macOS、Windows 和 Linux。

## 应用功能

- 支持多个连接、endpoint 和 region
- 支持 AWS S3 与 S3 兼容存储
- 以表格方式浏览 bucket、prefix 和对象；多页列举进度与取消；从工具栏导出当前列表为 JSON 或 CSV
- 支持对象搜索与过滤（含当前前缀下的深度键搜索，可设上限并取消）
- 浏览工具栏：估算当前前缀或当前选中对象与文件夹前缀的总大小
- 创建和删除 bucket
- 上传文件与文件夹
- 下载文件、文件夹和整个 bucket
- 大对象并行分片下载（HTTP Range）：在 multipart 选项中设置分片大小与单对象并发 Range 数（最高 128，并受在途缓冲总量限制）；传输队列中显示与 multipart 上传类似的分段进度
- 支持拖拽上传
- 在不同 bucket 和 profile 之间复制、移动对象；迁移向导（连通性检查、前缀体量估计、将前缀复制加入队列）
- 重命名文件和文件夹
- 单个与批量删除对象
- 传输队列支持暂停、继续、取消；按进度估算剩余时间并显示速度行；任务详情含进度条及解析出的来源与目标；进行中的任务进度条带轻微强调效果
- 显示任务状态、进度与错误详情
- 支持 multipart 上传
- 查看并中止未完成的 multipart 上传
- 支持对象版本管理
- 查看、下载、恢复、删除对象版本
- 查看对象元数据与标签
- 编辑自定义元数据与标签
- 管理对象与 bucket ACL
- 对选中对象执行批量 ACL 操作
- 管理 bucket Object Lock，以及对象 retention 和 legal hold
- 对象级服务端加密：SSE-S3、SSE-KMS、SSE-C；通过同键复制移除加密；SSE-C 密钥可存于 profile 的 keyring，或在对话框中一次性粘贴 base64；对所选键与前缀的批量解密在独立对话框中完成并校验 base64 密钥
- 生成 presigned URL
- 查看 virtual-host 和 path-style 静态链接
- 预览可支持类型的对象内容
- 管理 bucket 设置
- Bucket Policy、CORS、Lifecycle、Encryption、Logging、Versioning、Object Lock
- Public Access Block 相关控制
- 双面板 Commander 模式
- 面板间复制与同步
- 比较两个 S3 面板内容差异
- 浏览工具栏：复制 rclone 片段与当前前缀的 AWS CLI 示例（不含密钥）
- 浏览工具栏右键菜单：配置按钮与表格列显示、按内容调整列宽、重置视图
- S3 Inventory：从 CSV、`csv.gz` 或 `manifest.json` 导入键列表；将解析出的键批量加入复制队列
- 常用操作快捷键
- 全局与 profile 级代理设置（HTTP 与环境变量自动模式）；S3 兼容厂商预设以改进错误提示
- 队列、重试、带宽限速、multipart（上传与下载分片大小、单文件上传并行分片数与单对象下载并行 Range 数，最高 128 并受在途缓冲上限约束）、下载完整性（元数据与 HEAD 的 sha256/crc32c）、小文件上传校验算法与日志等应用参数
- 生成用于支持排障的诊断快照
- 界面支持俄语、英语和中文；设置中的内置帮助（目录与搜索）
- `s3tm-cli` 命令行工具（终端场景）
- 支持在 Windows 上导入 S3 Browser 连接

## 适用人群

适合管理员、开发者和团队，  
用于日常高效管理 S3 对象存储。

## 支持项目

- Boosty: https://boosty.to/itnitro
- WeChat: `itnitro`（二维码: [screenshots/wechat-itnitro-qr.png](screenshots/wechat-itnitro-qr.png)）
- USDT (TON): `UQBZhwBuZCgQOtrgRGMu4PKiiOcf9dTKxRpapZt1oDn0m3yH`
- USDT/ETH (ERC-20): `0xeb05803030afB64C903C7BfB79d18957efD6bcCd`
- SOL (Solana): `GcKxgUeSfKnsPL9iEaYKJArosfYKMtE4W5wVDdHrRVTu`
- BTC (Bitcoin): `bc1qcyd3kaa3y2cv2yn90rsa628y3ptz56zs05z2jq`
