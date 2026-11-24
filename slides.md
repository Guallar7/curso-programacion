---
theme: default
layout: default
class: materials-slide
highlighter: shiki
lineNumbers: false
lang: es
favicon: ''
drawings:
  persist: false
transition: slide-left
title: Programación con IA para profesionales clínicos
titleTemplate: '%s'
seoMeta:
  ogDescription: Taller práctico para profesionales clínicos con David Guallar y Alejandro Venegas. Segunda edición, 24 de noviembre de 2026.
  ogUrl: https://guallar7.github.io/curso-programacion/
  ogImage: https://guallar7.github.io/curso-programacion/curso-ia-2026-og.jpg
themeConfig:
  primary: '#0f766e'
---

# Recibe los materiales del curso

<div class="materials-layout">
  <div>
    <p>Escanea el QR y <strong>envía el correo</strong> que se abre.</p>
    <p>Guardaremos tu dirección para enviarte el enlace a los materiales. La solicitud es voluntaria.</p>
  </div>
  <div class="materials-request">
    <img :src="'./solicitar-materiales-qr.png'" alt="Código QR para abrir el correo de solicitud de materiales" />
    <a href="mailto:davidguallargarcia@gmail.com?subject=MATERIALES%20PROGRAMACION%20IA%20SALUD%202026-11-24&amp;body=Quiero%20los%20materiales%20del%20curso%20de%20Programaci%C3%B3n%20con%20IA%20del%20SALUD.">Abrir correo</a>
  </div>
</div>

---
class: game-slide
---

# Un juego antes de empezar

<div class="game-links">
  <a href="https://salud-programacion-ia.vercel.app/" target="_blank" rel="noopener noreferrer" class="game-preview">
    <img :src="'./juego-salud-2026.jpg'" alt="Abrir el juego Menos tareas. Más ideas." />
    <span aria-hidden="true">Abrir el juego ↗</span>
  </a>
  <figure class="game-qr">
    <img :src="'./juego-salud-2026-qr.png'" alt="Código QR para abrir el juego" />
    <figcaption>Escanea con el móvil</figcaption>
  </figure>
</div>

24 de noviembre de 2026

---
routeAlias: como-funciona-el-juego
---

# ¿Cómo funciona el juego?

1. **Formulario web.** Envías una idea y tu correo. La web avisa a Make.
2. **Google Sheets.** Make registra la participación.
3. **IA.** Make pide a un modelo, a través de OpenRouter, que invente una solución imposible.
4. **Gmail.** Make te envía la respuesta por correo.

**Make encadena los pasos.** Más adelante veremos cómo un agente también puede usar herramientas de otros servicios mediante conectores.

<!--
Mostrar solo el recorrido de la idea. El formulario pasa por el servidor, que valida y registra la solicitud antes de avisar a Make. Para el ejemplo docente basta con seguir la idea hasta el correo.
-->

---
layout: cover
class: cover-slide
---

# Programación en Inteligencia Artificial y Aplicaciones Prácticas para Usuarios Avanzados

## David Guallar · Alejandro Venegas

Segunda edición · 24 de noviembre de 2026

---

# Índice

<nav class="index-list">
  <Link to="como-funciona-el-juego">Cómo funciona el juego</Link>
  <Link to="conceptos-base">Conceptos base</Link>
  <Link to="arquitectura-basica">Arquitectura muy básica</Link>
  <Link to="agentes-herramientas">Agentes, herramientas e integración</Link>
  <Link to="empecemos">EMPECEMOS A PROGRAMAR!</Link>
  <Link to="automatizaciones">Automatizaciones</Link>
</nav>

---

# Antes de empezar

- Tened a mano vuestro portátil y el cargador.
- Abrid la aplicación de IA que hayáis elegido (Codex, Claude o Antigravity) y comprobad que habéis iniciado sesión.
- Si habéis instalado Node.js, Python y Git, comprobad que responden en la terminal.<br>
  `node --version`, `python --version` (o `python3 --version`) y `git --version`.
- Comprobad que podéis acceder a vuestra cuenta de GitHub.

---
layout: section
routeAlias: conceptos-base
---

# Conceptos base

---

# LLM

