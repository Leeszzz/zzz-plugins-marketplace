# Paper 学术论文工具套件

学术论文检索与批量文献总结工具，集成 Semantic Scholar MCP 服务。

## 功能概览

### `/paper:search` - 论文检索

使用 Semantic Scholar 检索学术论文，将结果记录到 Markdown 文件。

**用法**：
```bash
/paper:search 微电网能量管理 2020-2025
/paper:search hydrogen fuel cell optimization
```

**特性**：
- 中英文关键词自动转换
- 自动去重，避免重复记录
- 结果追加到 `paper/论文.md`

### `/paper:summarize` - 文献总结

批量处理本地学术文献，生成结构化总结。

**用法**：
```bash
# 简短模式（表格汇总）
/paper:summarize --mode brief ./papers/

# 详细模式（每篇单独报告）
/paper:summarize --mode detailed ./papers/*.pdf

# 启用在线信息补充
/paper:summarize --mode brief --enrich ./papers/
```

**支持格式**：PDF、Markdown、文本文件

## 安装要求

需要配置 Semantic Scholar MCP 服务器才能使用检索功能。

## 作者

Leeszzz

## 许可证

MIT
