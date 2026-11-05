# deepseek-browser-use-docs

[deepseek-browser-use](https://github.com/litongjava/deepseek-browser-use) 的文档站：面向 AI 智能体的有状态浏览器服务。

- 文档站：https://deepseek-browser-use.io.nexus/

## 本地开发

```bash
pnpm install
pnpm docs:dev
```

## 构建

```bash
pnpm docs:build
```

构建产物位于 `docs/.vitepress/dist`。

## 部署

推送到 `main` 分支后，Cloudflare Pages 会自动构建并发布。

## AI 语料

构建时生成，供 AI 检索和问答使用：

- [llms.txt](https://deepseek-browser-use.io.nexus/llms.txt)：页面目录
- [llms-full.txt](https://deepseek-browser-use.io.nexus/llms-full.txt)：完整正文
- [ai/index.json](https://deepseek-browser-use.io.nexus/ai/index.json)：页面元数据
- [ai/chunks.jsonl](https://deepseek-browser-use.io.nexus/ai/chunks.jsonl)：按标题分段的语料
- `/ai/pages/<路径>.md`：每页的 Markdown 原文
