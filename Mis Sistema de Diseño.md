---
version: alpha
name: Mi Sistema de Diseño
description: "Sistema de diseño de la marca personal de Cecilia Ramírez Vázquez: identidad digital creativa, experimental y funcional para el portafolio de UX/UI, con base rojo + azul + blanco + negro."
colors:
  primary: "#AD2B2B"
  primary-dark: "#8E2222"
  secondary: "#7CAAD9"
  on-primary: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  surface-variant: "#F2F2F2"
typography:
  display:
    fontFamily: "Acumin Variable Concept"
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.1
  h1:
    fontFamily: "Acumin Variable Concept"
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.15
  h2:
    fontFamily: "Acumin Variable Concept"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
  h3:
    fontFamily: "Acumin Variable Concept"
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.25
  body:
    fontFamily: "Acumin Variable Concept"
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: "Acumin Variable Concept"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: "Acumin Variable Concept"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.4
spacing:
  base: 8px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  xxl: 64px
  3xl: 80px
  4xl: 96px
  5xl: 128px
  gutter: 24px
  margin-mobile: 16px
  margin-tablet: 40px
  margin-desktop: 64px
  max-width: 1440px
  grid-columns-desktop: 12
  grid-columns-tablet: 8
rounded:
  none: 0px
  sm: 4px
  md: 8px
  full: 9999px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 44px
    padding: 24px
  button-primary-hover:
    backgroundColor: "{colors.primary-dark}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 44px
    padding: 24px
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 44px
    padding: 24px
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 44px
    padding: 24px
  link:
    textColor: "{colors.secondary}"
    typography: "{typography.label-md}"
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.md}"
  chip:
    backgroundColor: "{colors.surface-variant}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 16px
    height: 32px
  nav-active:
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
---

# Mi Sistema de Diseño

## Overview

La marca personal representa una visión creativa, experimental y contemporánea del diseño digital, enfocada en explorar nuevas formas de comunicar, interactuar y resolver problemas mediante el diseño UX/UI.

El portafolio refleja tanto la formación académica como el proceso creativo, mostrando proyectos que combinan investigación, conceptualización, diseño visual y desarrollo de experiencias digitales. Se prioriza una estética limpia, dinámica y funcional, donde cada elemento visual tiene un propósito.

La identidad transmite curiosidad, creatividad y capacidad de exploración: el diseño se entiende como una herramienta para investigar, experimentar y resolver problemas, no solo como la creación de piezas visuales. En una frase: una identidad digital creativa, experimental y funcional que comunica la evolución académica y la manera de entender el diseño.

> **Notas de revisión**: los valores de tokens marcados como *asumidos* se completaron con el valor medio de los rangos indicados en el documento original. Revísalos y ajusta los que consideres: `colors.primary-dark`, tamaños de `typography`, `spacing.margin-tablet` y `spacing.margin-desktop`.

## Colors

La paleta se construye con rojo, azul, negro y blanco, tomando como referencia los elementos gráficos de la identidad. El contraste entre colores primarios y neutros genera una identidad visual dinámica, experimental y reconocible, sin perder claridad en la presentación de proyectos académicos.

