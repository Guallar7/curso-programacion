---
theme: default
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Conceptos
  Deck basado en Borrador del curso.md.
drawings:
  persist: false
transition: slide-left
title: Conceptos
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

<div class="grid grid-cols-4 gap-3 mt-6 text-[10px] leading-tight">
  <a href="https://chatgpt.com/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/chatgpt-access.png'" class="h-34 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">ChatGPT</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://chatgpt.com/</span>
  </a>
  <a href="https://claude.ai/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/claude-access.png'" class="h-34 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Claude</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://claude.ai/</span>
  </a>
  <a href="https://gemini.google.com/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/gemini-access.png'" class="h-34 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Gemini</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://gemini.google.com/</span>
  </a>
  <a href="https://github.com/features/copilot" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/copilot-access.png'" class="h-34 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Copilot</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://github.com/features/copilot</span>
  </a>
</div>

---

# Prompt

Instrucciones que le damos al LLM para que genere código o texto.

---

# Token

<div class="grid grid-cols-5 gap-6 items-start mt-4">
  <div class="col-span-2">
    <p>Unidad mínima de texto que el LLM puede procesar.</p>
    <p>Como los morfemas que se estudiaban en lengua.</p>
    <a href="https://platform.openai.com/tokenizer" target="_blank" class="inline-block mt-6 px-5 py-3 rounded-lg text-inherit no-underline shadow-sm" style="border: 1px solid #d1d5db !important; outline: none !important; text-decoration: none !important;">OpenAI Tokenizer<br />https://platform.openai.com/tokenizer</a>
  </div>
  <a href="https://platform.openai.com/tokenizer" target="_blank" class="col-span-3 block text-inherit no-underline rounded-lg overflow-hidden shadow-sm bg-white" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;"><img :src="'./downloads/tokenizer-example.png'" style="height: 27rem; width: 100%; object-fit: contain; object-position: top; display: block;" /></a>
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

<div class="grid grid-cols-2 gap-4 mt-6 text-[10px] leading-tight">
  <a href="https://www.python.org/downloads/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/python-download.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Python</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://www.python.org/downloads/</span>
  </a>
  <a href="https://nodejs.org/en/download" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/nodejs-download.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Node.js</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://nodejs.org/en/download</span>
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

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://git-scm.com/downloads" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/git-download.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Git</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://git-scm.com/downloads</span>
  </a>
</div>

---

# GitHub

Repositorio online donde frecuentemente los programadores suben su contenido.

Puede contener proyectos públicos o privados.

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://github.com/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/github-access.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">GitHub</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://github.com/</span>
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

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://supabase.com/" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/supabase-access.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Supabase</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://supabase.com/</span>
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

Instrucciones o prompts preconfigurados que le dicen a Claude cómo comportarse en una tarea concreta.

Pueden ser simples instrucciones o comandos de programación concretos.

---

# Extensiones

Equivalente a las skills en Antigravity.

Permiten conectar Antigravity con otras herramientas.

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://antigravity.google/download" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/antigravity-download.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Antigravity</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://antigravity.google/download</span>
  </a>
</div>

---
layout: section
---

# EMPECEMOS A PROGRAMAR!

---

# Guallar7/app-builder

<a href="https://github.com/Guallar7/app-builder" target="_blank" class="block max-w-4xl mx-auto mt-5 text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left text-[10px]" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
  <img :src="'./downloads/app-builder-repo.png'" class="h-92 w-full object-cover object-top" />
  <strong class="block px-3 pt-2 text-sm">Guallar7/app-builder</strong>
  <span class="block px-3 pb-2 opacity-70 break-all">https://github.com/Guallar7/app-builder</span>
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

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://developers.google.com/apps-script" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/apps-script-access.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Apps Script</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://developers.google.com/apps-script</span>
  </a>
</div>

---

# Make

Ejemplo: buzón de sugerencias.

<div class="max-w-lg mx-auto mt-6 text-[10px] leading-tight">
  <a href="https://www.make.com/en/register" target="_blank" class="block text-inherit no-underline rounded-lg overflow-hidden bg-white shadow-sm text-left" style="border: 1px solid #e5e7eb !important; text-decoration: none !important; color: inherit !important;">
    <img :src="'./downloads/make-access.png'" class="h-40 w-full object-cover object-top" />
    <strong class="block px-3 pt-2 text-sm">Make</strong>
    <span class="block px-3 pb-2 opacity-70 break-all">https://www.make.com/en/register</span>
  </a>
</div>
