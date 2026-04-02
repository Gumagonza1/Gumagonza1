<div align="center">

# Gumaro González · @Gumagonza1

**Owner & CTO · Tacos Aragón** | Culiacán, Sinaloa, México

*Self-taught developer. Built a full automation ecosystem for a real restaurant — 9 Docker containers in production on GCP.*

[![Portfolio](https://img.shields.io/badge/portfolio-gumaro.dev.tacosaragon.com.mx-00e5ff?style=flat-square&logo=googlechrome&logoColor=black)](https://gumaro.dev.tacosaragon.com.mx)
[![Website](https://img.shields.io/badge/tacosaragon.com.mx-live-00ff88?style=flat-square&logo=googlechrome&logoColor=black)](https://tacosaragon.com.mx)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gumaro_González-0077B5?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/gumaro-antonio-gonz%C3%A1lez-arag%C3%B3n-57644b159)
[![Email](https://img.shields.io/badge/email-gumaro.gonzalez@tacosaragon.com.mx-a855f7?style=flat-square&logo=gmail&logoColor=white)](mailto:gumaro.gonzalez@tacosaragon.com.mx)

</div>

---

## Stack

**Runtime & Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)

**AI Models & Agents**

![Claude Sonnet](https://img.shields.io/badge/Claude_Sonnet_4.6-tool_use-000000?style=flat-square&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-ordering_bot-4285F4?style=flat-square&logo=googlegemini&logoColor=white)
![Agentic Loops](https://img.shields.io/badge/Agentic_Loops-multi--agent-00e5ff?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-tool_servers-a855f7?style=flat-square)

**Frontend & Mobile**

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-000000?style=flat-square&logo=tailscale&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Let's Encrypt](https://img.shields.io/badge/Let's_Encrypt-003A70?style=flat-square&logo=letsencrypt&logoColor=white)

**Integrations**

![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=flat-square&logo=whatsapp&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Loyverse](https://img.shields.io/badge/Loyverse_POS-FF6600?style=flat-square)
![Facturama](https://img.shields.io/badge/Facturama_PAC-CFDI_4.0-00b4a0?style=flat-square)
![SAT](https://img.shields.io/badge/SAT-CFDI_4.0-red?style=flat-square)
![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white)

---

## Aragón Ecosystem

A fully custom automation platform built from scratch to digitalize a family restaurant. 9 Docker containers running on GCP, handling real orders, invoices, and customers daily.

```
Customer
  ├── WhatsApp ──────────► whatsapp-tacos-bot      (Gemini 2.5-flash + Loyverse POS)
  ├── Phone call ─────────► tacos-aragon-llamadas   (Twilio + Google STT/TTS)
  ├── Mobile app ─────────► tacos-aragon-app        (React Native + Expo)
  │                          via tacos-aragon-api   (Claude Sonnet + tool use)
  ├── Website ────────────► tacos-aragon-web        (Flask + CFDI 4.0)
  └── Tax / SAT ──────────► tacos-aragon-fiscal     (cfdiclient + SAT SOAP)

                  ┌──────────────────────────────────────┐
All services ────►│  orchestrator (Docker Engine API)     │──► Owner (Telegram)
                  │  health · recovery · CPU priorities   │
                  │  approval queue · PMO autocorrect     │
                  └──────────────────────────────────────┘
                            │
                  ┌─────────┴─────────┐
                  │                   │
          pmo-agent             telegram-dispatcher
       (Claude Code CLI)       (approval buttons ✅ ❌)
```

| Repo | Stack | Description |
|------|-------|-------------|
| [whatsapp-tacos-bot](https://github.com/Gumagonza1/whatsapp-tacos-bot) | Node.js · Gemini 2.5-flash · Loyverse | WhatsApp ordering bot with AI + POS integration |
| [tacos-aragon-monitor](https://github.com/Gumagonza1/tacos-aragon-monitor) | Node.js · Claude Sonnet 4.6 · tool use | Real-time quality monitor with code proposals |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Express · Claude CLI | Central API: sales, agent, invoicing, accounting |
| [tacos-aragon-orchestrator](https://github.com/Gumagonza1/tacos-aragon-orchestrator) | Docker Engine API · Node.js · SQLite | Self-healing watchdog with CPU priorities |
| [pmo-agent](https://github.com/Gumagonza1/pmo-agent) | Node.js · Claude Code CLI · MCP | Autonomous code agent with changelog system |
| [aragon-git-guardian](https://github.com/Gumagonza1/aragon-git-guardian) | Bash · Claude Code hooks | Pre-push security audit (15 categories) |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · EAS | Internal mobile dashboard |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Website + electronic invoicing |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT SOAP | Bulk SAT CFDI download + fiscal analysis |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Automated voice ordering |
| [tacos-aragon-wp](https://github.com/Gumagonza1/tacos-aragon-wp) | PHP · WordPress · Facturama | WP plugin: invoicing + Loyverse sync |
| cfo-aragon-agent | Python · Claude Sonnet · FastAPI | AI CFO — P&L, SAT cross-reference *(private)* |

---

## In Production

- ✅ 9 Docker containers on GCP Linux (migrated from Windows Server)
- ✅ WhatsApp bot taking real orders with Gemini AI + Loyverse POS auto-registration
- ✅ Quality monitor (Claude Sonnet) watching every conversation in real-time
- ✅ Voice ordering via automated phone system (Twilio → STT → POS → TTS)
- ✅ CFDI 4.0 electronic invoicing (Facturama PAC)
- ✅ Internal mobile app with sales dashboard + AI chat agent
- ✅ AI CFO agent for accounting, P&L, and SAT fiscal analysis
- ✅ Self-healing orchestrator with Docker Engine API, CPU priority management
- ✅ PMO agent: autonomous code corrections via Claude Code CLI
- ✅ Git Guardian: pre-push security audit (tokens, PII, bank data, GPS, phones)
- ✅ Monthly customer retention campaigns with personalized AI-generated promos
- ✅ Tailscale mesh network connecting all services

---

## About

Restaurant owner and self-taught developer. Since 2020 I've built every tool myself — no team, all running in production, handling real money and real customers daily.

> *Building intelligent systems for the businesses that actually run Mexico.*

---
---

<div align="center"><b>Versión en Español</b></div>

---

## Stack

**Runtime & Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)

**Modelos IA y Agentes**

![Claude Sonnet](https://img.shields.io/badge/Claude_Sonnet_4.6-tool_use-000000?style=flat-square&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-bot_pedidos-4285F4?style=flat-square&logo=googlegemini&logoColor=white)
![Agentic Loops](https://img.shields.io/badge/Loops_Agénticos-multi--agente-00e5ff?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-tool_servers-a855f7?style=flat-square)

**Frontend & Mobile**

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Infraestructura**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-000000?style=flat-square&logo=tailscale&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Let's Encrypt](https://img.shields.io/badge/Let's_Encrypt-003A70?style=flat-square&logo=letsencrypt&logoColor=white)

**Integraciones**

![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=flat-square&logo=whatsapp&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Loyverse](https://img.shields.io/badge/Loyverse_POS-FF6600?style=flat-square)
![Facturama](https://img.shields.io/badge/Facturama_PAC-CFDI_4.0-00b4a0?style=flat-square)
![SAT](https://img.shields.io/badge/SAT-CFDI_4.0-red?style=flat-square)
![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white)

---

## Ecosistema Aragón

Plataforma de automatización construida desde cero para digitalizar un restaurante familiar. 9 contenedores Docker en GCP, procesando pedidos, facturas y clientes reales todos los días.

```
Cliente
  ├── WhatsApp ──────────► whatsapp-tacos-bot      (Gemini 2.5-flash + Loyverse POS)
  ├── Llamada ────────────► tacos-aragon-llamadas   (Twilio + Google STT/TTS)
  ├── App móvil ──────────► tacos-aragon-app        (React Native + Expo)
  │                          via tacos-aragon-api   (Claude Sonnet + tool use)
  ├── Sitio web ──────────► tacos-aragon-web        (Flask + CFDI 4.0)
  └── SAT / Fiscal ───────► tacos-aragon-fiscal     (cfdiclient + SAT SOAP)

                  ┌──────────────────────────────────────┐
Todos los         │  orquestador (Docker Engine API)      │──► Admin (Telegram)
servicios ───────►│  salud · recuperación · prioridades CPU│
                  │  aprobaciones · auto-corrección PMO   │
                  └──────────────────────────────────────┘
                            │
                  ┌─────────┴─────────┐
                  │                   │
          pmo-agent             telegram-dispatcher
       (Claude Code CLI)       (botones ✅ ❌)
```

| Repo | Stack | Descripción |
|------|-------|-------------|
| [whatsapp-tacos-bot](https://github.com/Gumagonza1/whatsapp-tacos-bot) | Node.js · Gemini 2.5-flash · Loyverse | Bot de pedidos WhatsApp con IA + registro POS |
| [tacos-aragon-monitor](https://github.com/Gumagonza1/tacos-aragon-monitor) | Node.js · Claude Sonnet 4.6 · tool use | Monitor de calidad en tiempo real con propuestas de código |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Express · Claude CLI | API central: ventas, agente, facturación, contabilidad |
| [tacos-aragon-orchestrator](https://github.com/Gumagonza1/tacos-aragon-orchestrator) | Docker Engine API · Node.js · SQLite | Watchdog auto-recuperable con prioridades CPU |
| [pmo-agent](https://github.com/Gumagonza1/pmo-agent) | Node.js · Claude Code CLI · MCP | Agente de código autónomo con sistema de changelog |
| [aragon-git-guardian](https://github.com/Gumagonza1/aragon-git-guardian) | Bash · Claude Code hooks | Auditoría de seguridad pre-push (15 categorías) |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · EAS | Dashboard móvil interno |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Sitio web + facturación electrónica |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT SOAP | Descarga masiva CFDI + análisis fiscal |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Pedidos por llamada automática |
| [tacos-aragon-wp](https://github.com/Gumagonza1/tacos-aragon-wp) | PHP · WordPress · Facturama | Plugin WP: facturación + Loyverse |
| cfo-aragon-agent | Python · Claude Sonnet · FastAPI | Agente CFO con IA — P&L, cruces SAT *(privado)* |

---

## En producción

- ✅ 9 contenedores Docker en GCP Linux (migrado desde Windows Server)
- ✅ Bot WhatsApp tomando pedidos reales con Gemini AI + registro automático en Loyverse POS
- ✅ Monitor de calidad (Claude Sonnet) vigilando cada conversación en tiempo real
- ✅ Pedidos por llamada automática (Twilio → STT → POS → TTS)
- ✅ Facturación electrónica CFDI 4.0 (Facturama PAC)
- ✅ App móvil interna con dashboard de ventas + agente IA por chat
- ✅ Agente CFO con IA para contabilidad, P&L y análisis fiscal SAT
- ✅ Orquestador auto-recuperable con Docker Engine API y prioridades de CPU
- ✅ Agente PMO: correcciones de código autónomas via Claude Code CLI
- ✅ Git Guardian: auditoría de seguridad pre-push (tokens, PII, datos bancarios, GPS, teléfonos)
- ✅ Campañas mensuales de retención con promos personalizadas por IA
- ✅ Red mesh Tailscale conectando todos los servicios

---

## Contexto

Restaurantero y desarrollador. Desde 2020 construí cada herramienta yo mismo — sin equipo, en producción real, con dinero y clientes reales todos los días.

> *Construyendo sistemas inteligentes para los negocios que realmente mueven México.*

---

<div align="center">
<sub>Culiacán, Sinaloa · Tacos Aragón · Mar–Dom 6pm–11:30pm</sub>
</div>
