---
colors:
  # Brand colors
  primary: "#B82925"        # Rojo corazón - brand, CTA primary, main actions
  secondary: "#3D5A8A"      # Azul creativo (oscurecido para WCAG AA 4.5:1) - secondary actions, subtitles, supporting
  accent: "#00A79D"         # Turquesa - hover states, indicators, transitions (SOLO gráfico, nunca texto)
  
  # Neutral colors
  background: "#E7ECE8"     # Verde muy claro - base background
  surface: "#FFFFFF"        # Blanco - cards, inputs, alternate surfaces
  onSurface: "#000000"      # Negro - primary text, navigation, max contrast
  
  # Semantic aliases (reference tokens)
  ctaPrimary: "{colors.primary}"
  ctaPrimaryText: "{colors.surface}"
  ctaSecondaryBg: "{colors.background}"
  ctaSecondaryTextPrimary: "{colors.primary}"
  ctaSecondaryTextSecondary: "{colors.secondary}"
  linkPrimary: "{colors.secondary}"
  linkSecondary: "{colors.primary}"
  navBackground: "{colors.primary}"
  navText: "{colors.surface}"
  footerBackground: "{colors.onSurface}"
  separator: "{colors.accent}"
  cardBackground: "{colors.surface}"
  cardBackgroundAlt: "{colors.background}"
  cardSupport: "{colors.secondary}"
  hoverIndicator: "{colors.accent}"
  progressIndicator: "{colors.primary}"
  illustrationStroke: "{colors.onSurface}"
  illustrationAccentPrimary: "{colors.primary}"
  illustrationAccentSecondary: "{colors.secondary}"
  illustrationAccentTertiary: "{colors.accent}"

typography:
  # Escalas planas por rol (schema oficial: fontFamily, fontSize, fontWeight, lineHeight, letterSpacing)
  display:
    fontFamily: "Quimby Gobernatorial"
    fontSize: "64px"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "0px"
  h1:
    fontFamily: "Quimby Gobernatorial"
    fontSize: "48px"
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: "0px"
  h2:
    fontFamily: "Quimby Gobernatorial"
    fontSize: "40px"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "0px"
  subtitle:
    fontFamily: "Acumin Variable Concept"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "0px"
  body:
    fontFamily: "Acumin Variable Concept"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "0px"
  listItem:
    fontFamily: "Acumin Variable Concept"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "0px"
  small:
    fontFamily: "Acumin Variable Concept"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "0px"
  buttonLabel:
    fontFamily: "Acumin Variable Concept"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0px"
  link:
    fontFamily: "Acumin Variable Concept"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0px"
  nav:
    fontFamily: "Acumin Variable Concept"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0px"

spacing:
  base: "8px"
  scale:
    - "8px"
    - "16px"
    - "24px"
    - "32px"
    - "48px"
    - "64px"
    - "80px"
    - "96px"
  internal: "12-24px"       # Internal element spacing
  section: "64-96px"        # Section separation
  mobileMargin: "16-24px"   # Mobile section margins
  touchTarget: "44px"       # Minimum touch target

rounded:
  card: "16px"              # Cards and containers
  pill: "9999px"            # Fully rounded / pill shapes (was 50%, now valid px)
  button: "16px"            # Button border radius (matches card)

