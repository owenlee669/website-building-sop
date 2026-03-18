---
name: website-building-sop-quick-start
description: 哥飞社群快速上站 SOP。针对"2小时找词，半小时上站"的快速建站流程，3小时内完成从找词到上线的完整流程，适合抢占新词先机。
triggers:
  - 快速上站
  - 3小时上站
  - 紧急上站
  - 新词抢占
  - 快速建站
  - 半小时上站
---

# 快速上站 SOP

> **当天发现需求，当天上线。**

本 SOP 针对"2小时找词，半小时上站"的快速建站流程，帮助你在 3 小时内完成从找词到上线的完整流程，抢占新词先机。

---

## 核心理念

### 为什么要快？

**AI时代，先发优势巨大**
- 新词出现，谁先上线谁占坑
- 老站还没反应过来，你已经排名
- 速度就是竞争力

**新词新站策略**
- 新词竞争少，新站有机会"上线即排名"
- 拖延一天，可能错过最佳时机
- 快速验证，快速迭代

### 时间分配

```
找词：2小时
上站：30分钟
推广：30分钟
总计：3小时
```

**如果上站速度慢，说明经验不够，应放宽找词时间预期**

---

## 3小时上站完整流程

### 阶段一：找词（2小时）

#### 第1步：发现新词（30分钟）

**渠道优先级**：
1. **Google Trends**（5分钟）
   - 输入词根（ai, calculator, generator）
   - 查看「相关查询」→「上升」
   - 记录"Breakout"关键词

2. **Reddit/Twitter**（10分钟）
   - 浏览相关subreddit
   - 查看 trending topics
   - 关注行业KOL动态

3. **AI导航站**（10分钟）
   - Toolify.ai
   - theresanaiforthat.com
   - 查看最新收录的工具

4. **Vercel子域名**（5分钟）
   ```
   site:vercel.app "你的行业关键词"
   ```

**输出**：3-5个候选新词

---

#### 第2步：快速验证（30分钟）

**对每个候选词，快速检查**：

| 检查项 | 标准 | 工具 |
|--------|------|------|
| KD | < 30 | Semrush/Ahrefs |
| 搜索量 | > 100/月 | Semrush |
| intitle | < 1000 | Google搜索 |
| 趋势 | 上升或稳定 | Google Trends |
| 前10名 | 内页>5个 | Google搜索 |

**快速决策**：
- 满足4条以上 → 可以做
- 满足3条 → 考虑做
- 满足<3条 → 放弃

**输出**：1-2个确定要做的词

---

#### 第3步：需求理解（30分钟）

**搜索目标关键词，分析前3名**：
1. 他们提供什么功能/内容？
2. 用户真正想要什么？
3. 有什么可以改进的？
4. 差异化角度在哪里？

**确定网站类型**：
- 工具站 → 需要开发功能
- 内容站 → 需要撰写内容
- 混合站 → 工具+内容

**输出**：网站功能清单、内容大纲

---

#### 第4步：准备资料（30分钟）

**使用 Perplexity AI 收集资料**：

**提示词模板**：
```
请帮我收集关于"[关键词]"的详细信息：
1. 这个关键词是什么意思？
2. 用户搜索这个词是为了解决什么问题？
3. 现有的解决方案有哪些？
4. 用户对这个功能有什么具体需求？

请只收集整理原始资料，不要总结。
```

**输出**：原始资料文档

---

### 阶段二：上站（30分钟）

#### 第5步：代码生成（15分钟）

**使用 Claude 3.5 或 GPT-4o 生成代码**：

**第一步：设计结构**（5分钟）
```
提示词：
请基于以下资料，设计一个符合SEO最佳实践的Headings（H1-H6）结构：

关键词：[你的关键词]
网站类型：[工具站/内容站]
目标：提供[功能/内容]

资料：
[粘贴Perplexity收集的资料]

要求：
1. H1包含主关键词
2. H2-H6覆盖长尾词
3. 结构清晰，层级合理
4. 适合[工具站/内容站]类型
```

