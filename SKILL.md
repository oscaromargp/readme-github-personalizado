---
name: readme-github-personalizado
description: >
  Utiliza este skill SIEMPRE que necesites crear o actualizar un README.md para cualquier proyecto en GitHub.
  Genera READMEs profesionales y visualmente atractivos con badges de color, banners, capturas de pantalla,
  GIFs demo, secciones de características con íconos, tablas, y archivos de muestra.
  Se activa cuando el usuario menciona: crear README, documentar un repositorio, subir proyecto a GitHub,
  generar documentación, preparar repo para publicar, hacer el README bonito, agregar badges.
  Compatible con Claude Code, Antigravity y NoCode. Incluye datos de contacto y donación XRP de Oscar Omar Gómez Peña.
compatibility:
  - claude
  - antigravity
  - nocode
---

# Skill: README GitHub Personalizado

Genera READMEs profesionales, visualmente atractivos y completos, siguiendo los patrones de los mejores proyectos open source del mundo (referencia: [awesome-readme](https://github.com/matiassingers/awesome-readme)).

---

## Cuándo usar este skill

- Al crear un nuevo repositorio en GitHub
- Al subir un proyecto existente
- Al actualizar la documentación de un repo
- Cuando el usuario pida: "crea el README", "documenta mi repo", "hazlo más bonito", "agrega badges", "prepara para GitHub"
- En flujos Antigravity o NoCode como nodo previo al push a GitHub

---

## Elementos visuales obligatorios

Todo README generado con este skill DEBE incluir estos elementos visuales. Explica al usuario cómo obtener cada uno:

### 1. Banner / Header visual

```html
<p align="center">
  <img src="assets/banner.png" alt="Banner del proyecto" width="100%"/>
</p>
```

> Si el usuario no tiene un banner, sugiere crearlo gratis en [Canva](https://canva.com) o [carbon.now.sh](https://carbon.now.sh) para código.

### 2. Badges de color (shields.io)

Siempre incluir un bloque de badges centrado bajo el título. Adapta según el proyecto:

```html
<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/version-1.0.0-green?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/PRs-welcome-orange?style=for-the-badge" alt="PRs Welcome"/>
  <img src="https://img.shields.io/badge/made%20with-❤️-red?style=for-the-badge" alt="Made with love"/>
</p>
```

**Badges útiles por tipo de proyecto:**

| Tipo de proyecto | Badges recomendados |
|---|---|
| Web / Frontend | version, license, deploy status, npm downloads |
| API / Backend | build status, coverage, docker pulls, license |
| CLI tool | npm/pip installs, platform support, license |
| NoCode / Automation | status, compatible platforms, license |
| Librería | version, downloads semanales, size, license |

Genera las URLs de shields.io con este patrón:
```
https://img.shields.io/badge/<LABEL>-<MESSAGE>-<COLOR>?style=for-the-badge&logo=<LOGO>
```

Colores disponibles: `brightgreen`, `green`, `yellowgreen`, `yellow`, `orange`, `red`, `blue`, `lightgrey`, `blueviolet`

Logos disponibles (parámetro `logo=`): `github`, `npm`, `python`, `react`, `node.js`, `docker`, `supabase`, `vercel`, `javascript`, `typescript`, etc.

### 3. Demo visual (screenshot o GIF)

```html
<p align="center">
  <img src="assets/demo.gif" alt="Demo del proyecto" width="700"/>
</p>
```

o para screenshots estáticos:

```html
<p align="center">
  <img src="assets/screenshot.png" alt="Captura de pantalla" width="700"/>
</p>
```

> Si el usuario no tiene imágenes aún, usa placeholders de [via.placeholder.com](https://via.placeholder.com):
> ```html
> <img src="https://via.placeholder.com/700x400?text=Demo+Screenshot" alt="Demo" width="700"/>
> ```

**Herramientas para crear GIFs:**
- [ScreenToGif](https://www.screentogif.com/) — Gratis, Windows
- [Gifski](https://gif.ski/) — Alta calidad
- [LICEcap](https://www.cockos.com/licecap/) — Gratis, simple

### 4. Tabla de características con íconos

```markdown
## ✨ Características

| Característica | Descripción |
|---|---|
| ⚡ Rápido | Procesamiento en menos de 100ms |
| 🔒 Seguro | Autenticación JWT y cifrado AES-256 |
| 🌐 Multilenguaje | Soporte para ES, EN, FR |
| 📱 Responsivo | Diseño adaptable a todos los dispositivos |
| 🔌 Extensible | Sistema de plugins modular |
```

### 5. Sección de arquitectura (proyectos complejos)

```markdown
## 🏗️ Arquitectura

<p align="center">
  <img src="assets/architecture.png" alt="Diagrama de arquitectura" width="700"/>
</p>

### Estructura del proyecto

\```
mi-proyecto/
├── src/
│   ├── components/     # Componentes reutilizables
│   ├── pages/          # Páginas / rutas
│   ├── services/       # Lógica de negocio
│   └── utils/          # Helpers y utilidades
├── public/             # Assets estáticos
├── tests/              # Tests unitarios e integración
└── docs/               # Documentación adicional
\```
```

### 6. Sección de contribuidores con avatares

```html
## 👥 Contribuidores

<a href="https://github.com/oscaromargp">
  <img src="https://github.com/oscaromargp.png" width="50" style="border-radius:50%" alt="oscaromargp"/>
</a>
```

---

## Proceso de generación

1. **Recopila información** — Pregunta al usuario:
   - Nombre y descripción del proyecto
   - Tecnologías usadas
   - ¿Tiene logo, banner o screenshots? (si no, usa placeholders)
   - ¿Es web, CLI, librería, API, NoCode?
   - URL del repo: `https://github.com/oscaromargp/<repo>`

2. **Selecciona badges relevantes** para el tipo de proyecto

3. **Genera el README completo** usando la plantilla oficial abajo

4. **Crea la carpeta `assets/`** con un archivo `IMAGES.md` que explique qué imágenes agregar

5. **Confirma** con el usuario antes de hacer commit

---

## Plantilla oficial completa

Usa exactamente este formato, adaptando los campos `< >` al proyecto real:

````markdown
<p align="center">
  <img src="assets/banner.png" alt="<Nombre del Proyecto>" width="100%"/>
</p>

<h1 align="center"><Nombre del Proyecto></h1>

<p align="center">
  <strong><Descripción corta: qué hace y para quién es></strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/version-1.0.0-green?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/PRs-welcome-orange?style=for-the-badge" alt="PRs"/>
</p>

<p align="center">
  <a href="#-acerca-del-proyecto">Acerca</a> •
  <a href="#-características">Características</a> •
  <a href="#-demo">Demo</a> •
  <a href="#-comenzando">Comenzando</a> •
  <a href="#-uso">Uso</a> •
  <a href="#-contacto">Contacto</a>
</p>

---

## 📖 Acerca del Proyecto

<p align="center">
  <img src="assets/screenshot.png" alt="Captura de pantalla principal" width="700"/>
</p>

<Descripción detallada: problema que resuelve, tecnologías clave, público objetivo.>

### 🛠️ Construido Con

<p align="left">
  <img src="https://img.shields.io/badge/<Tech1>-<Color>?style=for-the-badge&logo=<logo1>" alt="<Tech1>"/>
  <img src="https://img.shields.io/badge/<Tech2>-<Color>?style=for-the-badge&logo=<logo2>" alt="<Tech2>"/>
</p>

---

## ✨ Características

| Característica | Descripción |
|---|---|
| ⚡ <Feature 1> | <Descripción breve> |
| 🔒 <Feature 2> | <Descripción breve> |
| 🌐 <Feature 3> | <Descripción breve> |
| 📱 <Feature 4> | <Descripción breve> |

---

## 🎬 Demo

<p align="center">
  <img src="assets/demo.gif" alt="Demo animado" width="700"/>
</p>

> ¿No puedes ver el GIF? [Haz clic aquí para ver el demo en video](https://github.com/oscaromargp/<repo>)

---

## 🚀 Comenzando

### Prerrequisitos

- <Prerequisito 1> — [Cómo instalarlo](<link>)
- <Prerequisito 2> — versión `>= X.X`

### Instalación

1. Clona el repositorio
   ```sh
   git clone https://github.com/oscaromargp/<repo>.git
   cd <repo>
   ```

2. Instala las dependencias
   ```sh
   npm install
   # o
   pip install -r requirements.txt
   ```

3. Configura las variables de entorno
   ```sh
   cp .env.example .env
   # Edita .env con tus valores
   ```

4. Inicia el proyecto
   ```sh
   npm run dev
   ```

---

## 💡 Uso

### Ejemplo básico

```<lenguaje>
// Ejemplo de código real del proyecto
const resultado = miProyecto.ejecutar({ opcion: 'valor' });
console.log(resultado);
```

### Capturas de pantalla adicionales

<p align="center">
  <img src="assets/screenshot-2.png" alt="Funcionalidad X" width="45%"/>
  &nbsp;&nbsp;
  <img src="assets/screenshot-3.png" alt="Funcionalidad Y" width="45%"/>
</p>

---

## 🤝 Contribuyendo

¡Las contribuciones son bienvenidas! Por favor lee las [guías de contribución](CONTRIBUTING.md).

1. Haz un fork del repositorio
2. Crea tu rama: `git checkout -b feature/nueva-funcionalidad`
3. Haz commit: `git commit -m 'feat: agrega nueva funcionalidad'`
4. Push: `git push origin feature/nueva-funcionalidad`
5. Abre un Pull Request

---

## 💖 Apoya este Proyecto

Si este proyecto te fue útil, considera hacer una contribución. Esto me ayuda a seguir creando herramientas de código abierto.

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
  <a href="https://github.com/oscaromargp/<repo>">Ver Repositorio</a>
</p>

---

## 🙏 Agradecimientos

- <Persona o proyecto 1> — por <razón>
- [Shields.io](https://shields.io) — por los badges
- [awesome-readme](https://github.com/matiassingers/awesome-readme) — por la inspiración
````

---

## Notas de implementación

- **Datos fijos** — Nunca cambiar: XRP `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`, GitHub `@oscaromargp`, portafolio `https://oscaromargp.github.io/Oscaromargp/`
- **Idioma** — Español por defecto, a menos que el usuario pida otro
- **Imágenes** — Si el usuario no tiene, usa placeholders de `via.placeholder.com` y crea `assets/IMAGES.md` explicando qué agregar
- **Badges** — Siempre generar con `style=for-the-badge` para mejor visual
- **Antigravity / NoCode** — Insertar este skill como nodo previo al nodo de push a GitHub; el output es el archivo `README.md`
