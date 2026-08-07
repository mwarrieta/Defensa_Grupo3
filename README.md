# Plan de Mejora en la Planificación del Mantenimiento y Gestión del Backlog de Equipos LHD

**Codelco · División Chuquicamata Subterránea**
Proyecto de Título EIN9947 · Grupo 03 · Ingeniería Industrial UDLA

Presentación interactiva de defensa (22 diapositivas, 20 minutos) con temporizador integrado, carta Gantt y cuaderno de datos anexo.

## Estructura

```
proyecto-lhd-main/
├── index.html      ← Presentación principal (22 diapositivas)
├── datos.html      ← Cuaderno de datos sistematizados (9 pestañas)
├── gantt.html      ← Carta Gantt de implementación (Anexo)
├── video.mp4       ← Video de fondo de portada
├── imagen.webp     ← Imagen de apoyo
├── img/            ← Fotos, infografías y logo
└── README.md
```

Todos los enlaces entre archivos son relativos. La carpeta funciona igual abierta localmente o publicada en un servidor.

## Publicar en GitHub Pages

1. Crear un repositorio nuevo y subir **el contenido de esta carpeta en la raíz** (que `index.html` quede en el primer nivel, no dentro de una subcarpeta).
2. En el repositorio: **Settings → Pages**.
3. En *Source*, elegir **Deploy from a branch**.
4. Rama `main`, carpeta `/ (root)` → **Save**.
5. A los pocos minutos queda disponible en `https://<usuario>.github.io/<repositorio>/`.

El repositorio puede ser público o privado; con Pages en repositorio privado se requiere cuenta Pro.

## Navegación

- **Flechas ← →** o clic en los controles inferiores para avanzar entre diapositivas.
- **Temporizador** abajo a la izquierda: 20 minutos, con play/pausa y reset.
- Desde la diapositiva 16 se abre la **carta Gantt** en pestaña nueva.
- Varias diapositivas tienen un botón **"Ver en el cuaderno de datos"** que abre `datos.html` en la pestaña correspondiente; el botón naranja del cuaderno devuelve a la diapositiva de origen.
- Las imágenes de proceso, el Ishikawa y el FODA se amplían con un clic (`Esc` para cerrar).

## Notas técnicas

- Chart.js va incrustado en los archivos: no hay dependencias externas de JavaScript.
- Las tipografías se cargan desde Google Fonts; sin conexión el navegador usa una alternativa del sistema y todo lo demás sigue funcionando.
- Requiere JavaScript habilitado. Probado en Chrome y Edge.
- `datos.html` se genera desde `../analisis/build.py`; no editarlo a mano.
