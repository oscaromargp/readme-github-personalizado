<p align="center">
  <img src="../assets/banner.png" alt="MiApp Web" width="100%"/>
</p>

<h1 align="center">MiApp Web</h1>

<p align="center">
  <strong>Plataforma web para gestionar tareas de equipo en tiempo real, con notificaciones y colaboración en vivo.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/version-1.2.0-green?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/deploy-Vercel-000000?style=for-the-badge&logo=vercel" alt="Vercel"/>
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
  <img src="https://via.placeholder.com/700x380?text=Dashboard+de+Tareas+en+Tiempo+Real" alt="Screenshot principal" width="700"/>
</p>

MiApp Web resuelve el caos de los equipos remotos: centraliza tareas, asignaciones y comentarios en un solo lugar con actualizaciones en tiempo real. Sin recargar la página, sin emails de seguimiento.

### 🛠️ Construido Con

<p align="left">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js" alt="Next.js"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase" alt="Supabase"/>
  <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss" alt="Tailwind"/>
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel" alt="Vercel"/>
</p>

---

## ✨ Características

| Característica | Descripción |
|---|---|
| ⚡ **Tiempo real** | Actualizaciones instantáneas con Supabase Realtime |
| 🔒 **Autenticación** | Login con Google, GitHub y email/password |
| 📋 **Tableros Kanban** | Arrastra y suelta tareas entre columnas |
| 👥 **Colaboración** | Asigna tareas, menciona compañeros con @usuario |
| 📱 **Responsivo** | Funciona perfecto en móvil, tablet y escritorio |
| 🔔 **Notificaciones** | Alertas en tiempo real para menciones y vencimientos |

---

## 🎬 Demo

<p align="center">
  <img src="https://via.placeholder.com/700x400?text=GIF+→+Crear+tarea+→+Asignar+→+Mover+columna" alt="Demo animado" width="700"/>
</p>

🌐 [Ver demo en vivo](https://miapp-demo.vercel.app)

---

## 🚀 Comenzando

### Prerrequisitos

- Node.js `>= 18.0`
- Cuenta en [Supabase](https://supabase.com) (gratis)

### Instalación

```sh
git clone https://github.com/oscaromargp/miapp-web.git
cd miapp-web
npm install
cp .env.example .env.local
# Agrega tus credenciales de Supabase en .env.local
npm run dev
```

Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

---

## 💡 Uso

### Crear una tarea

```ts
const tarea = await crearTarea({
  titulo: "Diseñar nueva landing page",
  asignadoA: "usuario@ejemplo.com",
  prioridad: "alta",
  fechaVencimiento: "2026-05-01"
});
```

<p align="center">
  <img src="https://via.placeholder.com/340x220?text=Vista+de+tablero" alt="Tablero" width="45%"/>
  &nbsp;&nbsp;
  <img src="https://via.placeholder.com/340x220?text=Vista+de+lista" alt="Lista" width="45%"/>
</p>

---

## 💖 Apoya este Proyecto

<p align="center">
  <img src="https://img.shields.io/badge/XRP-rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj-00AAE4?style=for-the-badge&logo=ripple" alt="XRP"/>
</p>

> Dirección XRP: `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`

---

## 📬 Contacto

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