components:
  # Cada variante = clave de primer nivel con sub-tokens permitidos:
  # backgroundColor, textColor, typography, rounded, padding, size, height, width
  buttonPrimary:
    backgroundColor: "{colors.ctaPrimary}"
    textColor: "{colors.ctaPrimaryText}"
    typography: "{typography.buttonLabel}"
    rounded: "{rounded.button}"
    padding: "0 24px"
    height: "44px"
  buttonSecondary:
    backgroundColor: "{colors.ctaSecondaryBg}"
    textColor: "{colors.ctaSecondaryTextPrimary}"
    typography: "{typography.buttonLabel}"
    rounded: "{rounded.button}"
    padding: "0 24px"
    height: "44px"
  buttonSecondaryAlt:
    backgroundColor: "{colors.ctaSecondaryBg}"
    textColor: "{colors.ctaSecondaryTextSecondary}"
    typography: "{typography.buttonLabel}"
    rounded: "{rounded.button}"
    padding: "0 24px"
    height: "44px"
  card:
    backgroundColor: "{colors.cardBackground}"
    textColor: "{colors.onSurface}"
    typography: "{typography.body}"
    rounded: "{rounded.card}"
    padding: "{spacing.internal}"
  cardAlt:
    backgroundColor: "{colors.cardBackgroundAlt}"
    textColor: "{colors.onSurface}"
    typography: "{typography.body}"
    rounded: "{rounded.card}"
    padding: "{spacing.internal}"
  nav:
    backgroundColor: "{colors.navBackground}"
    textColor: "{colors.navText}"
    typography: "{typography.nav}"
    rounded: "0px"
    padding: "16px 24px"
  linkPrimary:
    textColor: "{colors.linkPrimary}"
    typography: "{typography.link}"
    backgroundColor: "{colors.surface}"
  linkSecondary:
    textColor: "{colors.linkSecondary}"
    typography: "{typography.link}"
    backgroundColor: "{colors.surface}"
  chip:
    backgroundColor: "{colors.background}"
    textColor: "{colors.onSurface}"
    typography: "{typography.small}"
    rounded: "{rounded.pill}"
    padding: "0 12px"
    height: "32px"
  chipAccent:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.surface}"
    typography: "{typography.small}"
    rounded: "{rounded.pill}"
    padding: "0 12px"
    height: "32px"
  separator:
    backgroundColor: "{colors.separator}"
    height: "1px"
  footer:
    backgroundColor: "{colors.footerBackground}"
    textColor: "{colors.surface}"
    typography: "{typography.body}"
    padding: "32px 24px"
  progressIndicator:
    backgroundColor: "{colors.progressIndicator}"
    height: "3px"
    width: "100%"

breakpoints:
  mobile: "320-599px"
  tablet: "600-1023px"
  desktop: "1024px+"

motion:
  reducedMotion: "respect prefers-reduced-motion"
  soundDefault: "muted, user-controlled"
  cursor: "custom, subtle hover response"
  progressIndicator: "top bar, {colors.progressIndicator}"
  headlineAnimation: "handwriting reveal (Quimby Gobernatorial)"
  cardHover: "subtle scale/contrast shift"
  illustrationReveal: "progressive draw, slight displacement"
  transitionDuration: "short, natural"
  easing: "organic, ease-out"
---

# Overview

Mi marca encarna una personalidad creativa, cercana, espontánea y expresiva, construida alrededor de la idea de que el diseño también puede comunicar quién soy y lo que me mueve. "El corazón de Ceci" funciona como el eje conceptual de la identidad: una propuesta que combina sensibilidad, curiosidad y experimentación con una estructura clara y funcional.

La identidad visual equilibra una base suave y neutra con acentos de rojo cálido, azul y turquesa, utilizando el color como recurso para transmitir energía, emoción y personalidad. El rojo representa la parte más humana, apasionada y cercana de la marca; el azul aporta equilibrio y frescura; mientras que el turquesa introduce momentos de sorpresa y experimentación. El negro funciona como ancla y proporciona contraste, definición y legibilidad.

La tipografía establece un diálogo entre lo personal y lo funcional. Las formas manuscritas aparecen como la voz emocional de la marca: espontáneas, humanas y artesanales. En contraste, la tipografía sans serif organiza la información y mantiene la lectura clara. Esta combinación permite que la identidad tenga una voz propia sin perder funcionalidad.

El lenguaje gráfico se construye mediante formas orgánicas, trazos irregulares, estrellas, líneas curvas, ilustraciones y elementos superpuestos. Estos recursos buscan transmitir movimiento y libertad creativa, evitando una estética excesivamente rígida o corporativa. Las ilustraciones, especialmente el autorretrato, funcionan como extensiones de la identidad y hacen que la diseñadora sea parte activa de la experiencia.

