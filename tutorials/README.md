# 教学录像

RoboDK 操作与编程的屏幕录制，共 3 节。

## 目录

| 文件 | 大小 | 内容 |
| --- | --- | --- |
| `01-robotstudio-preprocessing.mkv` | 162 MB | RobotStudio 中的模型预处理 |
| `02-robodk-preprocessing.mkv` | 136 MB | RoboDK 中的模型与工作站预处理 |
| `03-robodk-single-arm-pick-and-place.mkv` | 115 MB | RoboDK 单机械臂抓取程序编写 |

## 播放

视频为 Matroska（`.mkv`）格式。GitHub 网页播放器不支持 MKV，Safari /
QuickTime 也无法打开，请使用：

- **VLC**（跨平台，推荐）
- **PotPlayer**（Windows）
- **mpv**（跨平台）

需要浏览器播放可本地转换（不影响仓库内容）：

```bash
ffmpeg -i 01-robotstudio-preprocessing.mkv -c copy 01-robotstudio-preprocessing.mp4
```

## 关于 Git LFS

三个文件都超过 GitHub 100 MB 单文件硬限制，因此必须通过 Git LFS 存储，
合计约 0.4 GiB（免费账户额度 10 GiB）。

克隆时跳过视频：

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone <repository-url>
```

之后单独拉取需要的某一节：

```bash
git lfs pull --include="tutorials/videos/01-*.mkv"
```

查看本地已下载状态（`*` 已下载，`-` 仅指针）：

```bash
git lfs ls-files
```

> 注意：LFS 存储按版本累计。若要更新内容，请使用新文件名，不要覆盖已有文件。
