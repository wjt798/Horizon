# 🌅 Horizon — AI 信息雷达

> 你的专属 AI 信息收集系统，每日自动抓取、评分、汇总 AI Agent、开源动态、超级个体资讯。

## 配置完成 ✅

本项目已为你完成以下配置：

| 项目 | 内容 |
|------|------|
| **AI 提供商** | DeepSeek (`deepseek-chat`) |
| **API Key** | 已配置在 `.env` |
| **新闻源** | Hacker News / Reddit / GitHub / RSS / OSS Insight |
| **关注领域** | AI Agent、AI工具、开源项目、一人公司、独立开发者生态 |
| **自动运行** | GitHub Actions 每日 UTC 22:00（北京时间 06:00） |
| **语言** | 中英双语日报 |

## 首次运行

### 方式 1：本地运行（需要 Python 3.11+）

```bash
cd Horizon

# 安装 uv 包管理器（推荐）
pip install uv

# 安装依赖
uv sync

# 运行 Horizon
uv run horizon

# 运行设置向导（可选）
uv run horizon-wizard
```

### 方式 2：Docker 运行

```bash
docker compose run --rm horizon
```

### 方式 3：GitHub Actions（每日自动运行）

1. 将本项目推送到你的 GitHub 仓库
2. 在 GitHub 仓库 Settings → Secrets and variables → Actions 中添加：
   - `DEEPSEEK_API_KEY` = `sk-c1d3f01d527a457f9d130362dd559baa`
3. 手动触发 Workflow 或等待每日定时运行
4. 生成的日报会自动部署到 GitHub Pages

### 方式 4：飞书/钉钉/邮件推送

如需要推送通知到飞书、钉钉或邮箱，请告知我，我帮你配置 webhook。

## 已配置的新闻源

### 🌐 Hacker News
- 科技创业前沿，Top 30 热门讨论

### 💬 Reddit
- `r/ArtificialIntelligence` — AI 前沿讨论
- `r/LocalLLaMA` — 本地大模型部署
- `r/SaaS` — SaaS 创业
- `r/Entrepreneur` — 创业圈
- `r/opensource` — 开源社区
- `r/selfhosted` — 自部署/自托管
- `r/indiebiz` — 独立开发者生意

### 🐙 GitHub
- **大佬动态**: karpathy, ggerganov, n8n-io
- **热门项目**: Dify, n8n, Firecrawl, AutoGPT, RAGFlow, AnythingLLM, browser-use

### 📡 RSS
- Simon Willison 博客 — LLM 工具与实验
- 量子位 / 新智元 — 中文 AI 资讯
- GitHub Trending — 每日热门仓库
- TechCrunch — 创业新闻
- Indie Hackers — 独立开发者社区

### 📊 OSS Insight
- GitHub 全站热门开源项目 AI/Agent 筛选
