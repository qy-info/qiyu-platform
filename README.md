# QiYu Platform

**Shopee AI Copilot — 专为 Shopee 卖家打造的 AI 智能运营平台**

---

## 产品定位

QiYu 是一个面向 Shopee 卖家的 AI 智能运营平台。通过 AI 自动分析店铺数据、商品数据、广告数据和订单数据，帮助卖家提升运营效率和销售额。

## 核心功能

- **商品管理** — 原始商品上架、编辑、批量操作，多维度商品管理
- **智能分析** — 商品表现分析、销售趋势、利润计算
- **运营看板** — 核心指标实时监控，数据可视化
- **团队协作** — 多空间/多成员权限管理，支持团队协作
- **自动匹配引擎** — 自动商品匹配与利润计算
- **Shopee 集成** — 官方 API 对接，商品/订单自动同步

## 技术栈

| 层 | 技术 |
|---|---|
| 前端 | Next.js 16 (App Router) + React 19 + TypeScript |
| UI | TailwindCSS v4 + Shadcn/UI + Framer Motion |
| 状态管理 | Zustand + TanStack Query |
| 后端 | Go-zero + sqlx + MySQL |
| AI 服务 | Python FastAPI (预留) |

## 架构概览

```
前端 (Next.js)  ──→  后端 API (Go-zero)  ──→  MySQL
                        │
                        └──→ AI 服务 (FastAPI)
                        │
                        └──→ Shopee Open API
```

前端与后端通过 RESTful API 通信，后端负责业务逻辑与数据持久化，AI 服务提供智能分析能力，Shopee API 负责平台数据同步。

---

*QiYu — 让 Shopee 运营更智能*
