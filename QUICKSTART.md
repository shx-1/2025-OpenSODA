# 快速开始指南

本指南帮助您快速查看和生成2025第三届OpenSODA大赛初赛PPT。

## 方式一：在线查看（最简单）

直接在GitHub上查看 [presentation.md](presentation.md) 文件，即可阅读所有演示内容。

## 方式二：本地预览（推荐）

### 前置要求
- 已安装 [Node.js](https://nodejs.org/) (v14或更高版本)

### 步骤

1. **克隆仓库**（如果还未克隆）
```bash
git clone <repository-url>
cd 2025-OpenSODA
```
或者直接进入已克隆的目录

2. **安装依赖**
```bash
npm install
```

3. **预览PPT**（在浏览器中实时预览）
```bash
npm run preview
```

4. **生成PDF文件**
```bash
npm run setup
npm run build:pdf
```
生成的PDF文件位于 `output/presentation.pdf`

5. **生成PowerPoint文件**
```bash
npm run setup
npm run build:pptx
```
生成的PPTX文件位于 `output/presentation.pptx`

6. **生成HTML文件**
```bash
npm run setup
npm run build:html
```
生成的HTML文件位于 `output/presentation.html`

7. **生成所有格式**
```bash
npm run setup
npm run build:all
```

## 方式三：使用VS Code（适合开发者）

### 步骤

1. **安装VS Code**
   下载并安装 [Visual Studio Code](https://code.visualstudio.com/)

2. **安装Marp扩展**
   - 打开VS Code
   - 按 `Ctrl+Shift+X`（Windows/Linux）或 `Cmd+Shift+X`（Mac）打开扩展面板
   - 搜索 "Marp for VS Code"
   - 点击安装

3. **打开项目**
```bash
code .
```

4. **查看PPT**
   - 打开 `presentation.md` 文件
   - 点击右上角的预览按钮（或按 `Ctrl+K V`）
   - 即可看到演示效果

5. **导出文件**
   - 在预览模式下，点击右上角的导出按钮
   - 选择要导出的格式（PDF、PPTX、HTML等）

## 方式四：全局安装Marp CLI

### 安装
```bash
npm install -g @marp-team/marp-cli
```

### 使用
```bash
# 预览
marp presentation.md --preview

# 生成PDF
marp presentation.md --pdf

# 生成PPTX
marp presentation.md --pptx

# 生成HTML
marp presentation.md --html
```

## 文件说明

- `presentation.md` - 演示文稿主文件（Markdown格式）
- `README.md` - 项目说明文档
- `GUIDE.md` - 详细参赛指南
- `QUICKSTART.md` - 本快速开始指南
- `package.json` - Node.js项目配置文件

## 演示文稿内容概览

本PPT包含以下内容：
1. 大赛简介
2. 赛事信息
3. 初赛安排
4. 初赛内容和赛道
5. 参赛要求
6. 评审标准
7. 奖项设置
8. 参赛流程
9. 技术支持
10. 注意事项
11. 联系方式
12. 资源链接

## 常见问题

### Q: 为什么使用Markdown而不是PowerPoint？
A: Markdown格式的演示文稿便于版本控制、协作编辑，且可以轻松转换为多种格式（PDF、PPTX、HTML等）。

### Q: 生成的PowerPoint能正常编辑吗？
A: 是的，生成的PPTX文件可以用Microsoft PowerPoint或其他兼容软件打开和编辑。

### Q: 可以自定义主题吗？
A: 可以，在 `presentation.md` 文件的头部修改 `theme` 参数，或创建自定义CSS主题。

### Q: 预览时无法显示？
A: 确保已正确安装Node.js和相关依赖，可以尝试重新运行 `npm install`。

## 需要帮助？

如有任何问题，请：
- 查看 [Marp官方文档](https://marp.app/)
- 在GitHub上提交Issue
- 联系大赛组委会：contact@opensoda.org

---

**祝您使用愉快！** 🎉
