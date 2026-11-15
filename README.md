# Bitácora — Rueda Libre

## URL de GitHub Pages

<https://blairsawyer17.github.io/RuedaLibre/>

---

## Peticiones HTTP observadas

**Petición 1**

- **URL:** `http://127.0.0.1:5500/index.html`
- **Protocolo:** `http://`
- **Host:** `127.0.0.1:5500`
- **Puerto:** `5500`
- **Ruta:** `index.html`
- **Método de petición:** `GET`
- **Código de estado:** `304 Not Modified`

**Petición 2**

- **URL:** `http://127.0.0.1:5500/RuedaLibre/promociones.html`
- **Método de petición:** `GET`
- **Código de estado:** `404 Not Found`

---

## Rol de cada lenguaje

- **HTML:** Con este lenguaje crearemos toda la estructura de la página. Se establecerá el orden de las secciones, de los títulos, tablas, páginas, enlaces, imágenes, textos y demás, siguiendo una nomenclatura semántica que permita la legibilidad de la página y la accesibilidad a la misma.
- **CSS:** Con las hojas de estilo estableceremos las reglas de diseño como el formato de los títulos, subtítulos y párrafos; los colores de las letras, del fondo, listas, secciones, etc.; crearemos las animaciones; organizaremos los "bloques" para que la página se vea bonita; y haremos que la página sea *responsive* para que pueda visualizarse bien en cualquier dispositivo.
- **JavaScript:** Con este lenguaje de programación haremos funcional la página.

---

## Tabla de rutas

| Archivo de origen | Destino | Ruta escrita |
|---|---|---|
| `index.html` | `paginas/tarifas.html` | `./paginas/tarifas.html` |
| `index.html` | `paginas/reservas.html` | `./paginas/reservas.html` |
| `paginas/reservas.html` | `css/style.css` | `../css/style.css` |
| `paginas/tarifas.html` | `css/style.css` | `../css/style.css` |
| `paginas/reservas.html` | `paginas/tarifas.html` | `./tarifas` |
| `paginas/reservas.html` | `index.html` | `../index.html` |
| `index.html` | `css/style.css` | `./css/style.css` |
| `paginas/tarifas.html` | `index.html` | `../index.html` |
| `paginas/tarifas.html` | `paginas/reservas.html` | `./reservas` |

---

## Esquema de regiones

### Página: `index.html`

