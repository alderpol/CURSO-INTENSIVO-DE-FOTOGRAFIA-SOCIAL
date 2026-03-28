# 📷 Cuestionario · Fotografía de Eventos Sociales

App web interactiva para evaluar alumnos en un curso intensivo de fotografía de eventos. Incluye preguntas abiertas, multiple choice con corrección automática y casos prácticos.

---

## 🗂 Módulos

| # | Módulo |
|---|--------|
| 1 | Exposición |
| 2 | Foco y Nitidez |
| 3 | Flash |
| 4 | Composición Funcional |
| 5 | Narrativa |
| 6 | Dirección y Manejo del Cliente |
| 7 | Criterio Profesional |
| 8 | Diagnóstico Final |

---

## 🚀 Cómo usar

### Opción 1 — Vercel (recomendado)

1. Subí el repositorio a GitHub
2. Entrá a [vercel.com](https://vercel.com) → **Add New Project**
3. Importá el repo
4. Vercel detecta la config automáticamente y lo despliega
5. Listo — te da una URL pública para compartir con tus alumnos

### Opción 2 — GitHub Pages

1. En tu repo → **Settings → Pages**
2. Source: `Deploy from a branch` → rama `main`, carpeta `/ (root)`
3. Guardá — en unos minutos tenés la URL

### Opción 3 — Local

Abrí `cuestionario-fotografia.html` directamente en el navegador. No necesita servidor ni instalación.

---

## 📁 Estructura del proyecto

```
/
├── cuestionario-fotografia.html   # App completa (un solo archivo)
├── vercel.json                    # Configuración de despliegue
└── README.md                      # Este archivo
```

---

## ✏️ Cómo editar el contenido

Todo el cuestionario está en `cuestionario-fotografia.html`. Para modificar preguntas:

- **Preguntas abiertas / casos**: buscá el texto dentro de `<div class="q-text">` y editalo
- **Multiple choice**: editá las opciones en `<div class="mc-label">` y cambiá `data-correct="X"` con la letra correcta
- **Agregar módulos**: copiá un bloque `<div class="module-section">` y actualizá el ID y contenido

---

## 🛠 Tecnologías

- HTML5 / CSS3 / JavaScript vanilla
- Fuentes: Playfair Display + Outfit (Google Fonts)
- Sin dependencias ni frameworks — un solo archivo

---

Hecho para uso educativo · Curso de Fotografía de Eventos Sociales
