# Guía de aprendizaje

Notas personales y hoja de ruta para aprender Astro mientras construyo esta colección.

## Cursos generales de Astro (en español)

- 🎥 [Aprende Astro 3 desde cero: curso para principiantes](https://www.youtube.com/watch?v=RB5tR_nqUEw) (midudev)
- 🎥 [Curso de Astro con proyectos](https://www.youtube.com/playlist?list=PLUofhDIg_38q8ZBsl9-GPRNI1AIjkRIHZ) (playlist de midudev)
- 📚 [Curso de Astro y Headless CMS](https://midu.dev/curso/astro-cms-headless) (midu.dev, gratis)
- 📚 [Tutorial oficial: construye tu primer blog con Astro](https://docs.astro.build/es/tutorial/0-introduction/)

## Hoja de ruta

### 1. Componentes y props

Cómo hacer tu primer componente.

- [ ] Entender la estructura del proyecto (`src/pages`, `src/components`, `public`)
- [ ] Crear tu primer componente `.astro` en `src/components/`
- [ ] Pasarle datos con props y tiparlos con `interface Props`
- [ ] Usarlo dentro de una página
- [ ] Darle estilos con `<style>` (los estilos quedan limitados al componente)

📚 Recursos:

- [Estructura del proyecto](https://docs.astro.build/es/basics/project-structure/)
- [Componentes de Astro](https://docs.astro.build/es/basics/astro-components/)
- [Estilos en Astro](https://docs.astro.build/es/guides/styling/)

### 2. Layouts y `<slot />`

La estructura que comparten todas tus páginas.

- [ ] Crear un layout en `src/layouts/` con el `<html>`, `<head>` y `<body>` base
- [ ] Usar `<slot />` para insertar el contenido de cada página
- [ ] Pasarle props al layout (por ejemplo, el `title` de la página)
- [ ] Probar los slots con nombre (`<slot name="..." />`)
- [ ] Hacer que todas las páginas usen el layout

📚 Recursos:

- [Layouts](https://docs.astro.build/es/basics/layouts/)
- [Slots en componentes de Astro](https://docs.astro.build/es/basics/astro-components/#slots)

### 3. Routing

Páginas, rutas dinámicas y paginación con `paginate()`.

- [ ] Entender el routing basado en archivos (cada archivo en `src/pages/` es una ruta)
- [ ] Crear una página de demo por cada componente
- [ ] Crear una ruta dinámica (`[slug].astro`) con `getStaticPaths()`
- [ ] Hacer la página principal como galería que enlace a cada demo
- [ ] Paginar la galería con `paginate()` (`[...page].astro`)
- [ ] Agregar botones de "anterior" y "siguiente" usando `page.url.prev` y `page.url.next`

📚 Recursos:

- [Routing](https://docs.astro.build/es/guides/routing/)
- [Paginación](https://docs.astro.build/es/guides/routing/#paginación)
- [Referencia de routing (`getStaticPaths`, `paginate`)](https://docs.astro.build/es/reference/routing-reference/)

### 4. Content collections

Por si quieres manejar la colección como datos.

- [ ] Entender qué es una colección y cuándo conviene usarla
- [ ] Definir la colección en `src/content.config.ts` con un esquema (título, descripción, fecha, tags...)
- [ ] Guardar la información de cada componente como entrada de la colección (Markdown, MDX o JSON)
- [ ] Consultarla con `getCollection()` para armar la galería
- [ ] Generar las páginas de cada componente a partir de la colección
- [ ] Filtrar u ordenar (por fecha, por tag...)

📚 Recursos:

- [Content collections](https://docs.astro.build/es/guides/content-collections/)
- [TypeScript en Astro](https://docs.astro.build/es/guides/typescript/)

### Extra (cuando termines lo anterior)

- [ ] Agregar interactividad con `<script>` → [Scripts del lado del cliente](https://docs.astro.build/es/guides/client-side-scripts/)
- [ ] Transiciones animadas entre páginas → [View transitions](https://docs.astro.build/es/guides/view-transitions/)
- [ ] Usar React, Svelte o Vue en algún componente → [Componentes de frameworks](https://docs.astro.build/es/guides/framework-components/)
- [ ] Publicar la colección → [Despliegue en GitHub Pages](https://docs.astro.build/es/guides/deploy/github/)