**第二步：生成代码**（10分钟）
```
提示词：
请根据以下已批准的Headings结构，生成完整的HTML、CSS、JavaScript代码：

[粘贴Headings结构]

要求：
1. 使用现代前端技术（HTML5 + CSS3 + Vanilla JS）
2. 响应式设计，移动端友好
3. 页面加载速度快（优化图片、最小化CSS/JS）
4. 包含完整的TDH（Title、Description、Headings）
5. 包含基本的SEO标签（canonical、og标签等）
6. 代码简洁，易于部署

输出：
1. 完整的HTML文件
2. 内联的CSS样式
3. 内联的JavaScript代码
```

**输出**：完整代码文件

---

#### 第6步：极速部署（10分钟）

**使用 Vercel 部署**：

1. **创建GitHub仓库**（2分钟）
   ```bash
   # 在GitHub上创建新仓库
   # 仓库名：你的关键词（如：ai-image-generator）
   ```

2. **推送代码**（3分钟）
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/你的用户名/仓库名.git
   git push -u origin main
   ```

3. **Vercel部署**（5分钟）
   - 登录 vercel.com
   - 点击 "Add New Project"
   - 选择GitHub仓库
   - 点击 "Deploy"
   - 等待部署完成（约1-2分钟）

**输出**：网站已上线，获得Vercel子域名

---

#### 第7步：域名绑定（5分钟）

**购买域名**（如果还没有）：
- Namecheap / Cloudflare Registrar
- 优先关键词域名（Exact Match Domain）
- 如：aiimagegenerator.com

**绑定域名**：
1. 在Vercel项目设置中添加自定义域名
2. 在域名注册商添加DNS记录
3. 等待DNS生效（几分钟到几小时）

**输出**：网站绑定自定义域名

---

### 阶段三：推广（30分钟）

#### 第8步：提交收录（10分钟）

1. **Google Search Console**（5分钟）
   - 添加属性（域名或URL前缀）
   - 验证域名所有权
   - 提交sitemap.xml

2. **索引请求**（5分钟）
   - 在GSC中请求索引首页
   - 提交几个重要内页

---

#### 第9步：冷启动推广（20分钟）

**高权重平台引蜘蛛**：

1. **V2EX**（5分钟）
   - 发布介绍帖
   - 标题：「做了个[关键词]工具，欢迎试用」
   - 内容：简单介绍 + 链接

2. **Reddit**（5分钟）
   - 找到相关subreddit
   - 发布软推广帖
   - 讲故事，不要硬广

3. **Twitter/X**（5分钟）
   - 发推文介绍
   - 使用相关hashtag
   - @相关账号

4. **Product Hunt**（5分钟）
   - 准备产品信息
   - 提交产品（可选，如果时间允许）

**输出**：网站获得首批外链和流量

---

## 快速上站检查清单

### 找词阶段（2小时）
- [ ] 发现3-5个候选新词
- [ ] 快速验证（KD<30, intitle<1000）
- [ ] 确定1-2个要做的词
- [ ] 分析前3名竞品
- [ ] 用Perplexity收集资料

### 上站阶段（30分钟）
- [ ] 用AI设计Headings结构
- [ ] 用AI生成完整代码
- [ ] 创建GitHub仓库
- [ ] 推送到GitHub
- [ ] Vercel自动部署
- [ ] 绑定自定义域名（可选）

### 推广阶段（30分钟）
- [ ] 提交Google Search Console
- [ ] 提交sitemap.xml
- [ ] 请求索引首页
- [ ] V2EX发布介绍
- [ ] Reddit发布介绍
- [ ] Twitter发布介绍

---

## 快速上站模板

### 工具站模板结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[关键词] | Free Online Tool</title>
    <meta name="description" content="Free [关键词] tool. [价值主张]. No signup required. Try it now!">
    <!-- SEO标签 -->
    <link rel="canonical" href="https://yourdomain.com/">
    <!-- Open Graph -->
    <style>
        /* 内联CSS */
    </style>
</head>
<body>
    <header>
        <h1>[关键词]</h1>
        <p>简短描述</p>
    </header>
    
    <main>
        <!-- 工具区域 -->
        <section id="tool">
            <input type="text" placeholder="输入...">
            <button>生成/计算</button>
            <div id="result"></div>
        </section>
        
        <!-- 说明区域 -->
        <section>
            <h2>What is [关键词]?</h2>
            <p>解释...</p>
            
            <h2>How to use</h2>
            <ol>
                <li>步骤1</li>
                <li>步骤2</li>
                <li>步骤3</li>
            </ol>
            
            <h2>FAQ</h2>
            <details>
                <summary>Is this tool free?</summary>
                <p>Yes, completely free.</p>
            </details>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2024 Your Site</p>
    </footer>
    
    <script>
        // 内联JS
    </script>
</body>
</html>
```