```text
PÁGINA: index.html
|
|-- ENCABEZADO (header)
|   |
|   |-- Logo (a > img)
|   |
|   |-- NAVEGACIÓN (nav)
|       |
|       |-- Lista de enlaces (ul)
|           |-- Inicio
|           |-- Nosotros
|           |-- Servicios
|           |-- Contacto
|           |-- Tarifas
|           |-- Reservas
|
|-- CONTENIDO PRINCIPAL (main)
|   |
|   |-- SECCIÓN: Bienvenida (section)
|   |   |-- Título principal (h1)
|   |   |-- Texto de bienvenida (p)
|   |
|   |-- SECCIÓN: Nosotros (section)
|   |   |-- Título de sección (h2)
|   |   |-- Descripción de la empresa (p)
|   |
|   |-- SECCIÓN: Servicios (section)
|   |   |-- Título de sección (h2)
|   |   |
|   |   |-- ARTÍCULO: Alquiler de bicicletas (article)
|   |   |   |-- Título del servicio (h3)
|   |   |   |-- Descripción (p)
|   |   |   |-- Enlace para reservar (a)
|   |   |   |-- Imagen del servicio (img)
|   |   |
|   |   |-- ARTÍCULO: Rutas guiadas (article)
|   |   |   |-- Título del servicio (h3)
|   |   |   |-- Descripción (p)
|   |   |   |-- Enlace a las rutas (a)
|   |   |   |-- Imagen del servicio (img)
|   |   |
|   |   |-- ARTÍCULO: Taller básico (article)
|   |       |-- Título del servicio (h3)
|   |       |-- Descripción (p)
|   |       |-- Imagen del servicio (img)
|   |
|   |-- SECCIÓN: Cómo alquilar (section)
|   |   |-- Título de sección (h2)
|   |   |-- Subtítulo (h3)
|   |   |-- Descripción introductoria (p)
|   |   |-- Lista ordenada de pasos (ol)
|   |   |-- Subtítulo: Beneficios de alquilar (h3)
|   |   |-- Lista de beneficios (ul)
|   |   |-- Enlace a las tarifas (a)
|   |
|   |-- SECCIÓN: Nuestra flota (section)
|   |   |-- Título de la flota (h2)
|   |   |-- Contenedor de artículos (div)
|   |       |
|   |       |-- Artículo: Urbana Clásica (article)
|   |       |   |-- Imagen bicicleta (img)
|   |       |   |-- Contenedor información de bicicleta (div)
|   |       |       |-- Título bicicleta (h3)
|   |       |       |-- Descripción bicicleta (p)
|   |       |       |-- Precio alquiler bicicleta (p)
|   |       |       |-- Enlace a reservas (a)
|   |       |
|   |       |-- Artículo: Bicicleta urbe pegable (article)
|   |       |   |-- Imagen bicicleta (img)
|   |       |   |-- Contenedor información de bicicleta (div)
|   |       |       |-- Título bicicleta (h3)
|   |       |       |-- Descripción bicicleta (p)
|   |       |       |-- Precio alquiler bicicleta (p)
|   |       |       |-- Enlace a reservas (a)
|   |       |
|   |       |-- Artículo: Bicicleta montaña trail (article)
|   |       |   |-- Imagen bicicleta (img)
|   |       |   |-- Contenedor información de bicicleta (div)
|   |       |       |-- Título bicicleta (h3)
|   |       |       |-- Descripción bicicleta (p)
|   |       |       |-- Precio alquiler bicicleta (p)
|   |       |       |-- Enlace a reservas (a)
|   |       |
|   |       |-- Artículo: Bicicleta gravel aventura (article)
|   |       |   |-- Imagen bicicleta (img)
|   |       |   |-- Contenedor información de bicicleta (div)
|   |       |       |-- Título bicicleta (h3)
|   |       |       |-- Descripción bicicleta (p)
|   |       |       |-- Precio alquiler bicicleta (p)
|   |       |       |-- Enlace a reservas (a)
|   |       |
|   |       |-- Artículo: Bicicleta eléctrica urbana (article)
|   |       |   |-- Imagen bicicleta (img)
|   |       |   |-- Contenedor información de bicicleta (div)
|   |       |       |-- Título bicicleta (h3)
|   |       |       |-- Descripción bicicleta (p)
|   |       |       |-- Precio alquiler bicicleta (p)
|   |       |       |-- Enlace a reservas (a)
|   |       |
|   |       |-- Artículo: Bicicleta infantil (article)
|   |           |-- Imagen bicicleta (img)
|   |           |-- Contenedor información de bicicleta (div)
|   |               |-- Título bicicleta (h3)
|   |               |-- Descripción bicicleta (p)
|   |               |-- Precio alquiler bicicleta (p)
|   |               |-- Enlace a reservas (a)
|   |
|   |-- SECCIÓN: Encuéntranos (section)
|       |-- Título de sección (h2)
|       |-- Información de contacto introductoria (p)
|       |
|       |-- CONTENEDOR DEL MAPA (div)
|       |   |-- Subtítulo: Visítanos en (h3)
|       |   |-- Mapa de ubicación (iframe)
|       |
|       |-- Información de contacto (address)
|           |-- Enlace de correo electrónico (a)
|
|-- PIE DE PÁGINA (footer)
    |-- Nombre del sitio, correo y año
```

### Página: `reservas.html`