La composición mantiene una estructura editorial clara, pero permite cierta espontaneidad dentro de ella. Los elementos pueden desbordar, superponerse o cambiar de escala, generando una sensación de movimiento y descubrimiento. El sistema no busca un minimalismo absoluto, sino un equilibrio entre orden y expresión, estructura y juego, claridad y personalidad.

En una frase: una identidad cálida y gráfica que transforma la personalidad de Ceci en un lenguaje visual espontáneo, colorido y humano, donde cada elemento se siente hecho con el corazón.

# Colors

Mi paleta se construye a partir de tres colores de identidad y tres neutros, creando un equilibrio entre calidez, energía y frescura. El rojo funciona como el color principal de la marca y concentra su carácter emocional; el azul aporta equilibrio y estructura; mientras que el turquesa introduce acentos de experimentación y dinamismo. Los neutros permiten mantener una composición clara y legible sin perder la personalidad gráfica de la identidad.

| Token | Hex | Role | Usage |
|-------|-----|------|-------|
| `colors.primary` | `#B82925` | Rojo corazón | Brand, CTA principal, títulos principales, enlaces prioritarios, máxima atención |
| `colors.secondary` | `#4A6FA5` | Azul creativo (ajustado AA) | Subtítulos, enlaces secundarios, botones secundarios, etiquetas, apoyo visual |
| `colors.accent` | `#00A79D` | Turquesa | **Solo gráfico**: hover decorativo, indicadores, separadores. NUNCA como texto. |
| `colors.background` | `#E7ECE8` | Verde muy claro | Fondo base predominante, secciones principales |
| `colors.surface` | `#FFFFFF` | Blanco | Tarjetas, campos, contenedores, superficies diferenciadas, texto sobre fondos oscuros |
| `colors.onSurface` | `#000000` | Negro | Texto principal, navegación, máximo contraste, apoyo sobre fondos claros |

**Reglas de uso:**
- Usa `{colors.primary}` para los CTA principales y los momentos de mayor énfasis de marca.
- Mantén `{colors.secondary}` como color secundario para información y acciones complementarias.
- Utiliza `{colors.accent}` **solo** para elementos gráficos decorativos (líneas, iconos, hover visual), nunca como texto.
- Mantén `{colors.background}` como fondo base predominante.
- No utilices todos los colores de la paleta con la misma intensidad dentro de un mismo componente.
- No utilices el turquesa como color dominante de la interfaz ni como texto.

# Typography

Uso dos familias tipográficas con roles claramente diferenciados. **Quimby Gobernatorial** es mi tipografía expresiva y principal de identidad: se utiliza en los títulos que buscan comunicar personalidad, cercanía y el carácter hecho a mano de la marca. **Acumin Variable Concept** funciona como tipografía funcional y de lectura: organiza la navegación, subtítulos, cuerpo de texto, botones y contenidos informativos.

## Escala tipográfica (tokens válidos del schema)

| Token | Tamaño | Familia | Peso | Line-height | Uso |
|-------|--------|---------|------|-------------|-----|
| `typography.display` | 64px | Expresiva | 400 | 1.1 | Nombre de marca, titulares de mayor impacto |
| `typography.h1` | 48px | Expresiva | 400 | 1.15 | Encabezados principales de sección |
| `typography.h2` | 40px | Expresiva | 400 | 1.2 | Secciones secundarias |
| `typography.subtitle` | 24px | Funcional | 700 | 1.25 | Subtítulos |
| `typography.body` | 16px | Funcional | 400 | 1.5 | Cuerpo de texto |
| `typography.listItem` | 16px | Funcional | 400 | 1.5 | Ítems de lista |
| `typography.small` | 14px | Funcional | 400 | 1.4 | Texto pequeño |
| `typography.buttonLabel` | 16px | Funcional | 700 | 1 | Etiquetas de botones y CTA |
| `typography.link` | 16px | Funcional | 700 | 1 | Enlaces |
| `typography.nav` | 16px | Funcional | 400 | 1 | Navegación |

