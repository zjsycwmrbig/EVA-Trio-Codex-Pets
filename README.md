# EVA Trio Codex Pets

三只同批制作的 Q 版 EVA 角色 Codex 宠物：绫波丽-Q、真嗣-Q、明日香-Q。

这是非官方、粉丝制作的桌面宠物素材，不是《新世纪福音战士》官方项目。

| 预览 | 宠物 | 目录 | 稳定 ID |
| --- | --- | --- | --- |
| ![绫波丽-Q](previews/eva-rei-q.png) | 绫波丽-Q | `eva-rei-q/` | `pet_6ad7382f67b48191afc964ab25c49e56` |
| ![真嗣-Q](previews/eva-shinji-q.png) | 真嗣-Q | `eva-shinji-q/` | `pet_6ad7382b18248191897dc458b267e3fc` |
| ![明日香-Q](previews/eva-asuka-q.png) | 明日香-Q | `eva-asuka-q/` | `pet_6ad73826baf8819188eab744e227096a` |

## 安装

### macOS / Linux

```bash
git clone https://github.com/zjsycwmrbig/EVA-Trio-Codex-Pets.git
mkdir -p "$HOME/.codex/pets"
cp -R EVA-Trio-Codex-Pets/eva-rei-q \
      EVA-Trio-Codex-Pets/eva-shinji-q \
      EVA-Trio-Codex-Pets/eva-asuka-q \
      "$HOME/.codex/pets/"
```

### Windows PowerShell

```powershell
git clone https://github.com/zjsycwmrbig/EVA-Trio-Codex-Pets.git
$pets = Join-Path $HOME ".codex\pets"
New-Item -ItemType Directory -Force $pets | Out-Null
Copy-Item -Recurse -Force ".\EVA-Trio-Codex-Pets\eva-*" $pets
```

复制后重新打开 Codex 的宠物选择器即可看到三只宠物。

## 宠物包结构

每个目录都是一个完整、独立的 Codex 宠物包：

```text
eva-rei-q/
├── pet.json
└── spritesheet.webp
```

三张精灵图均为 v2 规格：

- 尺寸：`1536 x 2288`
- 单元格：`192 x 208`
- 网格：`8 x 11`
- 格式：透明 WebP

素材已通过 Codex Pets 的精灵图结构校验。

## English

This repository contains three fan-made, chibi-style custom pets for Codex:
Rei-Q, Shinji-Q, and Asuka-Q. Each directory is a self-contained pet package
with `pet.json` and a validated `1536 x 2288` transparent WebP sprite sheet.

Copy the three directories into `~/.codex/pets` on macOS/Linux or
`%USERPROFILE%\.codex\pets` on Windows, then reopen the Codex pet picker.

## 许可与声明

- 仓库中的文档和配置文件使用 [MIT License](LICENSE)。
- 创作者对粉丝绘制宠物的原创贡献按 [CC BY 4.0](LICENSE-ASSETS) 提供。
- 《新世纪福音战士》及相关角色、名称与设定的权利归其各自权利人所有。
- 本仓库不是官方发布，也不代表或获得权利人的认可。上述素材许可不授予任何第三方角色、商标或作品权利。详见 [NOTICE.md](NOTICE.md)。
