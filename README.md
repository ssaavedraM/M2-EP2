# Tarea1 : Desarrollo de la Página Web de un Hospital

## Descripción

El siguiente proyecto muestra el entregable "Ejercicio Práctico 2" que considera mejorar la modularización de estilos y en asegurar que el sitio sea completamente responsivo. Esto implica la implementación de una metodología como BEM, el uso de SASS para estructurar el CSS de manera eficiente, y la aplicación de media queries para lograr una correcta adaptabilidad en dispositivos de diferentes tamaños.

## Instrucciones para Visualizar el Proyecto

1. Clone o descargue el repositorio en su máquina.
2. Navegue hasta la carpeta del proyecto.
3. Abra el archivo `index.html` en el navegador web. Puede hacerlo de las siguientes maneras:
   - Haciendo doble clic sobre el archivo `index.html`.
   - Abriendo el navegador y arrastrando el archivo `index.html` a la ventana del navegador.

## Estructura de Carpetas y Archivos

    .
    ├── index.html             # Página de inicio
    ├── team.html              # Página del equipo médico
    ├── contact.html           # Página de contacto
    ├── scss/
    │   ├── abstracts/
    │   │   ├── _mixins.scss
    │   │   └── _variables.scss
    │   ├── base/
    │   │   ├── _base.scss
    │   │   ├── _reset.scss
    │   │   └── _typography.scss
    │   ├── components/
    │   │   ├── _button.scss
    │   │   ├── _card.scss
    │   │   └── _form.scss
    │   ├── layout/
    │   │   ├── _footer.scss
    │   │   └── _form.scss
    │   ├── pages/
    │   │   ├── _contact.scss
    │   │   ├── _home.scss
    │   │   └── _team.scss
    │   ├── theme/
    │   │   ├── _dark.scss
    │   │   └── _light.scss
    │   └── vendors/
    │   │   └── _normalize.scss
    │   ├── main.css
    │   ├── main.css.map
    │   └── main.scss
    ├── img/
    │   ├── icons/
    │   │   ├── medical_attention.svg
    │   │   ├── medical_emergencies.svg
    │   │   ├── medical_specialities.svg
    │   │   └── person.svg
    │   ├── doctor1.png
    │   ├── doctor2.png
    │   ├── doctor3.png
    │   ├── doctor4.png
    │   └── logo.png
    └── README.md

## Explicación de cada vista

- Home (index.html): Página principal donde se podrán encontrar los servicios que el hospital ofrece junto a testimonios de los pacientes.
- Equipo Médico (team.html): Página donde se puede encontrar información de los distintos doctores que atienden en el hospital, junto a sus especialidades.
- Contacto (contact.html): Página con formulario de contacto para establecer comunicación con el Hospital. Posee un Mapa embebido mostrando la ubicación del Hospital.

## Implementación de la Modularización de Estilos y Media Queries

Se utiliza SASS siguiendo el patrón de arquitectura 7-1, utilizando de base el siguiente recurso: https://github.com/tanrax/pattern-7-1.

# Media Queries
Se implementan media queries para asegurar que el sitio web sea completamente responsivo, adaptándose a diferentes tamaños de pantalla (dispositivos móviles, tablets y pantallas de escritorio). Se establecen tres puntos de ruptura principales:

- Pantallas pequeñas (small): Menos de 768px.
- Pantallas medianas (medium): Entre 768px y 1024px.
- Pantallas grandes (large): Más de 1024px.

En el archivo `scss/abstracts/_mixins.scss`, se define un mixin para facilitar el uso de media queries

## Estructura de SASS y organización de Archivos Parciales

El proyecto sigue el patrón 7-1, que divide los estilos en 7 carpetas principales y un archivo main.scss:

1. abstracts/
Contiene los abstractos como variables y mixins que se utilizan en todo el proyecto.
- _variables.scss: Define variables globales (colores, tipografías, espaciados).
- _mixins.scss: Contiene mixins reutilizables, como el de media queries.

2. base/
Incluye los estilos base y las reglas de reset.
- _reset.scss: Restablece los estilos predeterminados del navegador.
- _typography.scss: Define las reglas tipográficas generales.
- _base.scss: Contiene estilos generales para elementos HTML básicos.

3. components/
Contiene los estilos de componentes reutilizables.
- _button.scss: Estilos para botones.
- _card.scss: Estilos para tarjetas utilizadas en servicios, testimonios y equipo médico.
- _form.scss: Estilos para formularios.

4. layout/
Incluye estilos que estructuran el diseño general del sitio.
- _header.scss: Estilos para el encabezado.
- _footer.scss: Estilos para el pie de página.

5. pages/
Estilos específicos para páginas particulares.
- _home.scss: Estilos exclusivos de la página de inicio.
- _team.scss: Estilos para la página del equipo médico.
- _contact.scss: Estilos para la página de contacto.

6. themes/
Para estilos temáticos o de personalización.
- _dark.scss: Estilo para tema oscuro (por realizar)
- _light.scss: Estilo para tema claro (por realizar)

7. vendors/
Incluye archivos de terceros o librerías externas.
- _normalize.scss: Restablece los estilos de los navegadores de forma más completa que un simple reset. Libreria en https://github.com/kristerkari/normalize.scss/tree/master 

