# AI 辅助写页面规则

## 📋 项目概述
- **项目类型**: GitHub Pages 静态网站
- **主要功能**: 个人主页平台，包含旅游规划、技术博客、创意作品、实用工具等多个分类
- **设计风格**: 基于 `hulunbeier_travel_guide.html` 的专业设计风格
- **技术栈**: HTML, CSS, JavaScript (原生)
- **目标用户**: 中文用户，多元化内容需求
- **核心特色**: 集成高德地图导航、移动端优化、AI辅助写作

## 🎯 AI 辅助开发规则

### 1. 代码风格规范
- **语言**: 所有页面内容必须使用中文
- **命名**: 文件名使用下划线分隔，如 `beijing_trip_qrcode.html`
- **CSS**: 使用内联样式或内部样式表，避免外部CSS依赖
- **JavaScript**: 使用原生JavaScript，避免引入外部库

### 2. 页面结构规范
- **HTML5**: 使用 `<!DOCTYPE html>` 和语义化标签
- **响应式**: 所有页面必须支持移动设备
- **字符集**: 使用 `UTF-8` 编码
- **语言标记**: `<html lang="zh-CN">`

### 3. 设计风格指南
- **背景色**: 淡绿到淡蓝渐变 `linear-gradient(135deg, #e8f5e8 0%, #f0f8ff 100%)`
- **主色调**: 绿色到蓝色渐变 `linear-gradient(135deg, #4CAF50 0%, #2196F3 100%)`
- **文字颜色**: 深绿色 `#2c5530`，绿色 `#4CAF50`，蓝色 `#2196F3`
- **字体**: `'Microsoft YaHei', Arial, sans-serif`
- **布局**: 最大宽度1200px，居中对齐
- **卡片设计**: 白色背景，圆角15px，阴影效果
- **边框装饰**: 使用左边框或上边框突出重点
- **动画**: 悬停时上移和阴影增强效果

### 4. 功能要求
- **导航**: 页面间要有返回主页的链接
- **时间**: 显示最后更新时间
- **交互**: 卡片悬停效果和点击反馈
- **图片**: 如有图片，放在 `assets/images/` 目录
- **地图集成**: 支持高德地图导航功能（参考呼伦贝尔页面）
- **设备适配**: 自动检测移动端，优化APP调用体验
- **提示框**: 使用不同类型的提示框（info、warning、highlight）

### 5. 内容管理规范
- **页面标题**: 格式为 `页面名称 - Soda Code`
- **描述**: 每个页面都要有清晰的功能描述
- **链接**: 所有内部链接使用相对路径
- **更新**: 每次修改后更新时间戳

### 6. AI 协作指令
当用户请求AI辅助时，AI应该：

#### 6.1 创建新页面
- 询问页面功能和内容要求
- **严格遵循** `hulunbeier_travel_guide.html` 的设计风格
- 使用绿色到蓝色的渐变配色方案
- 确保响应式设计和移动端优化
- 添加返回主页链接
- 更新 `index.html` 中的链接

#### 6.2 修改现有页面
- 先读取现有文件内容
- 保持与 `hulunbeier_travel_guide.html` 风格一致
- 使用统一的配色方案和布局结构
- 只修改必要的部分
- 确保修改后的响应式效果

#### 6.3 添加新功能
- 功能可以涵盖旅游规划、技术博客、创意作品、实用工具等多个分类
- 使用原生JavaScript实现
- 考虑移动端用户体验
- 添加适当的用户反馈
- 根据功能类型选择合适的页面结构

#### 6.4 优化现有功能
- 分析现有代码结构
- 提供性能优化建议
- 改进用户界面
- 增强交互体验

#### 6.5 发布协助指导
- **发布提醒**: 完成修改后提醒用户推送即发布
- **质量检查**: 协助用户进行发布前检查
- **测试建议**: 建议用户在本地充分测试后再推送
- **风险提示**: 对于重大修改提醒用户注意备份
- **验证协助**: 推送后协助用户验证线上效果

### 7. 文件组织规范
```
soda-git/
├── .gitignore                       # Git忽略文件配置
├── .nojekyll                        # GitHub Pages配置文件
├── AI_ASSISTANT_RULES.md            # AI助手规则和项目规范
├── README.md                        # 项目说明文档
├── index.html                       # 🏠 主页
├── travel/                          # 🌍 旅游规划模块
│   ├── beijing_trip_qrcode.html     # 🏛️ 北京3日游行程页面
│   └── hulunbeier_travel_guide.html # 🏔️ 呼伦贝尔房车游行程页面
├── blog/                            # 💻 技术博客模块（预留）
├── tools/                           # 🛠️ 实用工具模块（预留）
├── creative/                        # 🎨 创意作品模块（预留）
└── assets/                          # 静态资源目录
    ├── css/                         # CSS样式文件（如需要）
    ├── js/                          # JavaScript脚本文件（如需要）
    └── images/                      # 图片资源
        └── hulunbeier_route_map.png # 呼伦贝尔路线图
```