```text
PÁGINA: reservas.html
|
|-- ENCABEZADO (header)
|   |
|   |-- Logo (a > img)
|   |
|   |-- NAVEGACIÓN (nav)
|       |
|       |-- Lista de enlaces (ul)
|           |-- Inicio
|           |-- Nosotros
|           |-- Servicios
|           |-- Contacto
|           |-- Tarifas
|           |-- Reservas
|
|-- CONTENIDO PRINCIPAL (main)
|   |
|   |-- SECCIÓN: Horarios y contacto (section)
|   |   |
|   |   |-- Contenedor de título y correo (div)
|   |   |   |-- Título principal (h1)
|   |   |   |-- Correo electrónico (p > a)
|   |   |
|   |   |-- CONTENIDO COMPLEMENTARIO (aside)
|   |       |-- Lista de definiciones (dl)
|   |           |-- Días de atención (dt)
|   |           |-- Horario (dd)
|   |           |-- Días de atención (dt)
|   |           |-- Horario (dd)
|   |
|   |-- SECCIÓN: Formulario de reservas (section)
|       |
|       |-- Título de sección (h2)
|       |
|       |-- Formulario (form)
|           |
|           |-- GRUPO: Tus datos (fieldset)
|           |   |-- Nombre completo (label + input)
|           |   |-- Tipo de documento (label + select)
|           |   |-- Número de documento (label + input)
|           |   |-- Correo electrónico (label + input)
|           |   |-- Celular (label + input)
|           |
|           |-- GRUPO: Tu alquiler (fieldset)
|           |   |-- Fecha de alquiler (label + input)
|           |   |-- Tipo de bicicleta (label + select)
|           |   |-- Plan de alquiler (label + select)
|           |   |-- Número de bicicletas (label + input)
|           |   |-- Recorrido guiado (label + select)
|           |
|           |-- GRUPO: Confirmación (fieldset)
|           |   |-- Comentarios (label + textarea)
|           |   |-- Términos y condiciones (p)
|           |   |-- Aceptación de términos (input checkbox + label)
|           |   |-- Confirmación de reserva (input checkbox + label)
|           |
|           |-- Botón de envío (button)
|
|-- PIE DE PÁGINA (footer)
    |-- Nombre del sitio, correo y año
```

### Página: `tarifas.html`

```text
PÁGINA: tarifas.html
|
|-- ENCABEZADO (header)
|   |
|   |-- Logo (a > img)
|   |
|   |-- NAVEGACIÓN (nav)
|       |
|       |-- Lista de enlaces (ul)
|           |-- Inicio
|           |-- Nosotros
|           |-- Servicios
|           |-- Contacto
|           |-- Tarifas
|           |-- Reservas
|
|-- CONTENIDO PRINCIPAL (main)
|   |
|   |-- SECCIÓN: Tarifas de alquiler (section)
|   |   |
|   |   |-- Tabla de tarifas (table)
|   |       |-- Título de tabla (caption)
|   |       |-- Encabezados de columnas (thead)
|   |       |   |-- Tipo de bicicleta
|   |       |   |-- 1 hora
|   |       |   |-- Medio día
|   |       |   |-- Día completo
|   |       |
|   |       |-- Datos de tarifas (tbody)
|   |           |-- Bicicleta urbana (tr)
|   |           |-- Bicicleta de montaña (tr)
|   |           |-- Bicicleta eléctrica (tr)
|   |
|   |-- SECCIÓN: Tarifas de recorridos guiados (section)
|   |   |
|   |   |-- Tabla de recorridos (table)
|   |   |   |-- Título de tabla (caption)
|   |   |   |-- Encabezados de columnas (thead)
|   |   |   |   |-- Recorrido
|   |   |   |   |-- Distancia
|   |   |   |   |-- Duración
|   |   |   |   |-- Nivel
|   |   |   |   |-- Precio por persona
|   |   |   |
|   |   |   |-- Datos de recorridos (tbody)
|   |   |       |-- Río y Parques (tr)
|   |   |       |-- Sabores de Barrio (tr)
|   |   |       |-- Reto Las Palmas (tr)
|   |   |
|   |   |-- Enlace para reservar (a)
|   |
|   |-- SECCIÓN: Descripción y requisitos (section)
|       |
|       |-- Información sobre tarifas y horarios (p)
|       |
|       |-- CONTENIDO COMPLEMENTARIO (aside)
|           |-- Lista de requisitos (ul)
|               |-- Ropa cómoda (li)
|               |-- Agua (li)
|               |-- Protector solar (li)
|               |-- Documento de identidad (li)
|
|-- PIE DE PÁGINA (footer)
    |-- Nombre del sitio, correo y año
```

---

## Justificación de los `div`

### En `index.html`

- `<div class="container-content container-content-servicios">`: Me sirve para crear un bloque que separa el título de los `article` que contienen los servicios y así facilitar su diseño en CSS.
- `<div class="container-encuentranos-content encuentranos-map">`: En este caso no busco dar información complementaria ni información aparte, solo busco encapsular esa parte del contenido para su diseño en CSS.

### En `reservas.html`

