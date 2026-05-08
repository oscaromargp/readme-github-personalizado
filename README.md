<p align="center">
  <img src="assets/banner.png" alt="readme-github-personalizado" width="100%"/>
</p>

<h1 align="center">readme-github-personalizado</h1>

<p align="center">
  <strong>Skill para Claude, Antigravity y NoCode que genera READMEs profesionales y visualmente atractivos para GitHub — con badges, capturas de pantalla, GIFs y plantilla personalizada.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/version-2.0.0-green?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/PRs-welcome-orange?style=for-the-badge" alt="PRs Welcome"/>
  <img src="https://img.shields.io/badge/compatible-Claude%20%7C%20Antigravity%20%7C%20NoCode-blueviolet?style=for-the-badge" alt="Compatible"/>
</p>

<p align="center">
  <a href="#-acerca-del-proyecto">Acerca</a> •
  <a href="#-características">Características</a> •
  <a href="#-instalación">Instalación</a> •
  <a href="#-uso">Uso</a> •
  <a href="#-apoya-este-proyecto">Donar</a> •
  <a href="#-contacto">Contacto</a>
</p>

---

## 📖 Acerca del Proyecto

<p align="center">
  <img src="https://via.placeholder.com/700x380?text=README+generado+con+badges+%2B+screenshots+%2B+GIF+demo" alt="Demo del skill" width="700"/>
</p>

**readme-github-personalizado** es un skill listo para usar en Claude Code, Antigravity y NoCode que genera automáticamente un `README.md` de calidad profesional para cualquier proyecto.