**Reglas:**
- La jerarquía siempre se logra mediante tamaño, peso, estilo y color, nunca mediante opacidad.
- El cuerpo de texto nunca baja de 16px para conservar la legibilidad.
- Quimby Gobernatorial se utiliza con moderación, únicamente en títulos, frases y elementos de identidad donde se busca reforzar la personalidad artesanal y cercana de la marca.
- Acumin Variable Concept se reserva para toda la información funcional y de lectura.
- No utilices Quimby Gobernatorial para párrafos largos o información funcional.

# Layout

Mi layout combina una estructura vertical clara con composiciones orgánicas y dinámicas. El contenido se organiza por secciones amplias que permiten que cada bloque tenga su propio espacio visual, mientras que las ilustraciones y elementos decorativos pueden desbordar ligeramente la estructura para generar una sensación espontánea.

## Espaciado

El espaciado se basa principalmente en una escala de 8px (`spacing.base`), utilizando valores de 8, 16, 24, 32, 48, 64, 80 y 96px (`spacing.scale`). Los elementos internos utilizan espacios de 12–24px (`spacing.internal`), mientras que las secciones principales mantienen separaciones de aproximadamente 64–96px (`spacing.section`) para generar pausas visuales.

## Estructura

- El contenido se mantiene dentro de un ancho controlado y centrado.
- En escritorio se utiliza una composición de varias columnas que permite combinar texto, imágenes e ilustraciones.
- En móvil, el contenido se reorganiza principalmente en una sola columna.
- El espacio en blanco es parte fundamental de la identidad. No se busca llenar todos los espacios, sino permitir que los títulos manuscritos, fotografías e ilustraciones tengan suficiente aire para conservar su expresividad.
- La composición puede romper ligeramente la retícula mediante superposiciones, elementos desplazados y recursos gráficos que salen del flujo principal, siempre que no afecten la legibilidad ni la navegación.

## Breakpoints

| Breakpoint | Rango | Comportamiento |
|------------|-------|----------------|
| `breakpoints.mobile` | 320–599px | Una columna, márgenes 16–24px, elementos decorativos reducidos/reposicionados, tarjetas en una columna, fotos mayor ancho |
| `breakpoints.tablet` | 600–1023px | Dos columnas cuando el contenido lo permita, espacios laterales aumentados |
| `breakpoints.desktop` | 1024px+ | Composición editorial completa: navegación horizontal, superposiciones, elementos gráficos alrededor |

- Los elementos interactivos deben mantener un área mínima aproximada de 44 × 44px (`spacing.touchTarget`) para facilitar la interacción táctil.
- Los textos pueden reducir ligeramente su tamaño en móvil, pero el cuerpo nunca debe ser menor a 16px.
- Los titulares manuscritos pueden reducir su tamaño proporcionalmente, manteniendo siempre suficiente espacio para que sus formas no se amontonen.
- Las ilustraciones decorativas pueden cambiar de posición, tamaño o incluso desaparecer en determinados puntos de quiebre cuando sea necesario para priorizar la legibilidad.
- La navegación en móvil se transforma en una estructura compacta que mantiene siempre accesibles las secciones principales: Inicio, Sobre mí, Habilidades, Trabajos y Contacto.

# Elevation & Depth

El diseño es principalmente plano, ya que la identidad se apoya más en el color, la ilustración, la composición y la superposición de elementos que en efectos tridimensionales.

Los fondos, secciones y elementos principales no utilizan sombras de manera constante. La separación entre componentes se genera mediante espacio, color, contraste y posición.

Cuando sea necesario diferenciar una tarjeta, imagen o elemento interactivo del fondo, se puede utilizar una sombra muy suave y difusa, sin convertirla en un recurso dominante.

## Niveles de profundidad

