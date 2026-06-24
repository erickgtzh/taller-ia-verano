# 🤖 Taller IA Verano — Clasificador de Imágenes

Proyecto didáctico para enseñar programación e inteligencia artificial a través de un clasificador de imágenes construido con [Teachable Machine](https://teachablemachine.withgoogle.com/) y JavaScript.

## 🌐 Demo en vivo

👉 **[Abrir el clasificador](https://erickgtzh.github.io/taller-ia-verano/clasificador_camara.html)**

## 📁 Archivos

| Archivo | Descripción |
|---------|-------------|
| [`clasificador.html`](./clasificador.html) | Clasificador base — sube una imagen o toma foto |
| [`clasificador_camara.html`](./clasificador_camara.html) | Clasificador con cámara en vivo y permisos completos |

## 🗺️ Diagrama de flujo del programa

El código sigue este flujo:

```
Inicio
  ↓
[1] Cargar modelo entrenado (variable)
  ↓
[2] Recibir imagen ←──────────────────┐
  ↓                                    │
[3] El modelo predice (función)        │
  ↓                                    │
[4] Tomar la clase más probable        │
  ↓                                    │
[5] ¿Confianza > 80%? (if)             │
   ├─ SÍ → Mostrar "Es X (92%)"       │
   └─ NO → Mostrar "No estoy seguro"  │
  ↓                                    │
[6] ¿Otra imagen?                      │
   ├─ SÍ ──────────────────────────── ┘
   └─ NO → Fin
```

## 🚀 ¿Cómo usar?

1. Ve a [Teachable Machine](https://teachablemachine.withgoogle.com/) y entrena un modelo de imágenes
2. Expórtalo como **TensorFlow.js** y copia la URL
3. Abre cualquiera de los archivos HTML y pega la URL
4. ¡Comienza a clasificar!

> ⚠️ Para el clasificador con cámara, necesitas servir el archivo desde un servidor local (Live Server en VS Code) o usar la versión de GitHub Pages.

## 🛠️ Tecnologías

- [TensorFlow.js](https://www.tensorflow.org/js)
- [@teachablemachine/image](https://www.npmjs.com/package/@teachablemachine/image)
- HTML + CSS + JavaScript vanilla

## 👨‍🏫 Contexto

Creado para el Taller de IA · Verano 2026.
