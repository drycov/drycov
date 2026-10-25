## Hi there! 👋
[![Visitors](https://komarev.com/ghpvc/?username=drycov&label=Profile%20views&color=0e75b6&style=flat)](https://github.com/drycov)
[![GitHub Followers](https://img.shields.io/github/followers/drycov?label=Follow&style=social)](https://github.com/drycov)
[![Telegram Badge](https://img.shields.io/badge/-Telegram-0088CC?style=flat&logo=Telegram&logoColor=white)](https://t.me/ITISIDevRykov)

I'm a **full-stack developer** with expertise in **network configuration**, **CCTV/inventory systems**, and **Docker-based operations tooling**. I build practical platforms for field teams and network engineers — not just demos.

---

## 🚀 About Me
- 🔭 Building an **ops platform**: shared libs → inventory → field bot / CMS / backup
- 🌱 Learning **Rust** and **Kubernetes**
- ⚡ Fun fact: I love traveling and photography

---

## 🏗 Ops platform ecosystem

**One platform, several products.** Shared libraries first; separate UIs for operators, field staff, and backup compliance.

```text
Sources: Cerebro · ONVIF · Hikvision/Dahua · SNMP · MikroTik · Zabbix
                    │
    ┌───────────────┼───────────────────┐
    ▼               ▼                   ▼
camera-probe   network-core      cerebro-client
(lib)          (lib)             (lib)
    │               │                   │
    └───────────────┼───────────────────┘
                    ▼
            inventory + jobs
         (registry, sync, ping)
                    │
     ┌──────────────┼──────────────┬──────────────┐
     ▼              ▼              ▼              ▼
   cms        equipment-bot    backup_tool    erp / ppr
 (CCTV ops)   (field+map+TG)   (configs)     (process)
```

| Layer | Repos | Role |
| --- | --- | --- |
| **Camera lib** | [`camera-probe`](https://github.com/drycov/camera-probe) | Discovery / ONVIF / vendor identity probes |
| **Network lib** | [`network-core`](https://github.com/drycov/network-core) | MikroTik RouterOS API, read-only SSH, vendor labels, geo |
| **Cerebro lib** | [`cerebro-client`](https://github.com/drycov/cerebro-client) | HTTP client + channel helpers (no product DB) |
| **Field product** | [`equipment-bot`](https://github.com/drycov/equipment-bot) | Telegram + map; depends on all three libs |
| **Operator product** | [`cms`](https://github.com/drycov/cms) | CCTV operations UI |
| **Backup product** | [`backup_tool`](https://github.com/drycov/backup_tool) | Config backup, discovery, compliance |
| **Business process** | [`ppr-system`](https://github.com/drycov/ppr-system), ERP/Zeus | Processes — link equipment by ID |

**Rules (anti-duplication):**
1. Camera protocol code lives in **`camera-probe`** — products depend on it.
2. RouterOS / SSH / vendor normalize / geo live in **`network-core`**.
3. Cerebro HTTP lives in **`cerebro-client`**; products only upsert into their store.
4. Do **not** merge field bot and CMS into one monolith — share libs, not UX.
5. ERP/PPR consume inventory via API/ID — no copy of probe stacks.

Detail: [equipment-bot `docs/platform.md`](https://github.com/drycov/equipment-bot/blob/main/docs/platform.md)

---

## 🛠 Tech Stack & Tools

### Programming Languages
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![PHP](https://img.shields.io/badge/-PHP-777BB4?style=flat-square&logo=php&logoColor=white)

### Frameworks & Libraries
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![aiogram](https://img.shields.io/badge/-aiogram-2AABEE?style=flat-square&logo=telegram&logoColor=white)

### Databases & Infra
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## 📈 GitHub Stats
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=drycov&theme=radical&show_icons=true)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=drycov&layout=compact&theme=radical)](https://github.com/drycov)

---

## 📫 Contact Me
- Email: [drycov@gmail.com](mailto:drycov@gmail.com)
- Telegram: [@ITISIDevRykov](https://t.me/ITISIDevRykov)