Inspirado en los patrones de [awesome-readme](https://github.com/matiassingers/awesome-readme), el skill produce documentación que incluye badges de color, banners visuales, demostraciones en GIF, tablas de características con íconos, bloques de código con syntax highlighting, y una sección de donación XRP — todo con los datos de contacto de Oscar Omar Gómez Peña ya integrados.

### 🛠️ Construido Con

<p align="left">
  <img src="https://img.shields.io/badge/Claude-AI-5A67D8?style=for-the-badge&logo=anthropic" alt="Claude AI"/>
  <img src="https://img.shields.io/badge/Antigravity-Compatible-FF6B35?style=for-the-badge" alt="Antigravity"/>
  <img src="https://img.shields.io/badge/NoCode-Compatible-00D4AA?style=for-the-badge" alt="NoCode"/>
  <img src="https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown" alt="Markdown"/>
  <img src="https://img.shields.io/badge/Shields.io-badges-green?style=for-the-badge" alt="Shields.io"/>
</p>

---

## ✨ Características

| Característica | Descripción |
|---|---|
| 🎨 **Badges de color** | Genera badges personalizados con shields.io para version, licencia, estado, tecnologías |
| 🖼️ **Banner + Screenshots** | Incluye secciones para banner de proyecto y capturas de pantalla con placeholders |
| 🎬 **GIF Demo** | Instrucciones y herramientas para crear GIFs animados de demostración |
| 🏗️ **Estructura de proyecto** | Árbol de directorios y sección de arquitectura para proyectos complejos |
| 👥 **Sección de contribuidores** | Con avatares de GitHub enlazados automáticamente |
| 💰 **Donación XRP integrada** | Badge y dirección XRP de Oscar Omar Gómez Peña precargados |
| 🌐 **Multi-plataforma** | Compatible con Claude Code CLI, Antigravity y flujos NoCode |
| 📋 **Plantilla completa** | Todas las secciones estándar listas para copiar y adaptar |

---

## 🎬 Demo

<p align="center">
  <img src="https://via.placeholder.com/700x400?text=GIF+Demo+→+Invocar+skill+→+README+generado+en+segundos" alt="Demo animado" width="700"/>
</p>

**Flujo típico:**
1. Usuario: *"Crea el README para mi proyecto de API en FastAPI"*
2. El skill recopila: nombre, descripción, tecnologías, URL del repo
3. Output: `README.md` completo con badges, screenshots placeholder, secciones y contacto

---

## 🚀 Instalación

### Opción A — Claude Code (CLI)

```sh
git clone https://github.com/oscaromargp/readme-github-personalizado.git
cp readme-github-personalizado/SKILL.md ~/.claude/skills/readme-github-personalizado.md
```

El skill estará disponible en tu próxima sesión de Claude Code.

### Opción B — Antigravity

1. Descarga `SKILL.md` de este repositorio
2. En tu proyecto → **Skills → Importar skill**
3. Selecciona el archivo `SKILL.md`

### Opción C — NoCode

1. Agrega un nodo de tipo **Agente Claude**
2. Pega el contenido de `SKILL.md` en el campo de instrucciones
3. Conéctalo antes del nodo de push a GitHub

---

## 💡 Uso

Invoca el skill con cualquiera de estas frases:

```
"Crea el README para mi proyecto"
"Genera la documentación del repositorio"
"Hazlo más bonito con badges"
"Prepara el README antes de subir a GitHub"
"Documenta este repo con screenshots"
```

### Ejemplo de output generado

<p align="center">
  <img src="https://via.placeholder.com/680x200?text=Badges+→+Banner+→+Features+Table+→+Code+Block+→+XRP+Badge" alt="Secciones generadas" width="680"/>
</p>

```markdown
# Mi API REST

<img src="https://img.shields.io/badge/version-1.0.0-green?style=for-the-badge"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi"/>

## ✨ Características
| ⚡ Rápido | Respuestas < 50ms con async/await |
| 🔒 Seguro | JWT + OAuth2 integrado            |
...
```

---

## 📁 Archivos de este repositorio

```
readme-github-personalizado/
├── SKILL.md              # El skill — instrucciones para el agente IA
├── README.md             # Este archivo (generado con el propio skill)
├── LICENSE               # MIT License
├── assets/
│   ├── banner.png        # Banner del proyecto (agregar tu imagen)
│   ├── screenshot.png    # Captura de pantalla de ejemplo
│   └── IMAGES.md         # Guía de qué imágenes agregar y cómo
└── samples/
    ├── README-web-app.md     # README de ejemplo: aplicación web
    ├── README-cli-tool.md    # README de ejemplo: herramienta CLI
    └── README-nocode.md      # README de ejemplo: proyecto NoCode
```

---

## 🤝 Contribuyendo

¡Las contribuciones son bienvenidas! Si quieres mejorar la plantilla, añadir soporte para más tecnologías o traducirla:

1. Haz un fork: `gh repo fork oscaromargp/readme-github-personalizado`
2. Crea tu rama: `git checkout -b feature/mejora`
3. Commit: `git commit -m 'feat: mejora sección de badges'`
4. Push: `git push origin feature/mejora`
5. Abre un Pull Request

---

## 💖 Apoya este Proyecto

Si este skill te ha ahorrado tiempo o mejorado tus proyectos, considera hacer una contribución.

<p align="center">
  <strong>Donaciones en Criptomonedas — Red XRP</strong><br><br>
  <img src="https://img.shields.io/badge/XRP-rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj-00AAE4?style=for-the-badge&logo=ripple" alt="XRP Address"/>
</p>

> Dirección XRP: `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`

---

## 📄 Licencia

Distribuido bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más información.

---

## 📬 Contacto

<p align="center">
  <strong>Oscar Omar Gómez Peña</strong>
</p>

<p align="center">
  <a href="https://oscaromargp.github.io/Oscaromargp/">
    <img src="https://img.shields.io/badge/Portafolio-Web-blueviolet?style=for-the-badge&logo=github" alt="Portafolio"/>
  </a>
  &nbsp;
  <a href="https://github.com/oscaromargp">
    <img src="https://img.shields.io/badge/GitHub-oscaromargp-181717?style=for-the-badge&logo=github" alt="GitHub"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/oscaromargp/readme-github-personalizado">🔗 Ver este repositorio en GitHub</a>
</p>

---

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

- [matiassingers/awesome-readme](https://github.com/matiassingers/awesome-readme) — por la curaduría de los mejores READMEs del mundo
- [Shields.io](https://shields.io) — por los badges dinámicos
- [Anthropic / Claude](https://anthropic.com) — por el motor de IA
- [Antigravity](https://antigravity.ai) — por la plataforma de automatización
- [ScreenToGif](https://www.screentogif.com/) — herramienta recomendada para crear GIFs de demo


## 💬 Preguntas y Soporte

<p align="center">
  <a href="https://wa.me/526121077805?text=Hola%20Oscar%2C%20vi%20tu%20proyecto%20en%20GitHub%20y%20quisiera%20preguntarte...">
    <img src="https://img.shields.io/badge/WhatsApp-Contactar-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp"/>
  </a>
</p>