- `<div class="form-group">`: No busca dar información complementaria o secundaria, solo agrupa conjuntos de `label` + `input` del mismo `form` para separarlos en pequeños contenedores que después harán más fácil organizar su diseño y visualización estética por medio de CSS. El orden jerárquico y la estructura semántica no se ven afectados.

---

## Pruebas del formulario

**Formulario de reservas — Rueda Libre**

| N.º | Campo | Dato de prueba | Resultado esperado | Resultado obtenido |
|:---:|---|---|---|---|
| 01 | Nombre completo | `123456` | Error/Aviso, error de formato | El esperado |
| 02 | Nombre completo | `Ana` | Bien/Sin ningún aviso | El esperado |
| 03 | Tipo de documento | No seleccionar opción | Error/Aviso, debe elegir una opción | El esperado |
| 04 | Número de documento | `abc1234` | Error/Aviso, error de formato | El esperado |
| 05 | Número de documento | `12345` | Error/Aviso, debe tener mínimo 6 dígitos | El esperado |
| 06 | Número de documento | `12345678901` | Error/Aviso, debe tener máximo 10 dígitos | El esperado |
| 07 | Correo electrónico | `ana-correo.com` | Error/Aviso, falta `@` | El esperado |
| 08 | Correo electrónico | `ana@dominio` | Error/Aviso, debe tener una extensión | Bien/Deja continuar |
| 09 | Celular | `1234567890` | Error/Aviso, debe empezar con 3 | El esperado |
| 10 | Celular | `300123456` | Error/Aviso, debe tener 10 dígitos | El esperado |
| 11 | Celular | `30012345678` | Error/Aviso, debe tener 10 dígitos | El esperado |
| 12 | Fecha de alquiler | Fecha anterior al mínimo | Error/Aviso, fecha fuera del rango | El esperado |
| 13 | Fecha de alquiler | Fecha posterior al máximo | Error/Aviso, fecha fuera del rango | El esperado |
| 14 | Fecha de alquiler | No seleccionar fecha | Error/Aviso, debe elegir una fecha | El esperado |
| 15 | Tipo de bicicleta | No seleccionar opción | Error/Aviso, debe elegir una opción | El esperado |
| 16 | Plan de alquiler | No seleccionar opción | Error/Aviso, debe elegir una opción | El esperado |
| 17 | Número de bicicletas | `0` | Error/Aviso, el número debe ser mínimo 1 | El esperado |
| 18 | Número de bicicletas | `7` | Error/Aviso, el número debe ser máximo 6 | El esperado |
| 19 | Número de bicicletas | `2.5` | Error/Aviso, error de formato | El esperado |
| 20 | Recorrido guiado | No seleccionar opción | Error/Aviso, debe elegir una opción | El esperado |
| 21 | Comentarios | Texto de más de 300 caracteres | No permite escribir más | El esperado |
| 22 | Términos y condiciones | No marcar la casilla | Error/Aviso, debes marcar la casilla | El esperado |

---

## Paleta de colores

| Color | Código | Uso que propone el cliente |
|---|---|---|
| Verde Ruta | `#1E7A4F` | Botones y enlaces |
| Naranja Pedal | `#F39A2B` | Destacados y botones secundarios |
| Azul Noche | `#14213D` | Títulos y encabezado |
| Crema | `#FAF6EF` | Fondo general |
| Gris Asfalto | `#5B6470` | Texto secundario |

---

## Comprobación de contraste

| Combinación | Ratio | Texto normal | Texto grande | No apto |
|---|:---:|:---:|:---:|:---:|
| Texto blanco sobre Verde Ruta | 5.31:1 | Solo AA | X | |
| Texto blanco sobre Naranja Pedal | 2.21:1 | | | X |
| Texto Azul Noche sobre Naranja Pedal | 7.2:1 | X | X | |
| Texto Azul Noche sobre Crema | 14.82:1 | X | X | |
| Texto Gris Asfalto sobre Crema | 5.56:1 | Solo AA | X | |
| Texto Verde Ruta sobre Crema | 4.93:1 | Solo AA | X | |
| Texto Naranja Pedal sobre Crema | 2.05:1 | | | X |
| Texto blanco sobre Azul Noche | 15.97:1 | X | X | |

---

## Mapa de colores

