<p align="center">
  <img src="https://via.placeholder.com/1280x400?text=Flujo+NoCode+Automatizado" alt="Banner" width="100%"/>
</p>

<h1 align="center">Mi Flujo NoCode</h1>

<p align="center">
  <strong>Automatización NoCode para procesar formularios de Google Forms, enriquecer datos y enviarlos a Notion y Slack — sin una sola línea de código.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Antigravity-Compatible-FF6B35?style=for-the-badge" alt="Antigravity"/>
  <img src="https://img.shields.io/badge/Make-6D00CC?style=for-the-badge&logo=make" alt="Make"/>
  <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion" alt="Notion"/>
  <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack" alt="Slack"/>
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
</p>

---

## 📖 Acerca del Proyecto

Cuando un usuario envía un formulario de Google Forms, este flujo:
1. Captura la respuesta automáticamente
2. Enriquece los datos con IA (Claude via Antigravity)
3. Crea una entrada en Notion con los datos procesados
4. Envía una notificación a Slack con un resumen

**Tiempo ahorrado:** ~45 minutos por respuesta procesada manualmente → **0 minutos** con el flujo.

---

## 🏗️ Arquitectura del Flujo

<p align="center">
  <img src="https://via.placeholder.com/800x200?text=Google+Forms+→+Antigravity+AI+→+Notion+→+Slack" alt="Arquitectura" width="800"/>
</p>

```
Google Forms (trigger)
    ↓
Antigravity — Nodo Claude AI (enriquecimiento)
    ↓
Notion — Crear página en base de datos
    ↓
Slack — Enviar mensaje al canal #leads
```

---

## ✨ Características

| Característica | Detalle |
|---|---|
| 🔄 **Trigger automático** | Se activa con cada envío del formulario |
| 🤖 **Procesamiento con IA** | Claude categoriza y enriquece cada respuesta |
| 📝 **Notion integrado** | Crea ficha completa con todos los campos |
| 💬 **Alerta Slack** | Notificación instantánea al equipo |
| ⚡ **Tiempo de proceso** | < 8 segundos end-to-end |

---

## 🚀 Cómo importar este flujo

### En Antigravity

1. Descarga el archivo `flujo.json` de este repositorio
2. En Antigravity → **Importar flujo** → selecciona `flujo.json`
3. Configura las credenciales en cada nodo:
   - Google: conecta tu cuenta
   - Notion: agrega tu Integration Token
   - Slack: agrega el Webhook URL de tu canal

### Variables de entorno necesarias

| Variable | Dónde obtenerla |
|---|---|
| `NOTION_TOKEN` | [Notion Integrations](https://notion.so/my-integrations) |
| `SLACK_WEBHOOK` | [Slack API](https://api.slack.com/apps) → Incoming Webhooks |
| `CLAUDE_API_KEY` | [Anthropic Console](https://console.anthropic.com) |

---

## 🎬 Demo

<p align="center">
  <img src="https://via.placeholder.com/700x400?text=Demo+→+Formulario+enviado+→+Notion+actualizado+→+Slack+notificado" alt="Demo" width="700"/>
</p>

---

## 💖 Apoya este Proyecto

<p align="center">
  <img src="https://img.shields.io/badge/XRP-rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj-00AAE4?style=for-the-badge&logo=ripple" alt="XRP"/>
</p>

> Dirección XRP: `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`

---

## 📬 Contacto — Oscar Omar Gómez Peña

<p align="center">
  <a href="https://oscaromargp.github.io/Oscaromargp/">
    <img src="https://img.shields.io/badge/Portafolio-Web-blueviolet?style=for-the-badge&logo=github" alt="Portafolio"/>
  </a>
  &nbsp;
  <a href="https://github.com/oscaromargp">
    <img src="https://img.shields.io/badge/GitHub-oscaromargp-181717?style=for-the-badge&logo=github" alt="GitHub"/>
  </a>
</p>

## 🙏 Agradecimientos

<p align="center">
  <br/>
  <em>
    "Porque Dios es el que en vosotros produce<br/>
    así el querer como el hacer,<br/>
    por su buena voluntad."
  </em>
  <br/>
  <strong>— Filipenses 2:13</strong>
  <br/><br/>
  Todo lo que aquí existe nació primero como un deseo en el corazón.<br/>
  Cada proyecto, cada línea, cada idea que toma forma —<br/>
  es un regalo de Aquel que nos dio tanto el sueño como la fuerza de alcanzarlo.<br/>
  <strong>A Dios, toda la gloria.</strong>
  <br/>
</p>

---

## 📄 Licencia

MIT © [Oscar Omar Gómez Peña](https://github.com/oscaromargp)
