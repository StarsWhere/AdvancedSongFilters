# AdvancedSongFilters

按范围、模式、难度和曲包筛选歌曲，支持排序和个人预设。

支持 Windows x64、Beat Saber **1.45.2_28848**，依赖环境包含本地移植的模组；其他依赖组合的兼容性需另行确认。

## 安装

从 [Releases](https://github.com/StarsWhere/AdvancedSongFilters/releases) 下载压缩包，关闭游戏后将包内目录合并到游戏根目录。所需依赖及版本见 [manifest](scripts/advanced_song_filters/AdvancedSongFilters.manifest.json)。 [LocalModUI](https://github.com/StarsWhere/LocalModUI) 需要单独安装。

## 构建

准备 PowerShell 7、.NET SDK 和已安装兼容依赖的游戏，在 PowerShell 中运行：

```powershell
git clone --recurse-submodules https://github.com/StarsWhere/AdvancedSongFilters
cd AdvancedSongFilters
pwsh -File scripts/build_release.ps1 -GameRoot 'C:\Games\Beat Saber'
```

临时文件位于 `.tmp/`，发布文件位于 `releases/`。

## 许可

[MIT](LICENSE)，第三方声明见 [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt)。