Modelo de Lenguaje Grande.

Modelo entrenado con una cantidad masiva de datos que trabaja prediciendo el siguiente token.

---

# Modelos mencionados

<div class="tool-grid cols-4">
  <a href="https://chatgpt.com/" target="_blank" class="tool-card">
    <img :src="'./downloads/chatgpt-access.png'" />
    <strong>ChatGPT</strong>
    <span>https://chatgpt.com/</span>
  </a>
  <a href="https://claude.ai/" target="_blank" class="tool-card">
    <img :src="'./downloads/claude-access.png'" />
    <strong>Claude</strong>
    <span>https://claude.ai/</span>
  </a>
  <a href="https://gemini.google.com/" target="_blank" class="tool-card">
    <img :src="'./downloads/gemini-access.png'" />
    <strong>Gemini</strong>
    <span>https://gemini.google.com/</span>
  </a>
  <a href="https://copilot.microsoft.com/" target="_blank" class="tool-card">
    <img :src="'./downloads/copilot-access.png'" />
    <strong>Copilot</strong>
    <span>https://copilot.microsoft.com/</span>
  </a>
</div>

---

# Prompt

Instrucciones que le damos al LLM para que genere código o texto.

---

# Token

<div class="token-layout">
  <div class="token-copy">
    <p>Unidad mínima de texto que el LLM puede procesar.</p>
    <p>Como los morfemas que se estudiaban en lengua.</p>
    <a href="https://platform.openai.com/tokenizer" target="_blank" class="token-link">OpenAI Tokenizer<span>https://platform.openai.com/tokenizer</span></a>
  </div>
  <a href="https://platform.openai.com/tokenizer" target="_blank" class="token-shot"><img :src="'./downloads/tokenizer-example.png'" /></a>
</div>

---

# Ventana de contexto

Cantidad de tokens que el LLM puede procesar en un momento dado.

Para entendernos: la memoria activa de trabajo por sesión.

---

# Lenguaje de programación

Lenguaje formal que permite especificar instrucciones que serán ejecutadas por un computador.

Es como un idioma que el computador entiende.

---

# Lenguajes

Python es uno de los lenguajes mencionados en el borrador.

JavaScript puede usarse en backend con Node.js.

<div class="tool-grid cols-2">
  <a href="https://www.python.org/downloads/" target="_blank" class="tool-card">
    <img :src="'./downloads/python-download.png'" />
    <strong>Python</strong>
    <span>https://www.python.org/downloads/</span>
  </a>
  <a href="https://nodejs.org/en/download" target="_blank" class="tool-card">
    <img :src="'./downloads/nodejs-download.png'" />
    <strong>Node.js</strong>
    <span>https://nodejs.org/en/download</span>
  </a>
</div>

---

# IDE

Entorno de Desarrollo Integrado.

Programa informático utilizado para la creación y modificación de software: el Word que se utiliza para programar.

---

# Git

Programa gratuito diseñado para el control de versiones de software.

Actúa en local.

<div class="single-tool">
  <a href="https://git-scm.com/downloads" target="_blank" class="tool-card">
    <img :src="'./downloads/git-download.png'" />
    <strong>Git</strong>
    <span>https://git-scm.com/downloads</span>
  </a>
</div>

---

# GitHub

Repositorio online donde frecuentemente los programadores suben su contenido.

Puede contener proyectos públicos o privados.

<div class="single-tool">
  <a href="https://github.com/" target="_blank" class="tool-card">
    <img :src="'./downloads/github-access.png'" />
    <strong>GitHub</strong>
    <span>https://github.com/</span>
  </a>
</div>

---
layout: section
routeAlias: arquitectura-basica
---

# Arquitectura muy básica

---

# Frontend

Interfaz.

Es lo que se ve de los programas.

---

# Backend

Servidor o centro del programa.

Alberga su función propiamente dicha.

---

# Base de datos

Archivos en los que se almacena información.

Clave para programas que requieren recordar información de una sesión a otra.

<div class="single-tool">
  <a href="https://supabase.com/" target="_blank" class="tool-card">
    <img :src="'./downloads/supabase-access.png'" />
    <strong>Supabase</strong>
    <span>https://supabase.com/</span>
  </a>
