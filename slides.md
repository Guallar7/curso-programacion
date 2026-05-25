---
theme: default
layout: cover
class: cover-slide
highlighter: shiki
lineNumbers: false
info: |
  ## Conceptos
  Deck basado en Borrador del curso.md.
drawings:
  persist: false
transition: slide-left
title: Conceptos
themeConfig:
  primary: '#0f766e'
---

# Conceptos

## Borrador del curso

Alex · David

---
layout: section
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

---
layout: section
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
---

# Automatizaciones

---

# Automatizaciones

Sólo si sobra tiempo.

---

# Apps Script

Ejemplo: formulario satisfacción de consulta.

<div class="single-tool">
  <a href="https://developers.google.com/apps-script" target="_blank" class="tool-card">
    <img :src="'./downloads/apps-script-access.png'" />
    <strong>Apps Script</strong>
    <span>https://developers.google.com/apps-script</span>
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
