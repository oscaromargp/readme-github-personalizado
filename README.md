# readme-github-personalizado

Skill para Claude, Antigravity y NoCode que genera automáticamente un README profesional y completo para cualquier repositorio de GitHub, con la plantilla personalizada de Oscar Omar Gómez Peña.

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

Este repositorio contiene el skill `readme-github-personalizado`, una instrucción estructurada para agentes de IA (Claude, Antigravity, NoCode) que genera READMEs de calidad profesional de forma automática.

El skill resuelve el problema habitual de llegar a GitHub con un repositorio vacío de documentación o con un README genérico. Basta con invocar el skill y proporcionar los datos básicos del proyecto; el agente produce un archivo `README.md` completo, con todas las secciones estándar, ejemplos de código, información de contacto y dirección de donación XRP.

### Construido Con

- [Claude Code](https://claude.ai/code) — Motor de IA para ejecutar el skill
- [Antigravity](https://antigravity.ai) — Plataforma de automatización compatible
- [NoCode](https://nocode.com) — Flujos visuales donde el skill actúa como nodo de documentación
- Markdown — Formato de salida universal para GitHub

## Comenzando

### Prerrequisitos

Necesitas **una** de las siguientes plataformas:

| Plataforma | Versión mínima |
|------------|---------------|
| Claude Code (CLI) | Cualquiera con soporte de skills |
| Antigravity | Compatible con skills `.skill` |
| NoCode | Nodo de agente Claude activo |

### Instalación

#### Opción A — Claude Code (CLI)

1. Clona este repositorio
   ```sh
   git clone https://github.com/oscaromargp/readme-github-personalizado.git
   ```
2. Copia el archivo del skill a tu directorio de skills local
   ```sh
   cp readme-github-personalizado/SKILL.md ~/.claude/skills/readme-github-personalizado.md
   ```
3. El skill estará disponible en tu próxima sesión de Claude Code.

#### Opción B — Antigravity

1. Descarga `SKILL.md` de este repositorio.
2. En tu proyecto de Antigravity, ve a **Skills → Importar skill**.
3. Selecciona el archivo `SKILL.md` descargado.
4. El skill aparecerá en tu biblioteca con el nombre `readme-github-personalizado`.

#### Opción C — NoCode

1. En tu flujo NoCode, agrega un nodo de tipo **Agente Claude**.
2. En el campo de instrucciones del nodo, copia y pega el contenido de `SKILL.md`.
3. Conecta el nodo antes del paso de push a GitHub.

## Uso

Una vez instalado, invoca el skill con cualquiera de estas frases:

```
"Crea el README para mi proyecto"
"Genera la documentación del repositorio"
"Prepara el README antes de subir a GitHub"
"Documenta este repo"
```

El agente te pedirá:
- Nombre del proyecto
- Descripción breve
- Tecnologías usadas
- Pasos de instalación y uso

Y producirá el archivo `README.md` listo para commit.

**Ejemplo de salida (fragmento):**

```markdown
# MiProyecto

Aplicación web para gestionar tareas de equipo en tiempo real.

## Construido Con
- [Next.js](https://nextjs.org/)
- [Supabase](https://supabase.com/)
...
```

## Contribuyendo

¡Las contribuciones son bienvenidas! Si quieres mejorar la plantilla, agregar soporte para más secciones o traducirla a otro idioma:

1. Haz un fork del repositorio
2. Crea tu rama (`git checkout -b feature/mejora-plantilla`)
3. Haz commit de tus cambios (`git commit -m 'feat: agrega sección de screenshots'`)
4. Push a la rama (`git push origin feature/mejora-plantilla`)
5. Abre un Pull Request

## Apoya este Proyecto

Si este skill te ha ahorrado tiempo o mejorado tus proyectos, considera hacer una contribución. Esto me ayuda a seguir creando y manteniendo herramientas de código abierto.

**Donaciones en Criptomonedas (Red XRP):**

> Dirección XRP: `rBthUCndKy3Xbb19Ln4xkZeMwusX9NrYfj`

¡Muchas gracias por tu apoyo!

## Licencia

Distribuido bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más información.

## Contacto

**Oscar Omar Gómez Peña**

- Portafolio Web: [oscaromargp.github.io/Oscaromargp/](https://oscaromargp.github.io/Oscaromargp/)
- GitHub: [@oscaromargp](https://github.com/oscaromargp)
- Enlace al proyecto: [https://github.com/oscaromargp/readme-github-personalizado](https://github.com/oscaromargp/readme-github-personalizado)

## Agradecimientos

- [Anthropic / Claude](https://anthropic.com) — Por el motor de IA que ejecuta el skill
- [Antigravity](https://antigravity.ai) — Por la plataforma de automatización
- [Shields.io](https://shields.io) — Para futuras insignias en READMEs
- Comunidad de código abierto de GitHub — Por la inspiración en buenas prácticas de documentación