</div>

---
layout: section
routeAlias: agentes-herramientas
---

# Agentes, herramientas e integración

---

# MCP

Model Context Protocol.

Protocolos que definen cómo un LLM puede exponer y usar herramientas externas.

---

# Skills

Instrucciones reutilizables en una carpeta con `SKILL.md`.

Preparan al agente para una tarea concreta.

<table class="skills-table">
  <thead>
    <tr>
      <th>Entorno</th>
      <th>Documentación</th>
      <th>Carpeta</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>OpenAI Codex</td>
      <td><a href="https://developers.openai.com/codex/skills" target="_blank">developers.openai.com/codex/skills</a></td>
      <td><code>~/.agents/skills</code><br><code>.agents/skills</code></td>
    </tr>
    <tr>
      <td>Claude Code</td>
      <td><a href="https://docs.claude.com/en/docs/claude-code/skills" target="_blank">docs.claude.com/.../skills</a></td>
      <td><code>~/.claude/skills</code><br><code>.claude/skills</code></td>
    </tr>
    <tr>
      <td>Antigravity</td>
      <td><a href="https://antigravity.google/docs/skills" target="_blank">antigravity.google/docs/skills</a></td>
      <td><code>~/.gemini/antigravity/skills</code><br><code>.agents/skills</code></td>
    </tr>
  </tbody>
</table>

<p class="small-reference">
  Ejemplo: <a href="https://www.aitmpl.com/" target="_blank">aitmpl.com</a>
</p>

---
routeAlias: conectores
---

# Conectores y MCP

Codex, Claude Code y Antigravity pueden usar **MCP** para acceder a herramientas de otros servicios.

<img class="connector-diagram" :src="'./conectores-mcp.png'" alt="Ejemplo con Codex. A través de MCP, el agente intercambia llamadas y resultados con herramientas de GitHub, Supabase y Figma." />

---

# Plugins · conector ± skills

- **Conector.** Da acceso al servicio. Por ejemplo, GitHub permite leer incidencias.
- **Skill.** Aporta instrucciones reutilizables. Por ejemplo, cómo priorizar esas incidencias y redactar un resumen.
- **Plugin.** Es un paquete instalable. En Codex y Claude Code puede incluir un conector, skills o ambos.

<!--
Fórmula para explicarlo en clase: «conector con o sin skills» cuando el plugin conecta con un servicio. También hay plugins que solo aportan skills. El esquema anterior muestra Codex como ejemplo de MCP.
Referencias: https://developers.openai.com/plugins/concepts/plugins · https://code.claude.com/docs/en/plugins · https://antigravity.google/docs/mcp
-->

---
layout: section
routeAlias: empecemos
---

# EMPECEMOS A PROGRAMAR!

---

# Guallar7/app-builder

<a href="https://github.com/Guallar7/app-builder" target="_blank" class="repo-card">
  <img :src="'./downloads/app-builder-repo.png'" />
  <strong>Guallar7/app-builder</strong>
  <span>https://github.com/Guallar7/app-builder</span>
</a>

---
layout: section
routeAlias: automatizaciones
---

# Automatizaciones

---

# Automatizaciones

---

# Apps Script

Ejemplo: formulario satisfacción de consulta.

<div class="apps-script-layout">
  <div class="single-tool">
    <a href="https://developers.google.com/apps-script" target="_blank" class="tool-card">
      <img :src="'./downloads/apps-script-access.png'" />
      <strong>Apps Script</strong>
      <span>https://developers.google.com/apps-script</span>
    </a>
  </div>
  <a href="https://drive.google.com/drive/folders/1l-qomm67lEX2cHuFzYmDMTztf0rkCPtb" target="_blank" class="qr-card">
    <img src="./QR-apps-script.png" alt="QR material Apps Script" />
    <span>Material de apoyo</span>
  </a>
</div>

---

# Make

Ejemplo: buzón de sugerencias.

<div class="single-tool">
  <a href="https://www.make.com/en/register" target="_blank" class="tool-card">
    <img :src="'./downloads/make-access.png'" />
    <strong>Make</strong>
    <span>https://www.make.com/en/register</span>
  </a>
</div>