#### 功能模块目录说明
- **travel/** - 旅游规划相关页面
- **blog/** - 技术博客相关页面（预留）
- **tools/** - 实用工具相关页面（预留）
- **creative/** - 创意作品相关页面（预留）

#### 核心页面文件
- **index.html** - 网站主页，展示所有功能模块
- **功能页面** - 按类型分目录组织，使用下划线分隔

#### 资源文件组织
- **assets/css/** - 存放CSS样式文件（目前使用内联样式）
- **assets/js/** - 存放JavaScript脚本文件（目前使用内联脚本）
- **assets/images/** - 存放图片资源文件

#### 配置文件
- **.gitignore** - Git版本控制忽略配置
- **.nojekyll** - 禁用GitHub Pages的Jekyll处理
- **AI_ASSISTANT_RULES.md** - AI助手工作规范和项目标准

### 8. 常用操作模板

#### 8.1 创建新页面模板
```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>页面名称 - Soda Code</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Microsoft YaHei', Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #e8f5e8 0%, #f0f8ff 100%);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .header {
            background: linear-gradient(135deg, #4CAF50 0%, #2196F3 100%);
            color: white;
            padding: 40px 20px;
            text-align: center;
            border-radius: 15px;
            margin-bottom: 30px;
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }
        
        .section {
            background: white;
            margin: 20px 0;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
            border-left: 5px solid #4CAF50;
        }
        
        .back-home {
            background: linear-gradient(135deg, #4CAF50 0%, #2196F3 100%);
            color: white;
            text-decoration: none;
            padding: 12px 25px;
            border-radius: 25px;
            font-weight: bold;
            display: inline-block;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>页面标题</h1>
            <p>页面描述</p>
        </div>
        
        <div class="section">
            <h2>内容标题</h2>
            <!-- 页面内容 -->
        </div>
        
        <a href="index.html" class="back-home">🏠 返回主页</a>
    </div>
</body>
</html>
```

#### 8.2 添加新功能到主页
1. 在相应的功能模块目录中创建新页面
2. 在 `index.html` 中添加相应的链接卡片
3. 确保新页面包含返回主页的链接（使用 `../index.html` 路径）
4. 确保链接路径正确（如：`travel/页面名.html`）

### 9. 测试检查清单
- [ ] 页面在桌面端正常显示
- [ ] 页面在移动端正常显示
- [ ] 所有链接都能正确跳转
- [ ] 中文显示正常
- [ ] 样式风格保持一致
- [ ] JavaScript功能正常
- [ ] 没有控制台错误

### 10. 发布流程与部署规范

#### 10.1 发布机制
- **直接发布**: 推送到GitHub远程仓库 = 立即发布到线上
- **无需构建**: 静态文件直接通过GitHub Pages服务
- **自动更新**: 推送后1-2分钟内生效
- **回滚方便**: 可通过git revert快速回滚

#### 10.2 发布前检查清单
- [ ] 页面在本地预览正常
- [ ] 所有链接可以正确跳转
- [ ] 移动端显示效果良好
- [ ] 中文字符显示正常
- [ ] JavaScript功能正常运行
- [ ] 图片资源路径正确
- [ ] 无控制台错误信息

#### 10.3 发布操作流程
1. **本地测试**: 在本地浏览器中全面测试
2. **提交代码**: `git add . && git commit -m "更新描述"`
3. **推送发布**: `git push origin master`
4. **等待生效**: 1-2分钟后访问线上地址验证
5. **功能验证**: 检查所有功能是否正常

#### 10.4 发布注意事项
- **谨慎推送**: 推送即发布，确保代码质量
- **备份重要**: 重大更新前可创建分支备份
- **渐进更新**: 建议小步快跑，避免大幅改动
- **及时验证**: 推送后立即验证线上效果

#### 10.5 Git操作指导
```bash
# 查看当前状态
git status

# 添加所有修改
git add .

# 提交修改（写清楚修改内容）
git commit -m "添加XX功能/修复XX问题/优化XX页面"

# 推送到远程（即发布）
git push origin master

# 查看推送历史
git log --oneline

# 紧急回滚（如果发布后发现问题）
git revert HEAD
git push origin master
```

#### 10.6 推荐的提交信息格式
- `feat: 添加厦门旅游规划页面`
- `fix: 修复移动端导航问题`
- `style: 优化首页卡片样式`
- `update: 更新呼伦贝尔行程信息`
- `docs: 更新AI规则文档`

## 🚀 快速开始命令

当需要AI辅助时，可以使用以下格式：

### 创建页面
- "帮我创建一个[页面名称]页面，功能是[具体功能描述]"
- "帮我创建一个技术博客页面，用来发布编程文章"
- "帮我创建一个实用工具页面，收录各种在线工具"

### 修改页面
- "帮我修改[页面名称]，需要[具体修改需求]"
- "帮我修改主页，在旅游规划中增加新的目的地"

### 添加功能
- "帮我在[页面名称]添加[功能描述]"
- "帮我在主页添加一个新的分类模块"

### 优化页面
- "帮我优化[页面名称]的[具体方面]"
- "帮我优化呼伦贝尔页面的移动端显示效果"

### 发布协助
- "帮我检查一下这个页面是否可以发布"
- "我准备推送到GitHub，帮我确认一下有没有遗漏"
- "刚推送了代码，帮我验证一下线上效果"
- "这是个重大更新，有什么需要注意的吗？"

---

**最后更新**: 2024年12月19日
**版本**: 2.2
**参考风格**: `hulunbeier_travel_guide.html`
**新增功能**: 按类型分目录组织、功能模块化结构、发布流程规范
**维护者**: AI Assistant & User 