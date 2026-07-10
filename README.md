# 📷 Plan de Estudios · Fotografía de Eventos (La Belle Joie)

Web de capacitación interna para el equipo: bodas, 15 años y celebraciones sociales. Plan de 12 semanas (teoría + ejercicio práctico + chequeo rápido por módulo) más un cuestionario de evaluación final.

---

## 🗂 Contenido

| Archivo | Qué es |
|---|---|
| `index.html` | Plan de estudios completo — 12 módulos semanales, cronograma, progreso guardado por navegador |
| `cuestionario-fotografia.html` | Evaluación final — 8 ejes, preguntas abiertas, multiple choice y diagnóstico |
| `vercel.json` | Configuración de despliegue (home = plan de estudios, `/evaluacion` = cuestionario) |

## 🗓 Módulos del plan de estudios

1. Mentalidad del Fotógrafo Social
2. Cámara y Triángulo de Exposición
3. Ópticas Fotográficas
4. La Luz
5. Flash e Iluminación Artificial
6. Foco y Nitidez
7. Composición Funcional
8. Dirección de Modelos y Poses
9. Narrativa y Momentos Clave
10. Trato con Clientes y Equipo
11. Criterio Profesional, Edición y Entrega
12. Logística, Kit de Trabajo y Diagnóstico Final

---

## 🚀 Cómo usar

### Opción 1 — Vercel (recomendado)

1. Subí esta carpeta a un repositorio de GitHub.
2. Entrá a [vercel.com](https://vercel.com) → **Add New Project**.
3. Importá el repo. Vercel detecta `vercel.json` y lo despliega automáticamente.
4. Te da una URL pública para compartir con tu equipo.

### Opción 2 — GitHub Pages

1. En tu repo → **Settings → Pages**.
2. Source: `Deploy from a branch` → rama `main`, carpeta `/ (root)`.
3. En unos minutos tenés la URL (index.html se sirve como home automáticamente).

### Opción 3 — Local

Abrí `index.html` directamente en el navegador. No necesita servidor ni instalación. El progreso (módulos completados, checklists) se guarda en el navegador de cada persona con `localStorage`.

---

## ✏️ Cómo editar el contenido

- **Módulos del plan:** cada módulo es un bloque `<div class="module-section" id="mod-N">` dentro de `index.html`. Contiene tarjetas de teoría (`tag-teoria`), tips (`tag-tips`), ejercicio (`tag-ejer`) y chequeo rápido (`tag-check`).
- **Chequeos rápidos (multiple choice):** editá las opciones en `.mc-label` y el atributo `data-correct` con la letra correcta.
- **Checklist de ejercicios:** cada `<li>` con checkbox se guarda solo con `data-storage-prefix` del módulo — no requiere tocar el script.
- **Agregar un módulo nuevo:** copiá un bloque `module-section`, sumale un tab en el array `modNames` del script, y actualizá `TOTAL_MODULES`.
- **Cuestionario final:** se edita igual que antes, ver comentarios dentro de `cuestionario-fotografia.html`.

---

## 🛠 Tecnologías

HTML5 / CSS3 / JavaScript vanilla. Fuentes: Playfair Display + Outfit (Google Fonts). Sin dependencias ni frameworks — dos archivos autocontenidos.

---

Este plan integra el manual interno "Fotografía Social · Bodas & 15 Años" y contenido curado de guías profesionales de dirección y trato con clientes, adaptado a bodas y 15 años.

Hecho para uso interno del equipo · La Belle Joie