- **Rojo de marca** `{colors.primary}` (#AD2B2B): color principal de identidad. Se utiliza para títulos destacados, palabras clave, acentos gráficos, elementos de navegación activa ({components.nav-active}) y llamadas de atención.
- **Rojo oscuro (hover)** `{colors.primary-dark}` (#8E2222): *valor asumido* para el estado hover del rojo, ligeramente oscurecido.
- **Azul principal** `{colors.secondary}` (#7CAAD9): color secundario de identidad. Complementa al rojo y se usa para información secundaria, elementos interactivos y recursos gráficos.
- **Negro** `{colors.on-surface}` (#000000): color principal para textos, títulos, navegación y elementos de mayor contraste.
- **Blanco** `{colors.surface}` / `{colors.on-primary}` (#FFFFFF): fondo principal del portafolio. Permite espacios limpios y da protagonismo a los proyectos.
- **Gris claro** `{colors.surface-variant}` (#F2F2F2): fondo secundario para separar secciones, tarjetas o bloques de información sin introducir nuevos colores.

La combinación cromática debe mantenerse principalmente en blanco + negro, usando rojo y azul como acentos. El rojo representa energía y expresión; el azul aporta equilibrio y contraste. El color no es decoración: funciona para establecer jerarquías, navegación y puntos de atención.

## Typography

La tipografía transmite una personalidad contemporánea, experimental y académica, combinando una sans serif de alta legibilidad con pesos contrastantes. La familia principal, **Acumin Variable Concept**, se usa para cuerpo, navegación y descripciones. Los títulos usan pesos Bold o ExtraBold para marcar jerarquía.

- **Display** `{typography.display}`: 56 px · Bold. Para el nombre, títulos principales y mensajes de entrada. *(asumido del rango 48–64 px)*
- **Título 1** `{typography.h1}`: 44 px · Bold. Para títulos de proyectos y secciones principales. *(asumido del rango 40–48 px)*
- **Título 2** `{typography.h2}`: 32 px · Bold. Para subsecciones. *(asumido del rango 28–36 px)*
- **Título 3** `{typography.h3}`: 22 px · Semibold. Para categorías, apartados y elementos de apoyo. *(asumido del rango 20–24 px)*
- **Cuerpo** `{typography.body}`: 18 px · Regular, con interlineado de 1.5. Para descripciones, procesos y textos académicos.
- **Texto pequeño** `{typography.body-sm}`: 15 px. Para fechas, herramientas, categorías y datos secundarios. *(asumido del rango 14–16 px)*
- **Botones y navegación** `{typography.label-md}`: 16 px · Semibold. *(asumido del rango 16–18 px)*

La jerarquía se establece mediante tamaño, peso, posición y color, evitando depender solo de la opacidad. Los títulos pueden combinar negro con palabras o fragmentos destacados en rojo (`{colors.primary}`) o azul (`{colors.secondary}`) para reforzar la personalidad experimental.

## Layout

El sistema de composición es editorial digital: limpio, estructurado y experimental.

El espaciado usa una base de 8 px (`{spacing.base}`) con la escala `{spacing.xs}` · `{spacing.sm}` · `{spacing.md}` · `{spacing.lg}` · `{spacing.xl}` · `{spacing.xxl}` · `{spacing.3xl}` · `{spacing.4xl}` · `{spacing.5xl}`. La estrategia es *mobile-first*:

- **Móvil (320–599 px)**: una columna principal, márgenes de `{spacing.margin-mobile}` (16 px), navegación compacta, proyectos en una columna e imágenes a ancho completo. Display de 32–40 px y cuerpo de 16–18 px.
- **Tableta (600–1023 px)**: dos columnas de proyectos cuando el contenido lo permite, márgenes de `{spacing.margin-tablet}` (40 px, asumido del rango 32–48 px), mayor separación entre secciones y hero en dos bloques.
- **Escritorio (1024–1439 px)**: rejilla de `{spacing.grid-columns-desktop}` (12) columnas, márgenes de `{spacing.margin-desktop}` (64 px, asumido del rango 48–80 px), proyectos en composiciones de 2–3 columnas y títulos de mayor escala.
- **Escritorio amplio (1440 px+)**: contenido centrado con máximo de `{spacing.max-width}` (1440 px), uso amplio del espacio negativo, composiciones asimétricas y secciones separadas entre `{spacing.3xl}` y `{spacing.5xl}`.

El ancho máximo del contenido es de aproximadamente 1440 px, con márgenes amplios en escritorio. Las secciones principales pueden usar composiciones asimétricas para reforzar el carácter experimental, conservando siempre una estructura visual clara. El espacio en blanco es clave: separa proyectos, destaca imágenes y evita que la información académica se vuelva pesada.

Todos los elementos interactivos deben tener un área mínima de **44 × 44 px** ({components.button-primary} usa altura 44 px). La experiencia responsiva no debe sentirse como una versión reducida del escritorio, sino como una adaptación específica para cada dispositivo.

## Elevation & Depth

El sistema usa profundidad mínima y principalmente plana. El portafolio debe sentirse editorial y gráfico, no excesivamente tridimensional.

- **Nivel 0 — Plano**: fondos, navegación, textos y proyectos en reposo.
- **Nivel 1 — Interacción**: sombra muy ligera o cambio de borde para indicar hover.
- **Nivel 2 — Destacado**: tarjetas o ventanas que necesitan separarse del fondo.
- **Nivel 3 — Modal**: elementos que aparecen sobre el contenido principal.

Las sombras se usan con moderación. La personalidad visual se construye principalmente mediante color, composición, escala y contraste, no mediante efectos de profundidad.

## Shapes

Las formas combinan una estructura editorial limpia con elementos gráficos experimentales.

- Los contenedores principales usan esquinas rectas o ligeramente redondeadas de 4–8 px ({components.button-primary} usa `{rounded.sm}` y {components.card} usa `{rounded.md}`), evitando un estilo excesivamente corporativo.
- Los elementos gráficos de identidad pueden usar formas libres y orgánicas inspiradas en los recursos visuales de la identidad: estrellas, trazos, formas irregulares y elementos superpuestos.
- Los círculos se usan para fotografías, avatares o pequeños elementos de navegación.
- La superposición de rojo (`{colors.primary}`) y azul (`{colors.secondary}`) es un recurso experimental válido, especialmente en portadas de proyectos, separadores y composiciones destacadas.

Las formas gráficas no son decoración: deben señalar información, separar proyectos o generar puntos de atención.

## Components

### Buttons — Botones

El **botón principal** ({components.button-primary}) usa fondo rojo `{colors.primary}` con texto blanco `{colors.on-primary}`. Altura mínima de 44 px, padding horizontal de `{components.button-primary.padding}` (20–24 px), tipografía `{typography.label-md}` y radio `{rounded.sm}` (4–8 px). En hover ({components.button-primary-hover}) el rojo se oscurece a `{colors.primary-dark}` con un cambio sutil de posición o escala.

El **botón secundario** ({components.button-secondary}) usa fondo `{colors.surface}`, borde negro y texto negro `{colors.on-surface}`. En hover ({components.button-secondary-hover}) cambia a rojo con texto blanco.

Los botones no deben acumular efectos; la interacción se siente directa y clara.

### Cards — Tarjetas de proyectos

Las tarjetas ({components.card}) funcionan como elementos editoriales: fondo `{colors.surface}`, imagen del proyecto como elemento principal, título en negro, categoría o disciplina en rojo (`{colors.primary}`) o azul (`{colors.secondary}`), descripción breve y año o información académica en tamaño pequeño. En hover, la imagen puede aumentar ligeramente de escala o aparecer un acento rojo/azul. La tarjeta prioriza el proyecto visual antes que el texto.

### Hero

La sección inicial presenta el nombre, perfil académico y especialidad. Fondo `{colors.surface}`, tipografía `{colors.on-surface}` y elementos gráficos rojos y azules. Puede incorporar composiciones asimétricas, formas experimentales o elementos superpuestos para evitar una presentación genérica. Debe comunicar rápidamente: quién soy + qué hago + qué estoy estudiando/diseñando.

### Navigation — Navegación

Estructura sencilla y horizontal en escritorio: **Inicio · Sobre mí · Proyectos · CV · Contacto**. El texto se mantiene principalmente en negro. La sección activa usa rojo como indicador ({components.nav-active}). El azul es color secundario y no debe competir con el rojo en el mismo elemento interactivo.

### Chips — Etiquetas

Las etiquetas ({components.chip}) identifican **UX/UI · Diseño digital · Investigación · Prototipado · Branding · 3D · Diseño editorial**. Usan fondo `{colors.surface-variant}` con texto negro, o rojo/azul de manera puntual. Deben ser pequeñas y funcionales, no el elemento dominante.

### Profile photo — Fotografía de perfil

Puede usarse en formato circular o rectangular según la composición, e incorporar un marco o elemento gráfico rojo/azul para integrarla con la identidad. Debe sentirse natural y académica, evitando tratamientos excesivamente corporativos.

### Education & experience — Educación y experiencia

La información académica se presenta en bloques editoriales. Cada bloque incluye institución, programa, periodo y descripción breve o área de formación. El rojo puede funcionar como acento lateral o indicador de fecha, mientras que el negro mantiene la información principal.

### Skills — Habilidades

Se presentan mediante etiquetas o pequeñas listas visuales (ej. UX/UI · Diseño digital · Prototipado · Investigación · Figma · Adobe Creative Cloud · Diseño de interfaces). La información debe escanearse rápido y no ocupar demasiado espacio.

## Do's and Don'ts

### Do's — Lo que sí se permite

- Usar rojo (`{colors.primary}`) como color principal de acento.
- Usar azul (`{colors.secondary}`) como color secundario.
- Mantener negro y blanco como base visual.
- Priorizar la presentación visual de los proyectos.
- Usar composiciones asimétricas cuando refuercen la personalidad experimental.
- Usar suficiente espacio en blanco.
- Combinar imágenes, tipografía y formas gráficas.
- Mantener una jerarquía clara para que el contenido académico sea fácil de leer.
- Usar el rojo para información importante y navegación activa.
- Usar el azul para información secundaria y elementos complementarios.

### Don'ts — Lo que no se permite

- No usar demasiados colores fuera de la paleta.
- No combinar rojo y azul indiscriminadamente dentro de un mismo botón o acción.
- No sobrecargar las páginas con elementos decorativos.
- No usar sombras pesadas.
- No convertir todos los elementos en tarjetas.
- No usar tipografías decorativas que dificulten la lectura.
- No sacrificar la legibilidad por una composición experimental.
- No usar animaciones excesivas que distraigan de los proyectos.
- No reducir demasiado el tamaño del texto académico.