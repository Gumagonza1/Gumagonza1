<div align="center">

# Gumaro González · @Gumagonza1

**Owner & CTO · Tacos Aragón** | Culiacán, Sinaloa, México

*Self-taught developer. Built a full automation ecosystem for a real restaurant — in production since 2020.*

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
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)

**AI & Cloud**

![Intelligent Agents](https://img.shields.io/badge/Intelligent_Agents-agentic_loops-00e5ff?style=flat-square)
![Google Cloud STT](https://img.shields.io/badge/Google_Cloud-STT%2FTTS-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-processing-a855f7?style=flat-square)

**Frontend & Mobile**

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server_2022-0078D4?style=flat-square&logo=windows&logoColor=white)
![IIS](https://img.shields.io/badge/IIS-0078D4?style=flat-square&logo=microsoft&logoColor=white)
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

A fully custom automation platform built from scratch to digitalize a family restaurant. Every module handles real orders, invoices, and customers daily.

```
Customer
  ├── WhatsApp ──────────► tacos-aragon-bot        (NLP agent + Loyverse POS)
  ├── Phone call ─────────► tacos-aragon-llamadas   (Twilio + Google STT/TTS)
  ├── Mobile app ─────────► tacos-aragon-app        (React Native + Expo)
  │                          via tacos-aragon-api   (agentic loop + tool use)
  ├── Website ────────────► tacos-aragon-web        (Flask + CFDI 4.0)
  └── Tax / SAT ──────────► tacos-aragon-fiscal     (cfdiclient + SAT SOAP)

                    ┌─────────────────────────────────┐
All services ──────►│  orchestrator  (Dockerized)      │──► Owner (Telegram)
                    │  health · recovery · reasoning   │
                    │  approval queue · scheduler      │
                    └─────────────────────────────────┘
                              │
                    telegram-dispatcher (approval buttons ✅ ❌)
```

| Repo | Stack | Description |
|------|-------|-------------|
| [ecosistema-aragon](https://github.com/Gumagonza1/ecosistema-aragon) | — | Full system architecture |
| [tacos-aragon-bot](https://github.com/Gumagonza1/tacos-aragon-bot) | Node.js · whatsapp-web.js · Google STT | NLP ordering bot + voice recognition |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Express · Agentic SDK | Central API with agentic tool use |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · EAS | Internal mobile dashboard |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Website + electronic invoicing |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT SOAP | Bulk SAT CFDI download + fiscal analysis |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Automated voice ordering |
| [tacos-aragon-wp](https://github.com/Gumagonza1/tacos-aragon-wp) | PHP · WordPress · Facturama | WP plugin: invoicing + Loyverse sync |
| [tacos-aragon-orchestrator](https://github.com/Gumagonza1/ecosistema-aragon) | Docker · Node.js · SQLite | Self-healing orchestrator + reasoning engine |

---

## In Production

- ✅ WhatsApp bot taking real orders 24/7 with NLP
- ✅ Voice ordering via automated phone system (Twilio → STT → POS → TTS)
- ✅ CFDI 4.0 electronic invoicing from website
- ✅ Internal mobile app with sales dashboard + bot controls
- ✅ Automated SAT bulk CFDI download + AI fiscal analysis
- ✅ Self-healing orchestrator — health polling every 30s, auto-restart, Telegram approvals
- ✅ `tacosaragon.com.mx` on Windows Server 2022 + IIS + Let's Encrypt
- ✅ `gumaro.dev.tacosaragon.com.mx` — personal portfolio

---

## About

Restaurant owner and self-taught developer. Since 2020 I've built every tool myself — no team, all running in production, handling real money and real customers daily.

> *Building intelligent systems for the businesses that actually run Mexico.*

---
---

<div align="center"><b>🇲🇽 Versión en Español</b></div>

---

## Stack

**Runtime & Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)

**IA & Cloud**

![Agentes Inteligentes](https://img.shields.io/badge/Agentes_Inteligentes-agentic_loops-00e5ff?style=flat-square)
![Google Cloud STT](https://img.shields.io/badge/Google_Cloud-STT%2FTTS-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-procesamiento-a855f7?style=flat-square)

**Frontend & Mobile**

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Infraestructura**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server_2022-0078D4?style=flat-square&logo=windows&logoColor=white)
![IIS](https://img.shields.io/badge/IIS-0078D4?style=flat-square&logo=microsoft&logoColor=white)
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

Plataforma de automatización construida desde cero para digitalizar un restaurante familiar. Cada módulo procesa pedidos, facturas y clientes reales todos los días.

```
Cliente
  ├── WhatsApp ──────────► tacos-aragon-bot        (agente NLP + Loyverse POS)
  ├── Llamada ────────────► tacos-aragon-llamadas   (Twilio + Google STT/TTS)
  ├── App móvil ──────────► tacos-aragon-app        (React Native + Expo)
  │                          via tacos-aragon-api   (agentic loop + tool use)
  ├── Sitio web ──────────► tacos-aragon-web        (Flask + CFDI 4.0)
  └── SAT / Fiscal ───────► tacos-aragon-fiscal     (cfdiclient + SAT SOAP)

                    ┌─────────────────────────────────┐
Todos los servicios►│  orquestador  (Dockerizado)      │──► Admin (Telegram)
                    │  salud · recuperación · razonamiento │
                    │  cola de aprobaciones · scheduler│
                    └─────────────────────────────────┘
                              │
                    telegram-dispatcher (botones ✅ ❌)
```

| Repo | Stack | Descripción |
|------|-------|-------------|
| [ecosistema-aragon](https://github.com/Gumagonza1/ecosistema-aragon) | — | Arquitectura general del sistema |
| [tacos-aragon-bot](https://github.com/Gumagonza1/tacos-aragon-bot) | Node.js · whatsapp-web.js · Google STT | Bot de pedidos NLP + reconocimiento de voz |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Express · Agentic SDK | API central con agentic tool use |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · EAS | Dashboard móvil interno |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Sitio web + facturación electrónica |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT SOAP | Descarga masiva CFDI + análisis fiscal |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Pedidos por llamada automática |
| [tacos-aragon-wp](https://github.com/Gumagonza1/tacos-aragon-wp) | PHP · WordPress · Facturama | Plugin WP: facturación + Loyverse |
| [tacos-aragon-orchestrator](https://github.com/Gumagonza1/ecosistema-aragon) | Docker · Node.js · SQLite | Orquestador auto-recuperable + motor de razonamiento |

---

## En producción

- ✅ Bot WhatsApp tomando pedidos reales 24/7 con NLP
- ✅ Pedidos por llamada automática (Twilio → STT → POS → TTS)
- ✅ Facturación electrónica CFDI 4.0 desde el sitio web
- ✅ App móvil interna con dashboard de ventas + control del bot
- ✅ Descarga masiva SAT + análisis fiscal automatizado
- ✅ Orquestador auto-recuperable — polling cada 30s, reinicio automático, aprobaciones por Telegram
- ✅ `tacosaragon.com.mx` en Windows Server 2022 + IIS + Let's Encrypt
- ✅ `gumaro.dev.tacosaragon.com.mx` — portafolio personal

---

## Contexto

Restaurantero y desarrollador. Desde 2020 construí cada herramienta yo mismo — sin equipo, en producción real, con dinero y clientes reales todos los días.

> *Construyendo sistemas inteligentes para los negocios que realmente mueven México.*

---

<div align="center">
<sub>Culiacán, Sinaloa · Tacos Aragón · Mar–Dom 6pm–11:30pm 🌮</sub>
</div>
