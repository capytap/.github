# Capytap · 豚豚

> AI agent that helps non-technical users self-host on their own VPS.  
> 让小白用自己的 VPS 几分钟跑通——AI Agent 自动 SSH + 选协议 + 装服务。

**Status**: Pre-launch · PoC v0 validated 2026-05-25 · Public beta Q3 2026

## What we're building

A desktop client that turns "I bought a VPS but don't know how to use it" into "I have working dual-protocol proxy in 2 minutes", powered by:

- **AI Agent (DeepSeek v4-pro)** — protocol selection + config generation per VPS environment
- **Python orchestrator** — deterministic install flow (sing-box, systemd, ufw, certs)
- **Tauri + React client** — Windows-first, macOS / Android later

> v1 Tauri desktop client scaffolded 2026-05-26 in 19 min — bilingual (EN/ZH), 5 routed screens, ready for backend wire-up.

PoC v0 metrics (2 days of work, ~$0.07 in LLM cost):

| Metric | Value |
|---|---|
| End-to-end install on blank VPS | 134s |
| AI cost per install | ~$0.005 (¥0.04) |
| Engineering specs hardened | **10/10** (overnight Day 2) |
| QA regression scenarios | **5/5 passing** |
| Total AI cost (2 days) | ~$0.07 (¥0.51) |
| AI self-retry loop validated | ✓ |

## Roadmap

- ✅ PoC v0 (2026-05-24 → 25): blank VPS → working dual-protocol proxy, validated
- ✅ Engineering hardening: atomic config swap, post-start verify, auto-rollback, AI-retry-on-failure loop
- 🟡 v1 desktop client (Tauri + React) — in progress
- ⏳ Public beta Q3 2026
- ⏳ Early-bird founder lifetime license, $30 (¥199), first 100 buyers

## Contact

Building in public. DM on Twitter [@capytap](https://x.com/capytap) or wait for capytap.com.
