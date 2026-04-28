# Sokoban - Fantasy Jelly Factory — App Store 发布清单

## 项目信息

| 字段 | 值 |
|------|-----|
| App 名称 | Sokoban - Fantasy Jelly Factory |
| Bundle ID | `com.rosewood.sokoban.game` |
| 版本号 | `1.0.0` |
| 构建号 | `1` |
| 版权 | `© 2026 888ios` |

---

## 1. Archive 构建

### 检查清单
- [ ] `productName` = `Sokoban`（project.pbxproj）
- [ ] `PRODUCT_BUNDLE_IDENTIFIER` = `com.rosewood.sokoban.game`
- [ ] `CFBundleDisplayName` = `Sokoban`（Info.plist）
- [ ] App Icon 无 Alpha 通道（RGB 模式，非 RGBA）
- [ ] `ITSAppUsesNonExemptEncryption` = false（Info.plist）

### 构建命令
```bash
cd /path/to/project
xcodebuild -project Sokoban.xcodeproj \
  -scheme Sokoban \
  -configuration Release \
  clean archive \
  -archivePath build/Sokoban.xcarchive
```

### 上传方式
**Transporter（推荐）**
1. Mac App Store 下载 [Transporter](https://apps.apple.com/us/app/transporter/id1450874784)
2. 打开后拖入 `.xcarchive` 文件
3. 点击 Deliver

---

## 2. App Store Connect 填写规范

### 基本信息

| 字段 | 填写内容 |
|------|---------|
| App 名称 | `Sokoban - Fantasy Jelly Factory` |
| 副标题 | `Push boxes, solve puzzles, collect stars` |
| 主语言 | `Chinese (Simplified)` |
| Bundle ID | `com.rosewood.sokoban.game` |
| 版本号 | `1.0.0` |
| 隐私政策 URL | （上线后填入，见 privacy.html） |

### 关键词（100字符限制）
```
sokoban,puzzle,push,jelly,box,logic,brain,casual,sliding,strategy,factory,stars
```
> 注意：关键词之间用逗号分隔，不加空格，总长不超过100字符。（94字符）

### 描述（4000字符）
```
Sokoban - Fantasy Jelly Factory is a classic push-box puzzle game set in a whimsical jelly factory. Guide your worker through challenging levels, push crates and boxes into position, and collect stars to unlock new stages!

**How to Play:**
• Tap or swipe to move your character in 4 directions
• Push boxes and crates onto target spots to complete each level
• Collect all 3 stars in each level for the perfect score
• Use the undo button to reverse mistakes
• Unlock new levels as you progress

**Features:**
• Classic Sokoban puzzle gameplay with a charming jelly factory theme
• Multiple levels with increasing difficulty
• 3-star rating system per level
• Undo moves to correct mistakes
• Beautiful, colorful art style
• Play completely offline — no internet required
• No ads, no in-app purchases, no distractions
```

### 版权
```
© 2026 888ios
```

### 审核备注
```
This is a single-player puzzle game with no login, no ads, no in-app purchases, and no data collection. Tap directional buttons to move the character and push boxes onto target spots. Use the undo button to reverse moves. Complete levels to earn stars.
```

---

## 3. 加密文稿

| 字段 | 选择 |
|------|------|
| 你的 App 是否使用加密？ | **否** |

> 纯离线单机游戏，无网络连接。

---

## 4. 截图规格

### iPhone 6.5寸（1284×2778，必填）

| 序号 | 文件名 | 内容 |
|------|--------|------|
| 01 | `01_menu.png` | 主菜单 — 标题 "SOKOBAN" + "Fantasy Jelly Factory" + START GAME / SELECT LEVEL / SETTINGS |
| 02 | `02_levels.png` | 选关界面 — 关卡 1-12 网格布局 + 星级进度 |
| 03 | `03_gameplay.png` | 游戏进行中 — Level 10 + 角色推箱子 + 棋盘布局 |
| 04 | `04_complete.png` | Level Complete 弹窗 — 3星评价 + NEXT LEVEL / REPLAY / MAIN MENU |

### iPhone 5.5寸（1242×2208，必填）
同上 4 张截图（已缩放至 1242×2208）

所有截图已处理并保存在：
- `screenshots_65/` — iPhone 6.5寸
- `screenshots_55/` — iPhone 5.5寸

---

## 5. 隐私政策

见 `privacy.html`，声明要点：
- 纯离线单机游戏
- 不收集、不传输任何个人信息
- 无网络连接功能
- 无第三方 SDK
- 无广告、无内购

---

## 6. 提交流程

1. 登录 [App Store Connect](https://appstoreconnect.apple.com)
2. 我的 App → 新建 App（名称 `Sokoban - Fantasy Jelly Factory`，Bundle ID `com.rosewood.sokoban.game`）
3. 填写上述所有字段
4. 上传 `.xcarchive`（通过 Transporter）
5. 上传截图（6.5寸 4张 + 5.5寸 4张）
6. 完成加密文稿（选"否"）
7. 提交审核

---

## 快速复制汇总

| 字段 | 内容 |
|------|------|
| **App 名称** | `Sokoban - Fantasy Jelly Factory` |
| **副标题** | `Push boxes, solve puzzles, collect stars` |
| **Bundle ID** | `com.rosewood.sokoban.game` |
| **版本号** | `1.0.0` |
| **关键词** | `sokoban,puzzle,push,jelly,box,logic,brain,casual,sliding,strategy,factory,stars` |
| **加密** | 否 |
| **截图** | 4张（主菜单/选关/游戏中/完成弹窗）× 2种尺寸 |
