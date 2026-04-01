# Quartz 笔记博客

这是我的笔记博客，使用 [Quartz](https://quartz.jzhao.xyz/) 从 Obsidian 笔记自动生成。

## 🚀 快速开始

### 1. 链接到你的 Obsidian

Quartz 可以直接从你的 Obsidian 仓库读取笔记，自动同步：

```bash
# 在 quartz-blog 目录下，创建符号链接到你的 Obsidian content
# 注意：配置中已经忽略了私密内容，不会公开
cd /Users/luuli/Documents/personal-site/quartz-blog
ln -sf /Users/luuli/Documents/Obsidian/* content/
```

或者，如果你只想放公开的一部分笔记，可以手动复制公开笔记到 `content/` 目录。

### 当前配置已经自动忽略（不会公开）

- `private/` - 私密笔记
- `**/Templates*/**` - 模板目录
- `**/.obsidian*/**` - Obsidian 系统配置
- `**/01-Home*/**AI助手*` - AI 协作指南（不需要公开）
- `**/*Archive*` - 归档内容

### 2. 安装依赖

```bash
pnpm install
```

### 3. 本地预览

```bash
npx quartz build --serve
```

访问 http://localhost:8080 预览。

### 4. 配置修改

- 修改 `quartz.config.ts`：修改 `baseUrl` 为你的 GitHub Pages 地址
- 修改 `quartz.layout.ts`：修改 `footer` 中的返回主站链接

### 5. 部署到 GitHub Pages

1. 在 GitHub 创建仓库，命名为 `quartz-blog`
2. 修改配置文件中的链接
3. push 到 main 分支
4. 在 GitHub → Settings → Pages → Source → GitHub Actions
5. GitHub Actions 会自动构建部署

## 🔗 链接

- **主站（个人主页）**: [YOUR-GITHUB-USERNAME.github.io](https://YOUR-GITHUB-USERNAME.github.io)
- **这个博客**: [YOUR-GITHUB-USERNAME.github.io/quartz-blog](https://YOUR-GITHUB-USERNAME.github.io/quartz-blog)

---

> 基于 Quartz v4 构建 → https://quartz.jzhao.xyz/
