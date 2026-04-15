<h1 align="center">
  <img src="https://via.placeholder.com/80x80?text=CLI" alt="logo" width="80"/><br/>
  mi-cli-tool
</h1>

<p align="center">
  <strong>Herramienta de línea de comandos para automatizar el scaffolding de proyectos Node.js con estructura opinada y lista para producción.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/npm-v1.0.0-red?style=for-the-badge&logo=npm" alt="npm"/>
  <img src="https://img.shields.io/badge/node-%3E%3D18-339933?style=for-the-badge&logo=node.js" alt="Node"/>
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/platform-win%20%7C%20mac%20%7C%20linux-lightgrey?style=for-the-badge" alt="Platform"/>
</p>

---

## 🎬 Demo

<p align="center">
  <img src="https://via.placeholder.com/700x350?text=GIF+→+npx+mi-cli-tool+new+mi-proyecto+→+Estructura+generada" alt="Demo CLI" width="700"/>
</p>

---

## ⚡ Instalación rápida

```sh
npm install -g mi-cli-tool
# o sin instalar:
npx mi-cli-tool new mi-proyecto
```

---

## 💡 Uso

```sh
# Crear nuevo proyecto
mi-cli-tool new <nombre>

# Agregar módulo
mi-cli-tool add auth
mi-cli-tool add database --type postgres

# Ver ayuda
mi-cli-tool --help
```

### Output esperado

```
✔ Creando estructura del proyecto...
✔ Instalando dependencias...
✔ Configurando ESLint y Prettier...
✔ Inicializando git...

🎉 Proyecto "mi-proyecto" listo en 12s
   cd mi-proyecto && npm run dev
```

---

## 🏗️ Estructura generada

```
mi-proyecto/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── index.ts
├── tests/
├── .env.example
├── .eslintrc.js
├── package.json
└── README.md
```

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
    <img src="https://img.shields.io/badge/Portafolio-blueviolet?style=for-the-badge&logo=github" alt="Portafolio"/>
  </a>
  &nbsp;
  <a href="https://github.com/oscaromargp">
    <img src="https://img.shields.io/badge/GitHub-oscaromargp-181717?style=for-the-badge&logo=github" alt="GitHub"/>
  </a>
</p>

## 📄 Licencia

MIT © [Oscar Omar Gómez Peña](https://github.com/oscaromargp)