| Color | Código | Uso |
|---|---|---|
| Verde Hoja | `#286044` | Encabezado, navegación, títulos y pie de página |
| Naranja Pedal | `#F39A2B` | Destacados y botones secundarios |
| Verde Carbón | `#202c25` | Títulos y encabezado |
| Crema | `#FAF6EF` | Fondo general |
| Gris Asfalto | `#5B6470` | Texto secundario |

---

## Propiedades

- **Heredadas:** Si el elemento hijo no tiene valor, lo toma del elemento padre.

  En `index.html`, el `<h2 class="title nosotros-title">` hereda `color: var(--text-color);` del `body` de `style.css`.

- **No heredadas:** Si no tienen valor, lo toman del estándar de CSS.

  El mismo `h2` tiene este valor por defecto: `h2 { display: block; }`.

---

## Observación con flexbox

**Header y footer:** Al achicar la ventana se puede evidenciar cómo los elementos dentro de estos se van acoplando a la ventana gracias al `flex-wrap`, cosa que antes no pasaba. Ahora los elementos se mueven automáticamente para ajustarse a la pantalla.

---

## Observación de la flota con DevTools

Los artículos se van acomodando para no ser más pequeños que el tamaño mínimo establecido:

- En **1280px** se ven 3 artículos por fila.
- En **900px** se ven 2 artículos por fila.
- En **500px** se ve 1 artículo por fila.

---

## Flexbox o Grid

- **Portada:** Me tomé un par de licencias creativas. Utilicé la imagen como fondo y el contenido de texto en un `div` para poder difuminar el fondo y que sea legible. El contenido sí lleva flexbox para organizarlo en columna. Al ser solo una línea, no vi necesario usar grid.
- **Galería:** En la galería de rutas decidí convertirla en un carrusel para que la página se vea más dinámica, razón por la cual utilicé flexbox para poder deslizarlas en horizontal.
- **Formulario:** Aquí sí seguí las indicaciones al pie de la letra. Utilicé grid para dividir la página `reservas.html` en dos columnas: una de `2fr` (la que tiene el formulario) y otra de `1fr` (la que tiene el horario). A su vez, utilicé grid para dividir el formulario en 2 columnas iguales en su tamaño para PC y en una columna para móvil y tablet.
- **Encabezado y pie de página:** En ambos utilicé flexbox, tanto para la etiqueta padre como para los hijos. En el encabezado me sirvió para el menú hamburguesa en la versión móvil y de tablet, para desplegar el navbar en columna, y para el navbar visible y en fila en la versión de PC, además de mantener el espacio entre el logo y el navbar (o menú hamburguesa, dependiendo de la resolución) del mismo tamaño para que queden en las esquinas del header. Por otra parte, en el pie de página se utilizó flexbox para separar en fila los artículos (Marca, contacto y horario), además de que haga `wrap` si se queda sin espacio, y para organizar el contenido de cada uno en columnas.

---

## Enfoque mobile-first: correcciones

### Index

- En la media query de `1200px`, en el apartado de rutas, la parte de `ruta-info` se veía descompensada y extraña. Tuve que ajustar el `margin` para centrar bien el contenedor y que no se fusionara entre el fondo del padre y su hermano.
- En el carrusel de rutas, en la media query base, el carrusel no centraba las tarjetas automáticamente. Había olvidado colocar el desplazamiento en x en `scroll-snap-type: x mandatory;`.

### Reservas

- En el formulario, en el cajón de comentarios en la media query de `1200px`, el cajón ocupaba `1fr`, por lo que se veía extraño, así que usé `grid-column` para ajustar su tamaño y que ocupe `2fr` (todo el contenedor).
- También, en la confirmación del formulario, corregí la posición de los `label` del checkbox para que queden alineados verticalmente usando flexbox.

---

## Flota en Bootstrap: comparación

