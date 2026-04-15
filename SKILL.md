---
name: readme-github-personalizado
description: >
  Utiliza este skill SIEMPRE que necesites crear o actualizar un archivo README.md para cualquier proyecto en GitHub.
  Se activa cuando el usuario menciona: crear README, documentar un repositorio, subir un proyecto a GitHub, generar documentación de proyecto, o cualquier tarea que implique describir un repo para GitHub.
  Este skill genera un README profesional, informativo y fácil de leer con las secciones principales que todo proyecto debe incluir, adaptado con los datos de Oscar Omar Gómez Peña (XRP, portafolio, contacto).
  Compatible con flujos de trabajo en Antigravity, NoCode y Claude Code.
compatibility:
  - claude
  - antigravity
  - nocode
---

# Skill: README GitHub Personalizado

Genera READMEs profesionales y completos para repositorios de GitHub, aplicando la plantilla personalizada de Oscar Omar Gómez Peña.

## Cuándo usar este skill

- Al crear un nuevo repositorio en GitHub
- Al subir un proyecto existente a GitHub
- Al actualizar la documentación de un repositorio
- Cuando el usuario pida "crear README", "documentar mi repo", "preparar el proyecto para GitHub"
- En cualquier flujo NoCode o Antigravity que incluya un paso de publicación en GitHub

## Proceso

1. **Recopila información del proyecto** — Pregunta al usuario:
   - Nombre del proyecto
   - Descripción breve (qué hace, qué problema resuelve)
   - Tecnologías / frameworks utilizados
   - Pasos de instalación y uso
   - URL del repositorio (formato: `https://github.com/oscaromargp/<repo>`)

2. **Genera el README** usando la plantilla oficial abajo.

3. **Escribe el archivo** como `README.md` en la raíz del repositorio.

4. **Confirma** con el usuario que el contenido es correcto antes de hacer commit o push.

---

## Plantilla oficial

Usa exactamente este formato, sustituyendo los campos entre `< >` con la información real del proyecto:

```markdown
# <Nombre del Proyecto>

<Descripción breve: qué hace el proyecto y qué problema resuelve, en 2-3 frases.>

## Tabla de Contenidos

- [Acerca del Proyecto](#acerca-del-proyecto)
- [Comenzando](#comenzando)
  - [Prerrequisitos](#prerrequisitos)
  - [Instalación](#instalación)
- [Uso](#uso)
- [Contribuyendo](#contribuyendo)
- [Apoya este Proyecto](#apoya-este-proyecto)
- [Licencia](#licencia)
- [Contacto](#contacto)
- [Agradecimientos](#agradecimientos)

## Acerca del Proyecto

<Descripción detallada: problema que resuelve, decisiones de diseño, público objetivo.>

### Construido Con

<Lista de tecnologías principales con links oficiales. Ejemplo:>

- [React](https://reactjs.org/)
- [Node.js](https://nodejs.org/)
- [Supabase](https://supabase.com/)

## Comenzando

Sigue estos pasos para tener una copia local funcionando.

### Prerrequisitos

<Lista de dependencias necesarias y cómo instalarlas.>

### Instalación

1. Clona el repositorio
   ```sh
   git clone https://github.com/oscaromargp/<repo>.git
   ```
2. Instala las dependencias
   ```sh
   npm install
   ```
3. Configura las variables de entorno en `.env`

## Uso

<Instrucciones de uso con ejemplos de código, capturas de pantalla o GIFs.>

```<lenguaje>
// Ejemplo de uso
```

## Contribuyendo

Las contribuciones son bienvenidas. Por favor:

1. Haz un fork del repositorio
2. Crea tu rama (`git checkout -b feature/nueva-funcionalidad`)
3. Haz commit de tus cambios (`git commit -m 'feat: agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## Apoya este Proyecto

Si este proyecto te ha sido útil, considera hacer una contribución. Esto me ayuda a seguir creando y manteniendo herramientas de código abierto.

**Donaciones en Criptomonedas (Red XRP):**

> Dirección XRP: `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`

¡Muchas gracias por tu apoyo!

## Licencia

Distribuido bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más información.

## Contacto

**Oscar Omar Gómez Peña**

- Portafolio Web: [oscaromargp.github.io/Oscaromargp/](https://oscaromargp.github.io/Oscaromargp/)
- GitHub: [@oscaromargp](https://github.com/oscaromargp)
- Enlace al proyecto: [https://github.com/oscaromargp/<repo>](https://github.com/oscaromargp/<repo>)

## Agradecimientos

<Lista de personas, proyectos o recursos que inspiraron o ayudaron al proyecto.>
```

---

## Notas importantes

- **Siempre usa la dirección XRP exacta:** `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`
- **Siempre usa el usuario de GitHub:** `@oscaromargp`
- **Siempre enlaza al portafolio:** `https://oscaromargp.github.io/Oscaromargp/`
- El README debe escribirse en **español** salvo que el usuario pida otro idioma
- Si el proyecto no tiene cierta sección (ej. no hay agradecimientos), omítela o usa un placeholder claro
- En flujos Antigravity o NoCode, aplica este skill como paso previo al nodo de push a GitHub
