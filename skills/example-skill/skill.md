# 使用说明：example-skill

## 概览

example-skill 提供一个示例性的对外 API 适配层，展示如何描述 skill 的能力、认证方式、端点与使用范例。文档同时为自动化发布工具（如 skill-publish）提供必要的引用。

## 快速开始

使用 curl 示例：

```bash
# 查询示例
curl -H "Authorization: Bearer $TOKEN" "https://api.example.com/v1/query?prompt=hello"

# 执行动作示例
curl -X POST -H "Authorization: Bearer $TOKEN" -H "Content-Type: application/json" \
  -d '{"task":"do_something","params":{}}' \
  https://api.example.com/v1/action