| Comparativa | CSS puro | Bootstrap |
|---|---|---|
| **Tiempo invertido** | 5 minutos | 30 minutos |
| **Línea de código** | Se usaron líneas más largas como `display: flex;`, `display: grid;`, `grid-template-columns;`, etc., sin contar la repetición para los breakpoints del responsive. | Sus líneas fueron más cortas: `gap-4`, `row`, `col-12`, `col-md-4`, `btn`, etc. Muchísimo más cortas que en CSS, pero puede tardar un poco más al tener que repetirse por etiqueta, a menos que lo hagas con Emmet desde la construcción del HTML. |
| **Esfuerzo** | Tienes que ser creativo si quieres un diseño bonito; tienes que pensar muy bien en el diseño, la composición, los colores y muchas otras cosas, por lo que si no eres muy bueno en diseño puedes terminar creando una página mediocre. | Tiene estilos prediseñados que se pueden utilizar con sus respectivas clases, lo que puede ahorrar algunos minutos de código. |
| **Control** | Te permite tener control absoluto sobre el diseño: desde los colores, los cientos de parámetros, grosores, botones, filas, columnas, etc. Sacrificas tiempo por diseño. | Si bien ahorra tiempo y tiene estilos prediseñados, si se utiliza únicamente Bootstrap las páginas pueden verse muy genéricas o similares a muchas páginas, por lo que lo ideal es siempre utilizarlo junto a CSS. |

> **Nota:** En mi caso me demoré mucho más con Bootstrap porque es mi primera vez usándolo, cuando ya tengo mucha más experiencia con CSS, y porque no utilicé las clases de `card` de Bootstrap. Sé que lo pedía el reto de manera indirecta, pero quería conservar el estilo de las cards que tengo en mi CSS original, aunque solo con Bootstrap me fue imposible recrearlo.
>
> **Actualización:** Decidí dejar de intentar recrear mi diseño original con Bootstrap y usar la clase `card` de Bootstrap.

---

## Clases de Bootstrap

Navegando por la documentación encontré estas clases que, si bien no usé todas en esta ocasión, me parecieron interesantes.

- **`.hover-lift`:** Al pasar el mouse por la etiqueta, esta se levanta ligeramente y le da un pequeño sombreado inferior.
- **`.img-fluid`:** Hace que la imagen sea responsive; es el equivalente a usar `width: 100%;` y `height: auto;` en CSS.
- **`.accordion`:** Hace un desplegable perfectamente funcional junto con las clases `.accordion-item`, `.accordion-header` y `.accordion-button`, además de los atributos `data-bs-toggle="collapse"`, `data-bs-target="#idDelElementoADesplegar"`, `aria-expanded="true"` y `aria-controls="idDelElementoADesplegar"`. En el elemento a desplegar se usan `.accordion-collapse`, `.collapse`, `.show` y `data-bs-parent="#idDelDesplegable"`.
- **`.btn-outline-*`:** Hace que los botones no tengan fondo, sino que el borde y el texto se ponen del color del tipo de variante que se le asigne. Por ejemplo, si se escribe `class="btn btn-outline-success"`, entonces será verde.
- **`.carousel` y `.slide`:** Permiten crear un carrusel con flechas para moverse entre elementos. Sus hijos y nietos usan: `.carousel-inner`, `.carousel-item`, `.active`, `.carousel-control-prev`, `.carousel-control-prev-icon`, `.carousel-control-next`, `.carousel-control-next-icon` y `.visually-hidden`.

---

## Tres conflictos entre `bootstrap.css` y Bootstrap

1. **`.container` propio frente a `.container` de Bootstrap:** La regla propia fijaba ancho, márgenes, padding y bordes, por lo que podía imponerse sobre el contenedor responsive de Bootstrap. Se eliminó el selector genérico y se trasladó el espaciado al marcado con utilidades como `my-4`, `py-4` y `p-4`.

2. **Botones propios frente a variantes de Bootstrap:** La regla propia `.btn`, cargada después de Bootstrap, podía pisar el fondo y el color de `.btn-warning`. Se limitó el estilo heredado a `.btn:not(.btn-warning)` y su estado `hover`, dejando intacta la variante amarilla de las tarjetas de flota.

3. **Enlaces, tipografía y márgenes globales:** `a { color: inherit }` podía neutralizar el color de enlace de Bootstrap; además, el tamaño fijo del título y el párrafo de la portada podía imponerse sobre `display-3` y `lead`. Se eliminó el color heredado global y se restringió a `header a`; el tamaño del encabezado y del texto principal se delegó a `display-3` y `lead`. Las utilidades `mb-0` controlan los márgenes puntuales de esos párrafos.

---

## Migración de tarifas y reservas a Bootstrap: comparativa final

