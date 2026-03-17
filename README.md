<div align="center">

# Gumaro González · @Gumagonza1

**Owner & CTO · Tacos Aragón** | Culiacán, Sinaloa, México 🌮

*Self-taught developer building AI-powered operations for a real restaurant — since 2020.*

[![Website](https://img.shields.io/badge/app.tacosaragon.com.mx-live-brightgreen?style=flat-square&logo=googlechrome&logoColor=white)](https://app.tacosaragon.com.mx)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gumaro_González-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/gumaro-gonzalez)

</div>

---

## 🏗️ Aragón Ecosystem

A fully custom automation platform I built from scratch to digitalize a family restaurant. Every module is in production, handling real orders, invoices, and customers daily.

```
Customer
  ├── WhatsApp ──────────► tacos-aragon-bot       (Gemini + Loyverse POS)
  │                              │
  │                         tacos-aragon-monitor  ← Claude audits every bot response in real time
  │                         (tool use: logs, conversations, proposes fixes to admin)
  │
  ├── Phone call ─────────► tacos-aragon-llamadas  (Twilio + Google STT/TTS)
  ├── Mobile app ─────────► tacos-aragon-app       (React Native + Expo)
  │                          via tacos-aragon-api  (Claude agent + tool use)
  ├── Website ────────────► tacos-aragon-web       (Flask + CFDI 4.0)
  └── Tax / SAT ──────────► tacos-aragon-fiscal    (cfdiclient + Gemini)
                             cfo-aragon-agent       (Claude + FastAPI)
```

| Repo | Stack | Description |
|------|-------|-------------|
| [ecosistema-aragon](https://github.com/Gumagonza1/ecosistema-aragon) | — | Full system architecture overview |
| [whatsapp-tacos-bot](https://github.com/Gumagonza1/whatsapp-tacos-bot) | Node.js · Gemini · whatsapp-web.js | Natural-language ordering bot + POS integration |
| [tacos-aragon-monitor](https://github.com/Gumagonza1/tacos-aragon-monitor) | Node.js · Claude · Tool Use | Real-time quality audit agent for the WhatsApp bot |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Voice bot for phone orders |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Claude · Loyverse · Facturama | Central API + agentic tool use |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · Gemini STT | Internal mobile app with voice + sales dashboard |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Electronic invoicing portal |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT | Bulk SAT download and CFDI analysis |
| [cfo-aragon-agent](https://github.com/Gumagonza1/cfo-aragon-agent) | FastAPI · Claude · Gemini | Automated CFO: P&L, VAT/ISR, balance sheet |
| [bot-loyverse](https://github.com/Gumagonza1/bot-loyverse) | Python · pandas · matplotlib | Analytics and reports from Loyverse POS |

---

## 🧠 Stack

**Backend**
`Python` `Flask` `FastAPI` `Node.js` `Express`

**AI / Agents**
`Claude (Anthropic)` `Gemini (Google)` `Tool Use` `Agentic Loops` `STT/TTS`

**Integrations**
`Loyverse POS` `Facturama PAC` `SAT CFDI 4.0` `WhatsApp API` `Twilio` `MercadoPago`

**Infra**
`GCP VM` `Windows Server 2022` `IIS` `NSSM` `PM2` `Let's Encrypt` `SQLite` `PostgreSQL`

**Mobile**
`React Native` `Expo` `EAS Build`

---

## 🚀 In Production

- ✅ WhatsApp bot taking orders 24/7
- ✅ **Real-time audit agent**: Claude reviews every bot message, detects errors (wrong prices, unavailable items, tone) and proposes fixes to the admin via WhatsApp (`!m si` / `!m no`)
- ✅ Electronic invoicing CFDI 4.0 from the website
- ✅ Internal mobile app with voice agent (Claude + Gemini STT)
- ✅ CFO agent: automatic SAT download + AI-powered tax analysis
- ✅ `app.tacosaragon.com.mx` running on GCP with SSL

---

## 📍 Context

I'm a restaurant owner and self-taught developer. Since 2020 I've digitalized Tacos Aragón by building every tool myself — no team, from my phone, all running in production.

> *Building AI for the businesses that actually run Mexico.*

---
---

<div align="center"><b>🇲🇽 Versión en Español</b></div>

---

## 🏗️ Ecosistema Aragón

Plataforma de automatización construida desde cero para digitalizar un restaurante familiar. Cada módulo está en producción, procesando pedidos, facturas y clientes reales todos los días.

```
Cliente
  ├── WhatsApp ──────────► tacos-aragon-bot       (Gemini + Loyverse POS)
  │                              │
  │                         tacos-aragon-monitor  ← Claude audita cada respuesta en tiempo real
  │                         (tool use: logs, conversaciones, propone fixes al admin)
  │
  ├── Llamada telefónica ► tacos-aragon-llamadas  (Twilio + Google STT/TTS)
  ├── App móvil ──────────► tacos-aragon-app       (React Native + Expo)
  │                          via tacos-aragon-api  (Claude agent + tool use)
  ├── Sitio web ──────────► tacos-aragon-web       (Flask + CFDI 4.0)
  └── SAT / Fiscal ───────► tacos-aragon-fiscal    (cfdiclient + Gemini)
                             cfo-aragon-agent       (Claude + FastAPI)
```

| Repo | Stack | Descripción |
|------|-------|-------------|
| [ecosistema-aragon](https://github.com/Gumagonza1/ecosistema-aragon) | — | Arquitectura general del sistema |
| [whatsapp-tacos-bot](https://github.com/Gumagonza1/whatsapp-tacos-bot) | Node.js · Gemini · whatsapp-web.js | Bot de pedidos en lenguaje natural + integración POS |
| [tacos-aragon-monitor](https://github.com/Gumagonza1/tacos-aragon-monitor) | Node.js · Claude · Tool Use | Agente de auditoría en tiempo real del bot WhatsApp |
| [tacos-aragon-llamadas](https://github.com/Gumagonza1/tacos-aragon-llamadas) | Node.js · Twilio · Google STT/TTS | Bot de llamadas con voz en tiempo real |
| [tacos-aragon-api](https://github.com/Gumagonza1/tacos-aragon-api) | Node.js · Claude · Loyverse · Facturama | API central + agente con tool use |
| [tacos-aragon-app](https://github.com/Gumagonza1/tacos-aragon-app) | React Native · Expo · Gemini STT | App interna con voz + dashboard de ventas |
| [tacos-aragon-web](https://github.com/Gumagonza1/tacos-aragon-web) | Python · Flask · CFDI 4.0 | Portal de facturación electrónica |
| [tacos-aragon-fiscal](https://github.com/Gumagonza1/tacos-aragon-fiscal) | Python · cfdiclient · SAT | Descarga masiva y análisis de CFDIs |
| [cfo-aragon-agent](https://github.com/Gumagonza1/cfo-aragon-agent) | FastAPI · Claude · Gemini | CFO automatizado: P&L, ISR/IVA, balance |
| [bot-loyverse](https://github.com/Gumagonza1/bot-loyverse) | Python · pandas · matplotlib | Analytics y reportes desde Loyverse POS |

---

## 🚀 En producción

- ✅ Bot WhatsApp tomando pedidos 24/7
- ✅ **Agente monitor de auditoría**: Claude revisa cada mensaje del bot en tiempo real, detecta errores (precios, ítems no disponibles, tono) y propone fixes al admin vía WhatsApp con `!m si` / `!m no`
- ✅ Facturación electrónica CFDI 4.0 desde el sitio web
- ✅ App móvil interna con agente de voz (Claude + Gemini STT)
- ✅ CFO agent: descarga SAT automática + análisis fiscal con IA
- ✅ `app.tacosaragon.com.mx` en GCP con SSL

---

## 📍 Contexto

Soy restaurantero y desarrollador. Desde 2020 digitalicé Tacos Aragón construyendo cada herramienta yo mismo — sin equipo, desde el celular, en producción real.

> *Construyendo IA para los negocios que realmente mueven México.*

---

<div align="center">
<sub>Culiacán, Sinaloa · Tacos Aragón · Mar–Dom 6pm–11:30pm 🌮</sub>
</div>
