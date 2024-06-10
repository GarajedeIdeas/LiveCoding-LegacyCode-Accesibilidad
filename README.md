# ♿️ Legacy code y accesibilidad
Evento [Garaje de ideas Live Coding](https://www.youtube.com/watch?v=QspxkW7kheA&ab_channel=Garajedeideas%7CTech) realizado por [Mia Salazar](https://www.linkedin.com/in/miasalazar/)

En este Live Coding hicimos un refactor a un proyecto ya creado realizando mejoras para hacerlo más accesible en diferentes aspectos

## 🍪 Proyecto
* [Proyecto sobre el que se hizo el refactor](https://miasalazar.netlify.app/)
* [Repositorio](https://github.com/Mia-Salazar/cookies)
* [Rama inicial usada en el proyecto](https://github.com/Mia-Salazar/cookies/tree/feat/initial)
* [Rama con el resultado final](https://github.com/Mia-Salazar/cookies/tree/feat/live-coding)

## 🤓 Ejercicios realizados
### 🎯 Navegación por teclado
El primer ejercicio que realizamos fue mejorar la navegación por teclado de la página web.

#### ¿Por qué?
Esta mejora permitirá a las personas que naveguen por teclado poder utilizar la página web, y a todas aquellas personas que utilicen tecnologías asistivas que beban de esa navegación teclado.

#### ¿Qué se hizo?
- Eliminar el `outline: none` permitiendo que haya un indicativo visual de por dónde se está navegando
- Mejorar el `outline` a todos los elementos que tengan el foco para que haya mejor ratio de constraste
- Añadir un link que permita saltar al contenido principal

### 🎯 Encabezados
Se ha agregado encabezados utilizado las etiquetas `<h1> <h2> <h3>`

#### ¿Por qué?
Esta modificación permitirá a las personas que naveguen con tecnologías asistivas, poder conocer los encabezados que hay y su jerarquía.

#### ¿Qué se hizo?
- Modificar un componente `heading` que pintaba encabezados con un `div` y diferentes estilos para que también devuelva el tipo de encabezado
- Añadir etiquetas `<h>`
- Navegamos por encabezados con el lector de pantalla usando la tecla `h`

### 🎯 Estructura básica
Se ha añadido con HTML semántico estructura general al proyecto

#### ¿Por qué?
Agregar esa estructura a las páginas ayuda a las personas que utilicen tecnologías asistivas a entender el orden, estructura y jerarquía que tiene esa web.

#### ¿Qué se hizo?
- Se utilizó las etiquetas `header`, `footer`, `main` y `nav` para crear estructura
- Utilizamos la tecla `d` con el lector de pantallas encendido para ver las diferentes regiones en las que se dividía la web
- Se empleó la etiqueta `ul` para mostrar que un conjunto de elementos eran una lista
- Se pulsó la tecla `l` con el lector de pantallas encendido para entender qué listas hay en el proyecto

### 🎯 Imágenes
Se ha mejorado la accesibilidad de las imágenes

#### ¿Por qué?
Hay personas que no pueden ver las imágenes, o situaciones en las que estas no se ven bien o no cargan, por lo cual hacer estos elementos accesibles ayuda a que no se pierda el contexto de lo que son

#### ¿Qué se hizo?
- Se incorporó la etiqueta `figure` para mejorar la semántica de las imágenes
- Se añadió el atributo `alt` a las imágenes. Si la imagen no era relevante se dejaba vacío, y si era importante, se añadía la descripción
- Utilizamos el lector de pantalla para observar qué información nos daba

### 🎯 Formulario
Se han hecho cambios en el formulario de contacto para mejorar su accesibilidad

#### ¿Por qué?
Si realizamos de forma correcta los formularios, las tecnologías asistivas podrán darnos toda la información para que podamos rellenarlo de forma correcta

#### ¿Qué se hizo?
- Se transformó el componente de elemento de formulario para que tuviese un `label` y estuviese vinculado con el `input` o `textarea`
- Se utilizó un placeholder para dar más información sobre cómo rellenar el formulario

### 🎯 onClick
Se revisaron los elementos que utilizan los `onClick`

#### ¿Por qué?
Si se emplea un `onClick`en un elemento que no es interactivo, no podrá ser navegable por teclado y para las tecnologías asistivas no será posible dar información sobre cuál es el objetivo de ese onClick

#### ¿Qué se hizo?
- Se modificó un `div` que tenía un `onClick` y que redirigía a una página, para que fuese una `<a>`
- Se añadió un `aria-label`a ese link para que tuviese contexto textual ya que dentro solo tenía un icono, y se añadió un `aria-hidden="true"` a ese icono
- Se cambió un `div` que tenía un `onClick` y que hacía función de botón, para que fuese un botón
- Se añadió un `aria-label` a ese botón para que tuviese contexto textual ya que dentro solo tenía elementos gráfico, y se agregaron `aria-hidden="true"`
- Se modificó un filtro que estaba hecho con botones para utilizar `radio inputs` para mejorar su accesibilidad

## 🔗 Recursos
* [Presentación](https://docs.google.com/presentation/d/1b8nGXgL6E3tarq6Ca22HbmGk6fZ8jo2s/edit?usp=sharing&ouid=105566763085813942698&rtpof=true&sd=true)
* Lector de pantalla utilizado, [NVDA](https://nvda.es/)
* Principales [combinaciones de teclas para el lector de pantalla](https://dequeuniversity.com/screenreaders/nvda-keyboard-shortcuts)
* La única plataforma en el mundo donde encontrar restaurantes para personas con alergias e intolerancias, [Foodiesaurus](https://foodiesaurus.com/)
* [Datos sobre discapacidad](https://www.w3.org/WAI/business-case/#:~:text=At%20least%20one%20billion%20people,population%20%E2%80%93%20have%20a%20recognized%20disability&text=As%20the%20population%20ages%2C%20many,a%20%E2%80%9Cperson%20with%20a%20disability%E2%80%9D)
* [Magnificador usado](https://chromewebstore.google.com/detail/zoom-para-google-chrome/lajondecmobodlejlcjllhojikagldgd?hl=es-419)

## 📩 Contacto
Puedes encontrar a Mia Salazar en:
* [Linkedin](https://www.linkedin.com/in/miasalazar/)
* [Twitter](https://x.com/miadeveloper)
* [Medium](https://medium.com/@marasalazar)
* [Dev.to](https://dev.to/miasalazar)
* [GitHub](https://github.com/Mia-Salazar)
* [Codepen](https://codepen.io/MiaSalazar)
* [Email](mailto:maria.sgr@gmail.com)
