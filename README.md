# Taylor Swift — Curriculum Vitae

Práctica de Diseño de Interfaces Web (DAW).

## Archivos

- `index.html`: estructura y contenido del CV.
- `styles.css`: estilos del CV.
- `images/stage-background.svg`: imagen local utilizada como fondo.

## Análisis previo del diseño

Se ha tomado como referencia el CV de Son Goku facilitado por el profesor. La distribución mantiene la misma idea general: una barra lateral con datos personales, competencias, técnicas e idiomas; una cabecera principal; perfil profesional; experiencia; formación mediante tarjetas; logros; técnicas/eras y una tabla final.

### Partes y tecnología utilizada

| Parte | Tecnología |
|---|---|
| CV general | CSS Grid |
| Barra lateral | Grid + Flexbox |
| Cabecera | Flexbox |
| Perfil profesional | Grid |
| Experiencia | Flexbox para los títulos |
| Formación | Grid + tarjetas |
| Logros y eras | Grid + Flexbox |
| Tabla final | Tabla HTML + overflow responsive |
| Etiquetas de eras | Flexbox |
| Responsive | Media Query |

### Clases reutilizables

Se han reutilizado clases para elementos con el mismo aspecto: `.side-section`, `.skill`, `.tags`, `.card`, `.experience`, `.badge`, `.content-section` y `.section-heading`.

### Diseño responsive

Se ha utilizado **Desktop First**, igual que la referencia visual principal del profesor. Primero se construye la distribución de escritorio y después, mediante Media Queries, se adapta a pantallas más pequeñas.

Se utilizan dos puntos de adaptación:

- `max-width: 48rem`: la barra lateral pasa a la parte superior, el perfil pasa a una columna y las secciones de dos columnas se apilan.
- `max-width: 34rem`: se simplifica todavía más la barra lateral y las tarjetas pasan a una única columna.

El objetivo es que el contenido se adapte a la anchura disponible y no a un dispositivo concreto.

## Requisitos CSS del enunciado

- `box-sizing: border-box`: aplicado mediante el selector universal.
- Bordes redondeados: variable `--radio` y `--radio-grande`.
- Variables CSS: colores, radios, espacios y sombra.
- `rem`: utilizado en tamaños de letra y medidas principales.
- `calc()`: utilizado en el margen del pie.
- `min()`: utilizado para limitar la anchura del CV.
- Imagen de fondo: `stage-background.svg`.
- Gradiente: utilizado en el fondo general, perfil y bloques de imagen.
- Tarjetas adaptables: sección de formación con Grid y Media Queries.
- Grid: estructura principal, perfil, tarjetas y dos columnas.
- Flexbox: etiquetas, metadatos, títulos y pie.
- Responsive: Media Queries.
- `!important`: no se utiliza.

## Fuentes de información

Los datos biográficos y de trayectoria se han contrastado con la página de Taylor Swift en GRAMMY y con la web oficial de Taylor Swift. El contenido se ha reducido para mantener una cantidad y distribución de información similares al ejemplo de clase.
