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
    ┌───────────────┼───────────────────┬────────────────┐
    ▼               ▼                   ▼                ▼
camera-probe   network-core      cerebro-client    design-kit
(lib)          (lib)             (lib)             (UI)
    │               │                   │                │
    └───────────────┴───────────────────┴────────────────┘
                              │
                      inventory + jobs
                              │
     ┌──────────────┬─────────┴────────┬──────────────┐
     ▼              ▼                  ▼              ▼
   cms        equipment-bot       backup_tool    erp / ppr
```

| Layer | Repos | Role |
| --- | --- | --- |
| **Camera lib** | [`camera-probe`](https://github.com/drycov/camera-probe) | Discovery / ONVIF / vendor probes |
| **Network lib** | [`network-core`](https://github.com/drycov/network-core) | MikroTik, SSH facts, vendor labels, geo |
| **Cerebro lib** | [`cerebro-client`](https://github.com/drycov/cerebro-client) | HTTP client + channel helpers |
| **UI kit** | [`design-kit`](https://github.com/drycov/design-kit) | Telegram tokens, CSS, React primitives |
| **Field product** | [`equipment-bot`](https://github.com/drycov/equipment-bot) | Telegram + map |
| **Operator product** | [`cms`](https://github.com/drycov/cms) | CCTV operations UI |
| **Backup product** | [`backup_tool`](https://github.com/drycov/backup_tool) | Config backup & compliance |

**Rules:** share **libs and design kit**, not product UX shells. ERP/PPR link equipment by ID only.

---

## 🛠 Tech Stack & Tools

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## 📈 GitHub Stats
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=drycov&theme=radical&show_icons=true)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=drycov&layout=compact&theme=radical)](https://github.com/drycov)

---

## 📫 Contact Me
- Email: [drycov@gmail.com](mailto:drycov@gmail.com)
- Telegram: [@ITISIDevRykov](https://t.me/ITISIDevRykov)