### 内容站模板结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- 同上 -->
</head>
<body>
    <header>
        <h1>[关键词] - Complete Guide</h1>
    </header>
    
    <main>
        <article>
            <h2>Introduction</h2>
            <p>介绍...</p>
            
            <h2>What is [关键词]</h2>
            <p>详细解释...</p>
            
            <h2>How to [关键词]</h2>
            <p>步骤...</p>
            
            <h2>Benefits of [关键词]</h2>
            <ul>
                <li>好处1</li>
                <li>好处2</li>
            </ul>
            
            <h2>FAQ</h2>
            <!-- FAQ内容 -->
        </article>
    </main>
</body>
</html>
```

---

## 常见问题

### Q1: 3小时真的够吗？
**A**: 
- 新手可能需要更长时间（5-6小时）
- 有经验后，3小时足够
- 关键是不要追求完美，先上线

### Q2: 代码质量会不会太差？
**A**:
- 先用AI生成，快速上线
- 后期再优化代码
- 功能完整 > 代码完美

### Q3: 没有自定义域名可以吗？
**A**:
- 可以先用Vercel子域名
- 但建议尽快绑定自定义域名
- 关键词域名有SEO优势

### Q4: 上线后还要做什么？
**A**:
- 监控收录情况
- 持续加页面
- 建设外链
- 优化内容

### Q5: 什么时候可以变现？
**A**:
- 有稳定流量后（日UV>100）
- 申请Google AdSense
- 或推出Pro版本

---

## 加速技巧

### 1. 建立个人模板库
- 保存常用的HTML/CSS/JS代码
- 复用，不要重复造轮子
- 每次上站速度会越来越快

### 2. 使用ShipAny等工具
- ShipAny（idoubi开发）
- 快速生成网站模板
- 适合快速验证

### 3. 外包低价值任务
- 设计可以外包
- 内容可以外包
- 专注于核心功能

### 4. 批量操作
- 一次找10个词
- 批量生成代码
- 批量部署

---

## 快速上站 vs 精品站

| 维度 | 快速上站 | 精品站 |
|------|----------|--------|
| 时间 | 3小时 | 1-2周 |
| 代码质量 | 够用就行 | 优化完善 |
| 设计 | 简洁 | 精美 |
| 功能 | 核心功能 | 完整功能 |
| 内容 | 基础内容 | 深度内容 |
| 适用场景 | 新词抢占 | 长期运营 |
| 后期工作 | 持续优化 | 维护更新 |

**建议**：
- 新词 → 快速上站，占坑
- 验证有潜力 → 升级为精品站
- 长期运营 → 持续优化

---

## 关联资源

- 主 SOP 文档：`../SKILL.md`
- 找词指南：`../references/keyword-research-guide.md`
- 外链指南：`../references/backlink-building-guide.md`
- On-Page 指南：`../references/onpage-seo-guide.md`
- 检查清单：`../assets/checklist-template.md`
- 成功案例：`../experiences/success-cases.md`

---

*本快速上站 SOP 基于哥飞社群实战经验整理，建议结合实际情况灵活应用。*