**N.º de líneas:** En la versión 1.5 de Rueda Libre, el CSS (`mobile-first.css`) cuenta con 1129 líneas, mientras que con Bootstrap el CSS pasa a tener 769. Sin embargo, en tiempo de ejecución todo el CSS me tomó entre 4 y 5 horas, mientras que Bootstrap me tomó unas 5 horas solamente para `tarifas.html`, `reservas.html` y las secciones de ruta, flota y beneficios en `index.html`. Esto, porque como mencioné anteriormente, siempre he trabajado con CSS en lugar de Bootstrap.

### Resumen de la migración

- **`tarifas.html`:** `.row` con dos columnas desde `lg` (`col-lg-8` con las dos tablas apiladas y `col-lg-4` con la información complementaria). Las tablas van en `.table-responsive` y conservan sus estilos (`.tabla`).
- **`reservas.html`:** formulario (`col-md-8`) y contacto (`col-md-4`). Los campos cortos usan `.row g-3` con `col-sm-6`. Todos los atributos de validación nativa (`required`, `pattern`, `min`, `max`, `minlength`, `maxlength`, `type`, `title`) se mantuvieron sin cambios.

### Ventajas observadas

- La distribución (columnas, huecos, apilado en móvil) se resuelve con clases en el HTML y desaparece del CSS propio: no hay media queries de layout que mantener.
- `.table-responsive`, `.form-control`, `.form-select` y `.form-check` dan un comportamiento consistente (scroll de tablas, tamaño táctil, estados) sin reglas propias.
- El CSS propio quedó reducido a la identidad visual, así que es más fácil de leer y de cambiar (basta tocar las variables).
- Las tarjetas ahora se definen una sola vez con las variables `--bs-card-*`.

### Desventajas observadas

- El *reboot* de Bootstrap cambia cosas que antes no existían: el `caption` de las tablas pasa abajo (hubo que forzar `caption-side: top`), el `legend` se vuelve `float` y los `fieldset` pierden borde y padding.
- El HTML queda más cargado de clases (por ejemplo `card bg-white h-100`, `col-12 col-sm-6`) y cuesta más leerlo a primera vista.
- Hay que cuidar el orden de carga y la especificidad: `bootstrap.css` va después de Bootstrap y algunas utilidades (`!important`, como `bg-white` o `rounded-3`) ganan siempre.
- Se depende de un CDN y hay que aprender los nombres de las clases y los breakpoints.

---

## Comprobación de campos con script de Bootstrap

- El campo del correo electrónico sigue aceptando correos sin la extensión, con tener el nombre del usuario, la arroba (`@`) y el dominio. El resto de los campos funcionan perfectamente.
- Al darle enviar con alguno o varios campos mal, se marcan en rojo todos los campos que están mal. Sin embargo, al intentar enviar el formulario con los datos bien sale un error 404 y, aunque se recargue la página, sigue sin funcionar; toca modificar la URL manualmente para regresar.

---

## Resumen semana 2

Bootstrap resuelve muy bien la distribución y los componentes repetitivos (grilla, formularios, tablas responsive), y dejar en `bootstrap.css` solo la identidad visual evita pelear con él. Aun así, la identidad (colores, tipografía, estados) y los ajustes al *reboot* siguen siendo CSS propio, por lo que lo más sensato es usar Bootstrap junto con CSS propio y no en lugar de él.

Sinceramente, no soy muy buena con Bootstrap, me cuesta un poco compaginar Bootstrap con CSS y soy consciente de los errores que se tienen visualmente en esta versión beta 2.0; traté de emularlo lo más posible al CSS que tenía en un principio, pero me cuesta bastante, por lo que tardé muchísimo más. Cuando yo hago páginas, por lo general estructuro el HTML pensando en el CSS que haré después, por eso mis clases y estructura tienen un propósito claro que, al pasarlo a Bootstrap, siento que fue un poco complicado y difícil de emular.

Para mi estilo de hacer las cosas, implementar Bootstrap puede ser más tedioso, ya que es un poco limitante en el control y yo prefiero modificar todo, por lo que no me parece tan rentable salvo por algunas cosas, como los scripts que maneja para los modales, los carruseles, las validaciones, alertas y demás; pero para el estilo de la página en general, en lo personal, me parece mejor seguir solo con CSS.

> **Nota:** No pude integrar las imágenes del antes y después de Rueda Libre de solo con Bootstrap y luego de Bootstrap con CSS, porque mientras iba implementando Bootstrap iba cambiando las cosas en el CSS para adaptarlo al estilo de la versión 1.0.