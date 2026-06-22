# 古代埃及首饰库

一个简约优雅的古代埃及首饰文物展示网站。

## 功能特性

✨ **简约设计** - 清爽的界面，专注于展示文物  
🔍 **强大搜索** - 按名称、朝代、材质、来源快速查找  
📸 **图片展示** - 支持多张图片，点击查看详情  
📱 **响应式设计** - 完美适配电脑、平板、手机  
🚀 **零费用部署** - 使用 GitHub Pages 免费托管  

## 🚀 快速开始

### 第1步：启用 GitHub Pages

1. 进入仓库设置：**Settings** → **Pages**
2. 选择 **Deploy from a branch**
3. 选择分支：**Branch: main**, **/(root)**
4. 点击 **Save**
5. 等待 1-2 分钟，网站就会自动生成！

**您的网站链接：** `https://694827782-max.github.io/ancient-Egyptian-jewelry/`

### 第2步：准备数据文件

创建或编辑 `data.json` 文件，格式如下：

```json
[
    {
        "id": 1,
        "name": "文物名称",
        "dynasty": "朝代",
        "material": "材质",
        "craft": "工艺",
        "source": "来源",
        "description": "描述信息",
        "images": [
            "图片网址1",
            "图片网址2"
        ]
    }
]
```

### 第3步：数据字段说明

| 字段 | 说明 | 必需 | 示例 |
|------|------|------|------|
| id | 唯一标识号 | ✅ | 1 |
| name | 文物名称 | ✅ | "黄金项链" |
| dynasty | 朝代/年代 | ✅ | "新王朝" |
| material | 材质 | ✅ | "黄金" |
| craft | 工艺 | ✅ | "锻造、镶嵌" |
| source | 来源/博物馆 | ✅ | "埃及博物馆" |
| description | 详细描述 | ❌ | "这是一条精美的..." |
| images | 图片网址数组 | ❌ | ["url1", "url2"] |

## 📝 数据编辑方法

### 方法A：在线编辑（推荐新手）

1. 打开您的仓库首页
2. 找到 `data.json` 文件，点击它
3. 点击右上角的 **编辑按钮**（铅笔图标）
4. 修改内容
5. 滚到底部，点击 **Commit changes**
6. 点击 **Commit**

网站会在 1-2 分钟内自动更新！

### 方法B：上传文件（推荐大数据量）

1. 在仓库首页，点击 **Add file** → **Upload files**
2. 拖拽或选择您的 `data.json` 文件
3. 点击 **Commit changes**

## 🖼️ 图片上传指南

### 推荐方案1：用 GitHub 仓库存储图片（最简单）

1. 在仓库中创建 **images** 文件夹：
   - 点击 **Add file** → **Create new file**
   - 输入 `images/.gitkeep`
   - 点击 **Commit**

2. 上传图片到 images 文件夹：
   - 点击 **images** 文件夹
   - 点击 **Add file** → **Upload files**
   - 选择您的图片文件
   - 点击 **Commit changes**

3. 在 `data.json` 中引用图片：
   ```json
   "images": [
       "https://raw.githubusercontent.com/694827782-max/ancient-Egyptian-jewelry/main/images/necklace1.jpg"
   ]
   ```

### 推荐方案2：用免费图片托管服务

- **Imgur** (https://imgur.com) - 无需注册，直接上传
- **Smiling Tree** (https://www.smiling.tree) - 简单易用
- **Catbox** (https://catbox.moe) - 永久存储

上传后直接复制公开链接到 `data.json` 中的 `images` 数组。

## 📊 完整数据示例

```json
[
    {
        "id": 1,
        "name": "黄金镶青金石项链",
        "dynasty": "新王朝",
        "material": "黄金、青金石",
        "craft": "锻造、镶嵌、雕刻",
        "source": "埃及开罗博物馆",
        "description": "这条项链展示了古埃及工匠的精妙手艺。黄金部分采用精细的锻造工艺，青金石镶嵌在顶部，代表了天空和永恒。整件作品长约45厘米，重量约120克。项链采用链式设计，每个环节都经过精心打磨。",
        "images": [
            "https://raw.githubusercontent.com/694827782-max/ancient-Egyptian-jewelry/main/images/necklace1.jpg",
            "https://raw.githubusercontent.com/694827782-max/ancient-Egyptian-jewelry/main/images/necklace1-detail.jpg",
            "https://raw.githubusercontent.com/694827782-max/ancient-Egyptian-jewelry/main/images/necklace1-back.jpg"
        ]
    },
    {
        "id": 2,
        "name": "象牙及琥珀手镯",
        "dynasty": "中王朝",
        "material": "象牙、琥珀",
        "craft": "雕刻、抛光、镶嵌",
        "source": "大英博物馆",
        "description": "由象牙和琥珀组成的优雅手镯。表面雕刻有复杂的几何图案和莲花纹样，代表了埃及人对自然的崇拜。琥珀部分经过精心抛光，呈现出温暖的金色光泽。",
        "images": [
            "https://raw.githubusercontent.com/694827782-max/ancient-Egyptian-jewelry/main/images/bracelet1.jpg"
        ]
    }
]
```

## ❓ 常见问题

**Q: 网站多久能看到更新？**

A: 通常 1-2 分钟。如果很久没看到，请：
- 刷新浏览器（Ctrl+F5 或 Cmd+Shift+R）
- 清除浏览器缓存

**Q: 最多能上传多少件文物？**

A: GitHub 免费账户单个仓库限额是 1GB。对于 JSON 数据和图片来说，足够容纳上千件文物。

**Q: 图片大小有限制吗？**

A: 建议每张图片不超过 2MB，这样能保证网站加载速度。

**Q: 能在手机上编辑数据吗？**

A: 可以！在手机浏览器上登录 GitHub，编辑方式完全相同。

**Q: 如何删除或编辑某件文物？**

A: 打开 `data.json`，找到对应的文物对象，修改或删除它，然后提交更改。

**Q: 能改变网站的样式吗？**

A: 可以的，但需要编辑 `index.html` 文件中的 CSS 部分。建议先掌握基本操作后再尝试。

## 🔧 技术栈

- **前端**: 原生 HTML5 + CSS3 + JavaScript（无依赖）
- **数据格式**: JSON
- **部署平台**: GitHub Pages
- **成本**: 完全免费 🎉

## 📚 数据转换工具（可选）

如果您有 Excel 文件需要转换成 JSON 格式：

1. **在线转换工具**：
   - https://www.convertcsv.com/csv-to-json.htm
   - https://csvjson.com/

2. **操作步骤**：
   - 在 Excel 中保存为 CSV 格式
   - 上传到转换工具
   - 获取转换后的 JSON
   - 复制到 `data.json`

## 💡 建议

- 定期备份您的数据文件（可以下载 `data.json`）
- 为重要的更新添加有意义的 commit 信息
- 如果有大量数据，考虑分多次上传，每次验证是否正确

## 📞 获得帮助

如有问题，可以：
1. 检查 `data.json` 的 JSON 格式是否正确
2. 确保图片链接可以直接访问
3. 查看浏览器的开发者控制台（F12）是否有错误信息

---

**祝您使用愉快！🏺✨**
