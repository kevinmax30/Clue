# 🕯 Clue — Bloc de Pistas (PWA)

Bloc de notas digital para el juego **Clue / Cluedo**, instalable como app en cualquier celular.

## 📁 Estructura
```
clue-pwa/
├── index.html       ← App principal
├── manifest.json    ← Config PWA
├── sw.js            ← Service Worker (funciona offline)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## 🚀 Publicar en GitHub Pages

1. **Crear repositorio** en GitHub (ej: `clue-pwa`)
2. **Subir todos los archivos** (mantener la estructura de carpetas)
   ```bash
   git init
   git add .
   git commit -m "Clue PWA"
   git remote add origin https://github.com/TU_USUARIO/clue-pwa.git
   git push -u origin main
   ```
3. Ir a **Settings → Pages** en tu repo
4. En "Source" seleccionar **Deploy from a branch → main → / (root)**
5. Guardar. En ~1 minuto la app estará en:
   ```
   https://TU_USUARIO.github.io/clue-pwa/
   ```

## 📲 Instalar en el celular

### Android (Chrome)
- Abre la URL en Chrome
- Aparece un banner "Agregar a inicio" **o** menú ⋮ → "Instalar app"

### iPhone (Safari)
- Abre la URL en Safari
- Toca el botón compartir 📤 → "Agregar a pantalla de inicio"

Una vez instalada funciona **sin internet** (Service Worker cachea todo).

## 🎮 Funciones
- ✕ Marcar que nadie tiene la carta (toda la fila se pinta roja)
- ✔ Marcar que un jugador la tiene (verde + resto rojo)  
- ❓ Acumular sospechas (hasta 4, con badge visible)
- 🔀 Mezclar el orden de filas para despistar miradas
- Hasta 6 jugadores con nombres personalizables
