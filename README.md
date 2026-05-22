# Kit Web Scrolling — Webs Premium con Claude Code

Crea webs profesionales de una sola página con animaciones de scroll para cualquier tipo de negocio. Solo hablas con Claude Code, le das los datos de tu negocio, y él genera el sitio completo.

---

## Cómo funciona

1. Abres esta carpeta en VS Code con la extensión de Claude Code
2. Le dices a Claude el nombre y tipo de negocio
3. Claude te pregunta los datos (servicios, precios, horario, contacto, fotos...)
4. Genera un archivo HTML listo para abrir en el navegador
5. Si quieres cambiar algo, se lo dices y lo ajusta al instante

No necesitas saber programar.

---

## Webs generadas — ejemplos incluidos

| Archivo | Negocio | Estilo |
|---|---|---|
| `web-kikas-peluqueria.html` | Kika's Peluquería & Barber | Oscuro · Rojo y azul marino |
| `forbidden-coffee.html` | Forbidden Coffee | Oscuro · Minimalista |
| `cafe-cacao.html` | Café Cacao | Cálido · Marrón y crema |
| `web-eurotek.html` | Eurotek | Tecnológico · Azul y gris |

---

## Características de las webs generadas

- **Animaciones de scroll** — elementos que aparecen al hacer scroll con Intersection Observer nativo
- **Hero con foto real** — imagen de fondo con efecto parallax
- **Contadores animados** — estadísticas que cuentan desde 0 al entrar en pantalla
- **Diseño responsive** — funciona en móvil, tablet y escritorio
- **Menú hamburguesa** — navegación optimizada para teléfono
- **Mapa interactivo** — Google Maps embebido en la sección de contacto
- **Horario inteligente** — resalta automáticamente el día de hoy
- **Galería de fotos** — grid con imágenes reales del negocio
- **Sección de reseñas** — testimonios reales de clientes
- **Un solo archivo HTML** — sin frameworks, sin dependencias, funciona abriéndolo directamente

---

## Estructura del proyecto

```
kit-web-scrolling/
├── CLAUDE.md                        ← Instrucciones que Claude lee automáticamente
├── INSTRUCCIONES.md                 ← Guía de uso para el usuario
├── README.md                        ← Este archivo
├── .claude/
│   └── skills/
│       └── 01-web-scrolling.md      ← Skill que define cómo Claude genera las webs
├── assets/                          ← Pon aquí las fotos y vídeos del negocio
│   ├── interior-1.jpg
│   ├── corte-1.jpg
│   └── ...
└── web-[nombre-negocio].html        ← Web generada (un archivo por negocio)
```

---

## Requisitos

- [Visual Studio Code](https://code.visualstudio.com)
- Extensión [Claude Code](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code) para VS Code

---

## Uso rápido

```
1. git clone https://github.com/tu-usuario/kit-web-scrolling
2. Abre la carpeta en VS Code
3. Abre Claude Code en el panel lateral
4. Escribe: "Hazme una web para mi negocio"
```

---

## Publicar la web

### Netlify (gratis, 2 minutos)
1. Ve a [netlify.com](https://netlify.com) y crea una cuenta
2. Arrastra la carpeta del proyecto a la pantalla de Netlify
3. Obtienes una URL pública al instante

### Con dominio propio
1. Compra un dominio en Namecheap o GoDaddy (~$12 USD/año)
2. Sube la web a Netlify
3. Conecta el dominio desde el panel de Netlify

---

## Personalización

Claude puede ajustar cualquier cosa en la web generada. Ejemplos de lo que puedes pedirle:

```
"Cambia el color principal a verde"
"Añade una sección de precios"
"El sábado cerramos a las 6, no a las 8"
"Pon el logo en el menú"
"Quiero el efecto de vídeo con scroll como Apple"
```

### Efecto scroll-video (opcional)
Si tienes un vídeo del negocio, ponlo en `assets/hero.mp4` y pide:
> "Quiero el efecto de vídeo con scroll"

El vídeo avanzará fotograma a fotograma mientras el usuario hace scroll, igual que en la web de Apple.

---

## Stack técnico

Las webs generadas usan únicamente tecnologías nativas del navegador:

- **HTML5** semántico
- **CSS3** — variables, grid, flexbox, animaciones
- **JavaScript vanilla** — Intersection Observer, requestAnimationFrame
- **Google Fonts** — única dependencia externa (tipografía)
- **Google Maps Embed** — iframe interactivo sin API key

Sin React, sin Vue, sin bundlers. El archivo HTML funciona abriéndolo directamente.

---

## Licencia

MIT — úsalo libremente para proyectos personales y comerciales.
