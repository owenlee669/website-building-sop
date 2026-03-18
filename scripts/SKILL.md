---
name: website-building-sop-scripts
description: 哥飞社群建站自动化脚本。收录收录监控、排名追踪、外链检查等自动化脚本，帮助提高效率，减少重复劳动。
triggers:
  - 自动化脚本
  - 监控脚本
  - 收录监控
  - 排名追踪
  - 批量操作
---

# 建站自动化脚本

> **自动化是效率的终极武器。**

本文件夹收录建站所需的各类自动化脚本。

---

## 脚本分类

| 类别 | 用途 | 文件 |
|------|------|------|
| **收录监控** | 监控网站收录情况 | `index-monitor.py` |
| **排名追踪** | 追踪关键词排名 | `rank-tracker.py` |
| **外链检查** | 检查外链状态 | `backlink-checker.py` |
| **内容生成** | 批量生成内容 | `content-generator.py` |
| **数据导出** | 导出分析数据 | `data-exporter.py` |

---

## 使用说明

### 环境要求
- Python 3.8+
- 依赖包见各脚本文件

### 安装依赖
```bash
pip install -r requirements.txt
```

### 配置API密钥
- 复制 `.env.example` 为 `.env`
- 填入你的API密钥
- 不要提交 `.env` 到Git

---

## 脚本列表

### 收录监控脚本
**功能**：
- 监控网站收录数量
- 检查新页面收录情况
- 发送邮件/钉钉通知

**使用方法**：
```bash
python index-monitor.py --domain yourdomain.com
```

---

### 排名追踪脚本
**功能**：
- 追踪关键词排名变化
- 生成排名报告
- 监控竞品排名

**使用方法**：
```bash
python rank-tracker.py --keywords "keyword1,keyword2"
```

---

### 外链检查脚本
**功能**：
- 检查外链是否有效
- 监控外链状态
- 发现新外链机会

**使用方法**：
```bash
python backlink-checker.py --domain yourdomain.com
```

---

## 自动化运行

### 使用Cron定时运行
```bash
# 每天9点运行收录监控
0 9 * * * cd /path/to/scripts && python index-monitor.py

# 每周一运行排名追踪
0 9 * * 1 cd /path/to/scripts && python rank-tracker.py
```

### 使用GitHub Actions
- 免费定时运行
- 自动推送结果
- 详见 `.github/workflows/` 文件夹

---

## 贡献脚本

如果你有实用的脚本想要分享：

1. 按照模板格式编写
2. 添加使用说明
3. 提交PR

**脚本模板**：
```python
#!/usr/bin/env python3
"""
脚本名称：xxx
功能描述：xxx
作者：xxx
日期：xxx
"""

import requests
import json

def main():
    # 主逻辑
    pass

if __name__ == "__main__":
    main()
```

---

## 注意事项

### 1. API限制
- 注意API调用频率限制
- 添加适当的延迟
- 使用缓存避免重复请求

### 2. 数据安全
- 不要硬编码API密钥
- 使用环境变量
- 不要提交敏感信息

### 3. 错误处理
- 添加try-except
- 记录错误日志
- 失败时发送通知

---

## 关联资源

- 主 SOP 文档：`../SKILL.md`
- 工具清单：`../tools/SKILL.md`

---

*本脚本库基于哥飞社群成员分享整理，持续更新中。*