| Nivel | Descripción | Ejemplos |
|-------|-------------|----------|
| Plano | Contenido general sin elevación | Navegación, títulos, textos, ilustraciones |
| Superposición | Elementos que se colocan parcialmente sobre otros | Fotografías, ilustraciones, elementos gráficos superpuestos |
| Elevación sutil | Feedback interactivo ligero | Tarjetas o elementos interactivos durante hover |
| Contraste | Separación visual mediante color de fondo | Secciones con fondos diferenciados |

**Reglas:**
- No utilices sombras profundas o efectos tridimensionales que contradigan el lenguaje plano de la identidad.
- Utiliza el contraste de color y composición antes que sombras para generar jerarquía.

# Shapes

Las formas del sistema son principalmente orgánicas, redondeadas y espontáneas, en contraste con una interfaz basada exclusivamente en geometrías rígidas.

## Radios de borde

| Token | Valor | Uso |
|-------|-------|-----|
| `rounded.card` | 16px | Tarjetas, contenedores, botones |
| `rounded.pill` | 9999px | Formas completamente redondeadas, píldoras, avatares |

- Las tarjetas y contenedores utilizan esquinas redondeadas de aproximadamente 16px.
- Elementos completamente redondeados utilizan `rounded.pill` (9999px) para forma de píldora/círculo.
- Las formas circulares y redondeadas se utilizan para generar contraste con los trazos irregulares de las ilustraciones. Los círculos pueden funcionar como fondos decorativos, fotografías recortadas o elementos de apoyo.
- Las formas gráficas de la identidad pueden ser irregulares, curvas o dibujadas a mano. No necesitan mantener una geometría perfectamente uniforme, ya que la imperfección controlada forma parte de la personalidad de la marca.
- Las ilustraciones y trazos pueden superponerse parcialmente al contenido, pero nunca deben interferir con la lectura ni con los elementos interactivos.

**Reglas:**
- No conviertas cada elemento en una forma redondeada; el redondeo debe utilizarse de manera intencional.
- No sacrifiques legibilidad por una composición experimental.
- No utilices elementos decorativos detrás de textos si reducen el contraste.

# Components

## Botones y CTA

**Primario (CTA principal):**
- `components.buttonPrimary` — Fondo rojo (`{colors.primary}`), texto blanco, 44px alto, radio 16px
- Hover: oscurece rojo ~10% (definir valor exacto en implementación) o escala 1.02x

**Secundario (dos variantes):**
- `components.buttonSecondary` — Fondo verde claro/blanco, texto rojo, borde rojo, 44px alto
- `components.buttonSecondaryAlt` — Fondo verde claro/blanco, texto azul, borde azul, 44px alto

**Reglas:**
- Los botones deben conservar una apariencia cercana y sencilla, evitando estilos excesivamente corporativos o técnicos.
- No dependas únicamente del color para comunicar estados interactivos (usa subrayado, escala, borde).

## Tarjetas y contenedores

- `components.card` — Fondo blanco, texto negro, radio 16px, padding interno 12–24px
- `components.cardAlt` — Fondo verde muy claro, texto negro, radio 16px, padding interno 12–24px
- Color de apoyo: `{colors.cardSupport}` (azul) para etiquetas/categorías
- Las imágenes de proyectos tienen mayor protagonismo que los contenedores.
- Hover: escala 1.02x, borde rojo o sombra sutil `0 4px 12px rgba(0,0,0,0.08)`

## Navegación

- `components.nav` — Fondo rojo (`{colors.primary}`), texto blanco, tipografía `nav`, padding 16px 24px
- Layout: horizontal en escritorio, logo centrado; compacto en móvil
- Estado activo: subrayado o cambio de color (no solo opacidad)

## Enlaces

- `components.linkPrimary` — Color azul (`{colors.secondary}`), tipografía `link`, fondo transparente
- `components.linkSecondary` — Color rojo (`{colors.primary}`), tipografía `link`, fondo transparente
- Hover: subrayado + cambio de color evidente

