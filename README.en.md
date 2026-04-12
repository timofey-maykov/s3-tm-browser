# S3 TM Browser

Русская версия: [README.md](README.md)  
中文版本: [README.zh.md](README.zh.md)

S3 TM Browser is a cross platform desktop application for S3 object storage.
It works with AWS S3 and S3 compatible services.
Supported platforms are macOS, Windows, and Linux.

## Application Features

- Multiple connections, endpoints, and regions
- Support for AWS S3 and S3 compatible backends
- Bucket and object browsing in table view; multi-page listing progress with cancel; export the current object list to JSON or CSV from the toolbar
- Object search and filtering, including deep key search under the current prefix with caps and cancel
- Toolbar total size estimate for the current prefix or the current selection (objects and folder prefixes)
- Bucket create and delete actions
- File and folder upload
- File, folder, and full bucket download
- Parallel large-object download over HTTP Range: in multipart options set part size and concurrent Range requests per object (up to 128, subject to an in-flight buffer budget); the transfer queue shows segment-style progress similar to multipart upload
- Drag and drop upload
- Copy and move objects across buckets and profiles; migration wizard (access checks, prefix size estimate, queue prefix copy)
- File and folder rename
- Single and bulk delete
- Transfer queue with pause, resume, and cancel; rough remaining time and a live speed line; task details with progress bar and parsed source and destination; subtle progress highlight for active tasks
- Operation status, progress, and error details
- Multipart upload support
- Incomplete multipart upload list and abort actions
- Object versioning workflow
- Version list, download, restore, and delete
- Object metadata and tags view
- Metadata and tag editing
- Object and bucket ACL management
- Bulk ACL actions for selected objects
- Bucket Object Lock management, object retention, and legal hold
- Per object server side encryption: SSE-S3, SSE-KMS, SSE-C; remove encryption via same key copy; SSE-C key in the profile keyring or optional one time base64 key in the dialog; bulk decrypt for selected keys and prefixes in a dedicated dialog with base64 key validation
- Presigned URL generation
- Virtual host and path style static links
- Object preview for supported content
- Bucket settings management
- Bucket Policy, CORS, Lifecycle, Encryption, Logging, Versioning, and Object Lock
- Public Access Block controls
- Dual pane Commander mode
- Copy and sync between panes
- Diff view for two S3 panes
- Browse toolbar: copy rclone block and AWS CLI examples for the current prefix (no secrets)
- Browse toolbar context menu: show or hide toolbar buttons and table columns, fit column widths to content, reset layout
- S3 Inventory keys: CSV, `csv.gz`, or `manifest.json`; queue batched copy for parsed keys
- Hotkeys for common operations
- Global and per profile proxy settings (HTTP and env auto mode); vendor preset for S3-compatible endpoints to improve error hints
- App options for queue, retries, bandwidth limits, multipart (upload and download part sizes, parallel upload parts and parallel ranged downloads per object, up to 128 with an in-flight buffer cap), download integrity (sha256 and crc32c from metadata and HEAD checksums), small-upload checksum choice, and logs
- Diagnostics snapshot for support cases
- UI available in Russian, English, and Chinese; in-app Help under Settings with table of contents and search
- `s3tm-cli` for terminal workflows
- S3 Browser import on Windows

## Audience

S3 TM Browser is built for admins, developers, and teams
that need a clear desktop tool for daily S3 operations.

## Support the project

- Boosty: https://boosty.to/itnitro
- WeChat: `itnitro` (QR: [screenshots/wechat-itnitro-qr.png](screenshots/wechat-itnitro-qr.png))
- USDT (TON): `UQBZhwBuZCgQOtrgRGMu4PKiiOcf9dTKxRpapZt1oDn0m3yH`
- USDT/ETH (ERC-20): `0xeb05803030afB64C903C7BfB79d18957efD6bcCd`
- SOL (Solana): `GcKxgUeSfKnsPL9iEaYKJArosfYKMtE4W5wVDdHrRVTu`
- BTC (Bitcoin): `bc1qcyd3kaa3y2cv2yn90rsa628y3ptz56zs05z2jq`
