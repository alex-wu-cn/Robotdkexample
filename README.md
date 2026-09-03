# RoboDK Examples

RoboDK 操作与项目资料，分为两条互相独立的线：

| 目录 | 内容 | 说明 |
| --- | --- | --- |
| [`tutorials/`](tutorials/) | 3 段教学录像 | 预处理流程 + 单臂抓取程序编写 |
| [`projects/library-storage/`](projects/library-storage/) | 图书馆收纳项目 | RoboDK 工作站文件（36 MB） |

两条线没有依赖关系，可以只看其中一条。

## tutorials/ — 教学录像

| 文件 | 大小 | 内容 |
| --- | --- | --- |
| `01-robotstudio-preprocessing.mkv` | 162 MB | RobotStudio 中的模型预处理 |
| `02-robodk-preprocessing.mkv` | 136 MB | RoboDK 中的模型与工作站预处理 |
| `03-robodk-single-arm-pick-and-place.mkv` | 115 MB | RoboDK 单机械臂抓取程序编写 |

视频存放在 Git LFS 中（三个文件都超过 GitHub 100 MB 单文件上限）。

**只想要代码和文档、不下载 413 MB 视频：**

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone <repository-url>
```

之后按需单独拉取某一节：

```bash
git lfs pull --include="tutorials/videos/01-*.mkv"
```

视频是 MKV 格式，GitHub 网页无法直接播放，请用 VLC / PotPlayer / mpv 打开。

## projects/library-storage/ — 图书馆收纳项目

`library-storage-project.rdk`（35.85 MB）是用 RoboDK 交互式搭建的完整工作站，
直接用 RoboDK 打开即可（`File` → `Open`）。

详见 [projects/library-storage/README.md](projects/library-storage/README.md)。

## 环境

- RoboDK 5.6.5（录制与建模所用版本）

## 许可

MIT，见 [LICENSE](LICENSE)。
