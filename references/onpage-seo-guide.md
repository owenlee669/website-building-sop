# On-Page SEO 优化指南

## 什么是 On-Page SEO

On-Page SEO = 页面内部的优化，包括内容、HTML标签、网站结构等。

与 Off-Page SEO（外链）相对，On-Page SEO 是你能完全控制的优化。

## TDH 优化（核心）

### Title（标题）

**最佳实践**：
- 长度：50-60字符
- 格式：主关键词 + 修饰词
- 示例：`Free Online Calculator | Quick & Accurate Results`

**避免**：
- 标题堆砌关键词
- 所有页面标题相同
- 标题过长被截断

### Description（描述）

**最佳实践**：
- 长度：150-160字符
- 包含：主关键词 + 行动号召
- 示例：`Use our free online calculator for quick and accurate calculations. No signup required. Try it now!`

**注意**：Description不直接影响排名，但影响点击率

### Headings（标题层级）

**结构**：
```html
<h1>主标题（包含主关键词）</h1>
<h2>二级标题（包含相关词）</h2>
  <h3>三级标题</h3>
<h2>另一个二级标题</h2>
```

**规则**：
- 每页只有1个H1
- H2-H3可以多个
- 层级不要跳（H1直接到H3）

## 内容优化

### 内容长度

| 页面类型 | 建议字数 | 说明 |
|----------|----------|------|
| 首页 | 1000-2000字 | 全面介绍网站 |
| 分类页 | 500-1000字 | 介绍该分类 |
| 内容页 | 800-2000字 | 详细解答问题 |
| 工具页 | 300-500字 | 工具说明+使用指南 |

### 关键词密度

**自然分布原则**：
- 不要刻意计算密度
- 在关键位置出现即可
- 使用同义词和LSI关键词

**关键位置**：
1. Title
2. H1
3. 首段前100字
4. 中间段落
5. 结尾段落

### LSI 关键词（潜在语义索引）

**什么是LSI关键词**：
与主关键词相关的词，帮助Google理解页面主题。

**示例**：
- 主词：online calculator
- LSI词：math calculator, scientific calculator, percentage calculator

**找LSI词方法**：
1. Google搜索主词，看「相关搜索」
2. 用LSIGraph.com
3. 看排名靠前的页面用了哪些相关词

## 技术优化

### URL 结构

**最佳实践**：
- 短而描述性
- 包含关键词
- 使用连字符（-）分隔
- 全小写

**示例**：
```
✅ /online-calculator
✅ /tools/percentage-calculator
❌ /page.php?id=123
❌ /OnlineCalculator
```

### 图片优化

**Alt标签**：
- 描述图片内容
- 包含关键词（自然）
- 示例：`alt="Free online percentage calculator interface"`

**文件名**：
- 描述性文件名
- 使用连字符
- 示例：`online-calculator-screenshot.jpg`

**压缩**：
- 使用WebP格式
- 图片大小<100KB
- 使用懒加载

### 内部链接

**作用**：
- 传递页面权重
- 帮助Google爬虫发现页面
- 提升用户体验

**策略**：
- 每页至少3-5个内部链接
- 从高权重页面链接到新页面
- 使用描述性锚文本

**示例**：
```html
<p>Try our <a href="/percentage-calculator">percentage calculator</a> for quick calculations.</p>
```

### Schema Markup（结构化数据）

**常用类型**：
- FAQPage - FAQ富媒体摘要
- HowTo - 步骤指南
- Article - 文章
- Product - 产品
- Review - 评论

**FAQ示例**：
```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "name": "Is this calculator free?",
    "acceptedAnswer": {
      "@type": "Answer",
      "text": "Yes, our calculator is completely free to use."
    }
  }]
}
```

## 页面速度优化

### 核心指标（Core Web Vitals）

| 指标 | 目标 | 说明 |
|------|------|------|
| LCP | <2.5s | 最大内容绘制 |
| FID | <100ms | 首次输入延迟 |
| CLS | <0.1 | 累积布局偏移 |

### 优化方法

1. **图片优化**
   - 使用WebP格式
   - 响应式图片
   - 懒加载

2. **代码优化**
   - 压缩CSS/JS
   - 移除未使用的代码
   - 延迟加载非关键JS

3. **服务器优化**
   - 使用CDN
   - 启用浏览器缓存
   - 使用HTTP/2

## 移动端优化

### 响应式设计

- 使用viewport meta标签
- 媒体查询适配不同屏幕
- 触摸友好的按钮大小

### 移动端特有优化

- 字体大小至少16px
- 点击目标至少48x48px
- 避免使用Flash
- 测试真实移动设备

## 优化检查清单

### 发布前检查

- [ ] Title 50-60字符，包含关键词
- [ ] Description 150-160字符，有行动号召
- [ ] 只有1个H1，包含关键词
- [ ] H2-H3层级正确
- [ ] URL简洁，包含关键词
- [ ] 图片有Alt标签
- [ ] 至少3个内部链接
- [ ] 内容长度达标
- [ ] 页面加载<3秒
- [ ] 移动端显示正常

### 发布后监控

- [ ] GSC中无错误
- [ ] 页面被收录
- [ ] Core Web Vitals达标
- [ ] 移动端可用性无问题

## 竞品分析方法

1. **找到排名前五的页面**
2. **分析他们的Title/Description**
3. **统计内容长度**
4. **查看Heading结构**
5. **检查Schema标记**
6. **测试页面速度**
7. **记录可学习的点**

**目标**：达到或超越竞品的标准