## Chips / Etiquetas

- `components.chip` — Fondo verde claro, texto negro, radio pill (9999px), altura 32px
- `components.chipAccent` — Fondo azul, texto blanco, radio pill, altura 32px (uso puntual)

## Separadores

- `components.separator` — Color turquesa (`{colors.accent}`), altura 1px
- Uso: únicamente para marcar cambios importantes en la narrativa

## Footer

- `components.footer` — Fondo negro, texto blanco, tipografía `body`, padding 32px 24px
- Mensaje de cierre: "Hecho con el corazón"

## Indicador de progreso

- `components.progressIndicator` — Color rojo (`{colors.primary}`), altura 3px, ancho 100%, posición superior

# Do's and Don'ts

## Do's ✅

- Usa `{colors.primary}` para los CTA principales y los momentos de mayor énfasis de marca.
- Mantén `{colors.secondary}` como color secundario para información y acciones complementarias.
- Utiliza `{colors.accent}` **solo** para elementos gráficos decorativos (líneas, iconos, hover visual), nunca como texto.
- Mantén `{colors.background}` como fondo base predominante.
- Utiliza `typography.display/h1/h2` (Quimby Gobernatorial) principalmente en títulos y mensajes de identidad.
- Utiliza `typography.body/subtitle/buttonLabel/link/nav` (Acumin Variable Concept) para navegación, cuerpo, botones y contenido funcional.
- Mantén suficiente espacio alrededor de los títulos manuscritos y elementos ilustrados.
- Permite superposiciones y desplazamientos gráficos siempre que no afecten la lectura.
- Utiliza el contraste de color y composición antes que sombras para generar jerarquía.
- Mantén una relación constante entre fotografía, ilustración y tipografía.
- Utiliza movimientos suaves y orgánicos.
- Prioriza las ilustraciones y los titulares como elementos animados.
- Utiliza la escritura a mano para los títulos de mayor importancia.
- Utiliza el scroll para revelar progresivamente los contenidos.
- Mantén el cursor personalizado sencillo y funcional.
- Utiliza el rojo como referencia visual para el progreso.
- Permite que el usuario controle el sonido.
- Mantén las animaciones cortas y naturales.
- Respeta la preferencia de reducir movimiento del usuario (`prefers-reduced-motion`).
- El sonido siempre debe poder activarse, pausarse y silenciarse manualmente.

## Don'ts ❌

- No utilices todos los colores de la paleta con la misma intensidad dentro de un mismo componente.
- No utilices el turquesa como color dominante de la interfaz **ni como texto**.
- No utilices Quimby Gobernatorial para párrafos largos o información funcional.
- No sobrecargues las secciones con ilustraciones o elementos decorativos.
- No utilices sombras profundas o efectos tridimensionales que contradigan el lenguaje plano de la identidad.
- No conviertas cada elemento en una forma redondeada; el redondeo debe utilizarse de manera intencional.
- No sacrifiques legibilidad por una composición experimental.
- No utilices elementos decorativos detrás de textos si reducen el contraste.
- No dependas únicamente del color para comunicar estados interactivos.
- No pierdas la estructura editorial de la página por agregar elementos gráficos innecesarios.
- No utilices animaciones bruscas o excesivamente rápidas.
- No animes todos los elementos al mismo tiempo.
- No utilices efectos de escritura en párrafos extensos.
- No reproduzcas sonido automáticamente.
- No hagas que una animación sea necesaria para entender el contenido.
- No utilices efectos 3D o movimientos tecnológicos que contradigan el lenguaje artesanal.
- No utilices el cursor personalizado si dificulta identificar los elementos interactivos.
- No sobrecargues el scroll con demasiadas transiciones.

---

> **NOTA:** Los valores de hover exactos (oscurecer rojo 10%) requieren definición en implementación. Los tokens semánticos referencian otros tokens (ej. `{colors.primary}`) y deben resolverse en la build final.