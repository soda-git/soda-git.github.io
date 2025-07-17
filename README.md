# Soda Code

这是一个用于 GitHub Pages 用户主页的项目仓库。

## 项目说明

本仓库主要用于托管静态网页文件，通过 GitHub Pages 服务提供在线访问。

## 使用方法

### 方案一：用户主页（一级域名访问）

1. **重要**：仓库名称必须是 `soda-git.github.io`
2. 将项目文件放在仓库根目录
3. 推送到 GitHub 仓库
4. GitHub Pages 会自动启用（无需手动配置）
5. 访问地址：`https://soda-git.github.io`

### 方案二：项目页面（临时方案）

如果遇到问题，可以先使用项目页面：

1. 创建任意名称的仓库（如 `my-website`）
2. 将项目文件放在仓库根目录
3. 推送到 GitHub 仓库
4. 在 Settings → Pages 中手动启用
5. 访问地址：`https://soda-git.github.io/my-website`

## 目录结构

```
soda-git.github.io/    # 仓库名必须是这个格式
├── README.md          # 项目说明
├── index.html         # 主页面
├── .nojekyll         # 禁用 Jekyll 处理
└── assets/           # 静态资源目录
    ├── css/          # 样式文件
    ├── js/           # JavaScript 文件
    └── images/       # 图片文件
```

## 部署说明

### GitHub Pages 部署步骤

1. **推送代码到 GitHub 仓库**
2. **启用 Pages 服务**：
   - 进入仓库的 Settings 页面
   - 滚动到 Pages 部分
   - 选择 Source 为 "Deploy from a branch"
   - 选择分支（通常是 `main`）和目录（通常是 `/root`）
3. **访问网站**：
   - **用户主页地址**：`https://soda-git.github.io`（一级域名，无需路径）
   - **项目页面地址**：`https://soda-git.github.io/<repository-name>/`（如果仓库名不是 soda-git.github.io）
   - 部署成功后会在 Pages 设置中显示访问地址

### 自定义域名配置

如果您想使用自己的域名（如 `yourdomain.com`）：

1. **创建 CNAME 文件**（已包含在项目中）
2. **配置 DNS 记录**：
   - **顶级域名**：添加 A 记录指向 GitHub Pages 的 IP
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - **www 子域名**：添加 CNAME 记录指向 `<username>.github.io`

3. **在 GitHub Pages 设置中配置自定义域名**
4. **等待 DNS 传播**（可能需要几小时）
5. **启用 HTTPS**（GitHub 会自动颁发 SSL 证书）

### 注意事项

- GitHub Pages 支持自定义域名
- 支持 HTTPS（自动 SSL 证书）
- 构建和部署通常需要几分钟时间
- DNS 传播可能需要 24-48 小时
- 可以在仓库的 Actions 标签页查看部署状态

## GitHub Pages 特性

- ✅ 免费托管静态网站
- ✅ 支持自定义域名
- ✅ 自动 HTTPS
- ✅ CDN 加速
- ✅ 与 Git 工作流完美集成

## 更新日志

- 2024-12-19: 从 Gitee Pages 迁移到 GitHub Pages
- 2024-12-19: 目录重命名为 soda-git 