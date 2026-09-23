# astra-audio

Astra 语音音频归档仓库。共 **28,449** 个音频文件，合计 **1,246,192,948 字节（约 1.16 GiB）**。

## 目录结构

```
voice/
  <角色目录>/*.mp3      例：voice/abrams/abrams_attack_01.mp3
  _shared/              各角色共用音频
  _unreferenced/        未被引用的零散音频（含 7 个 .wav）
```

## 直链基址

| 用途 | 基址 |
| --- | --- |
| raw（GitHub 官方） | `https://raw.githubusercontent.com/41jebve/astra-audio/main/voice/` |
| jsDelivr（CDN） | `https://cdn.jsdelivr.net/gh/41jebve/astra-audio@main/voice/` |

拼接方式：`<基址><角色目录>/<文件名>`，例如
`https://raw.githubusercontent.com/41jebve/astra-audio/main/voice/abrams/abrams_attack_01.mp3`

## 关于 Git LFS

本仓库**故意不启用 Git LFS**。Git LFS 免费额度仅 1 GB，而本仓库音频总量约 1.16 GiB，一旦启用会直接超出额度。
所有音频均以普通 Git 对象直接提交，`.gitattributes` 中已将 `*.mp3` / `*.wav` 标记为二进制并显式关闭 `filter`。
