<div align="center">

<img src="./assets/img/Logo1.png" alt="Logo CineVerse" width="90" />

# CineVerse

**Plataforma de streaming ficticia — proyecto de práctica full front-end**

![Estado del proyecto](https://img.shields.io/badge/estado-en%20desarrollo-yellow)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3.8-7952B3?logo=bootstrap&logoColor=white)
![Licencia](https://img.shields.io/badge/licencia-educativa-lightgrey)

[Demo](#-cómo-usarlo) · [Características](#-características) · [Estructura](#-estructura-del-proyecto) · [Equipo](#-equipo)

</div>

---

## 📋 Descripción

**CineVerse** es un sitio web estático inspirado en las plataformas de streaming modernas (Netflix, HBO Max, Disney+). Cuenta con un diseño oscuro y cinematográfico, pensado para ofrecer una experiencia visual atractiva a la hora de explorar películas y series.

El proyecto simula **dos experiencias de usuario distintas**:

- 👤 **Visitante (no suscripto)** — navega el catálogo público, puede iniciar sesión o suscribirse.
- ⭐ **Usuario Premium (suscripto)** — accede a una experiencia personalizada con historial de reproducción, recomendaciones, tendencias y reproductor propio.

Todo el proyecto está desarrollado **sin una sola línea de JavaScript**: la interactividad (modales, dropdowns, navegación, collapse) se resuelve íntegramente con los componentes nativos de Bootstrap 5.

## ✨ Características

### 🌐 Sitio público (`/pages/noSuscripto`)
- 🏠 **Inicio** — hero destacado, películas y series destacadas, banner promocional, categorías.
- 🎞️ **Películas** — catálogo con filtros por género/orden y buscador.
- 📺 **Series** — catálogo con filtros, paginación y modal de detalle (tráiler + episodios).
- ℹ️ **Nosotros** — información del equipo.
- 📩 **Contacto** — formulario con validación nativa HTML5, datos de contacto y redes sociales.
- 💳 **Suscripción** — planes (Básico, Estándar, Premium) y formulario de registro.
- 🔐 **Modal de Login** — inicio de sesión con validación de campos y accesos sociales (visual).
- 🚫 **Error 404** — página de error con estilo propio.

### ⭐ Experiencia Premium (`/pages/suscripto`)
- 🎥 **Inicio Premium** — hero con **video de fondo autoplay**, menú de perfil con avatar e insignia Premium.
- ▶️ **Continuar viendo** — tarjetas con barra de progreso y tiempo restante.
- 🔥 **Tendencias** — ranking Top 10 con numeración destacada.
- 📌 **Mi Lista** — contenido guardado por el usuario.
- 🆕 **Estrenos** — nuevos lanzamientos con insignia "NUEVO".
- 🎬 **Reproductor** — pantalla inmersiva 16:9 sin navbar/footer, con barra de controles estilo streaming (play, volumen, progreso, calidad, pantalla completa) y estado de error simulado.
- 🪟 **Modales de detalle** — ficha de película/serie con tráiler embebido (YouTube), sinopsis, datos técnicos y episodios navegables.

### 📱 General
- Diseño **responsive** adaptado a mobile, tablet y desktop.
- Identidad visual coherente en todas las páginas mediante variables CSS.

## 🛠️ Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica |
| **CSS3** | Estilos, variables CSS (`:root`), Flexbox, Grid |
| **Bootstrap 5.3.8** | Grid system, modales, dropdowns, paginación, navbar |
| **Bootstrap Icons** | Iconografía |
| **Google Fonts (Montserrat)** | Tipografía |

> No se utiliza JavaScript propio ni frameworks adicionales. Toda la interactividad depende de los componentes nativos de Bootstrap.

## 🎨 Paleta de colores

| Color | Uso | Valor |
|---|---|---|
| 🔴 Principal | Acentos, botones, marca | `#E50914` |
| 🔴 Hover | Estados hover/focus | `#FF2D55` |
| ⚫ Fondo primario | Fondo general | `#111111` |
| ⚫ Fondo secundario | Secciones alternas | `#1B1B1B` |
| ⚫ Fondo de tarjetas | Cards, modales | `#202020` |
| ⚪ Texto primario | Texto principal | `#FFFFFF` |
| ⚪ Texto secundario | Texto apagado | `#B3B3B3` |
| ⚪ Bordes | Separadores | `#2D2D2D` |

## 📁 Estructura del proyecto
CineVerse/
├── index.html
├── assets/
│ ├── img/ # Imágenes y posters
│ └── vids/ # Videos (hero, trailers locales)
├── css/
│ ├── noSuscripto/ # Estilos del sitio público
│ │ ├── style.css
│ │ ├── pelicula.css
│ │ ├── series.css
│ │ ├── nosotros.css
│ │ ├── contacto.css
│ │ ├── suscripcion.css
│ │ └── error404.css
│ └── suscripto/ # Estilos de la experiencia Premium
│ ├── inicioSus.css
│ ├── peliculaSus.css
│ ├── seriesSus.css
│ ├── nosotrosSus.css
│ ├── contactoSus.css
│ ├── reproductor.css
│ └── error404Sus.css
└── pages/
├── noSuscripto/
│ ├── pelicula.html
│ ├── series.html
│ ├── nosotros.html
│ ├── contacto.html
│ ├── suscripcion.html
│ └── error404.html
└── suscripto/
├── inicioSus.html
├── peliculaSus.html
├── seriesSus.html
├── nosotrosSus.html
├── contactoSus.html
├── reproductor.html
└── error404Sus.html

## 🚀 Cómo usarlo

1. Cloná el repositorio:
```bash
   git clone https://github.com/herreraagustin/CineVerse.git
```
2. Entrá a la carpeta del proyecto:
```bash
   cd CineVerse
```
3. Abrí `index.html` en tu navegador, o usá una extensión como **Live Server** (VS Code) para levantarlo en un servidor local.

No requiere instalación de dependencias: Bootstrap, Bootstrap Icons y la tipografía se cargan desde CDN.

## 🗺️ Roadmap

- [ ] Página de perfil de usuario
- [ ] Página "Mi Lista" completa
- [ ] Sección de búsqueda con resultados dinámicos

## 👥 Equipo

Desarrollado por **DreamTeam**.

## 🔗 Enlaces

- 💻 [Repositorio en GitHub](https://github.com/herreraagustin/CineVerse)
- 📋 [Tablero de Trello](https://trello.com/b/086Mx1SU/cineverse)

## 📄 Licencia

Este proyecto fue creado con fines educativos/de práctica. Todas las imágenes, videos y contenido de terceros (posters, tráilers) se utilizan únicamente con fines demostrativos y pertenecen a sus respectivos titulares.

© 2024 CineVerse. Todos los derechos reservados.
