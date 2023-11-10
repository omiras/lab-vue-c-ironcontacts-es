![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Vue.js IronContacts (Composition API)

## Introducción

Después de Ironhack, has decidido trabajar en la industria cinematográfica, y has encontrado un trabajo en el que necesitas gestionar los contactos de un famoso productor.

Tu tarea es crear una aplicación de gestión de contactos para el productor utilizando Vue.js.

## Instrucciones

### Iteración 1 | Mostrar todos los contactos

Hemos inicializado una variable global con todos los contactos. Es un array de objetos. Puedes ver el aspecto de esta variable en el fichero `contacts.json`

<details>
  <summary> Ver imagen dentro - Iteración 1</summary>

![Screenshot - Iteration 1](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-1.png)

</details>

Utiliza v-for para crear tantas filas en la tabla como contactos hay en _allContacts_ , mostrando en cada celda la información que se muestra en la captura de pantalla anterior

### Iteración 2 | Mostrar Condicionalmente la Información de Premios

El productor desea ver la información sobre los _premios_ que el contacto ha ganado.

Actualice la lista y agregue dos columnas más "Ganó un Oscar" ("Won an Oscar") y "Ganó un Emmy" ("Won an Emmy"), al final de la tabla. Luego, dependiendo del valor `wonOscar` y `wonEmmy` de cada contacto, renderice condicionalmente un ícono de trofeo :trophy: o ningún contenido.

Una vez hecho esto, su aplicación debería verse así:

<details>

<summary> Ver imagen dentro - Iteración 2</summary>

![Screenshot - Iteration 2](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-2.png)

</details>

### Iteración 3 | Filtrar

Crea controles de formulario para filtrar por los siguientes criterios:

1. Poder filtrar por nombre y apellidos
2. Poder filtrar por un mínimo de popularidad
3. Poder filtrar por aquellos famosos que han ganado un Emmy y/o un Óscar

Tienes que pensar que tipo de control de formulario vamos a usar para cada campo. ¿Un select? ¿Un input? ¿checkboxes?

Necesitas crear un _computed property_ e iterar sobre ella con el v-for, en vez de la variable original allContacts. Es más fácil este apartado si se aplican los filtros inmediatamente al cambiar el valor en los diferentes selectores.

### Iteración 4 | Eliminar contactos

El productor también desea eliminar algunos de sus contactos. Implemente un botón _Eliminar_ (_Delete_) en cada fila de su `<table>` que permita al usuario eliminar el contacto que haya hecho clic.

Cuando hagan clic, debe obtener el `id` de ese actor y utilizarlo para eliminar el contacto del array. ¡Recuerde actualizar la variable de referencia que contiene los contactos después de eliminar el contacto!

Cuando termine, su aplicación debería verse así (después de jugar un poco con el botón _Eliminar_ (_Delete_)):

<details>
  <summary> Ver imagen dentro - Iteración 5 </summary>

![Screenshot - Iteration 5](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-5.png)

</details>

### Iteración 5 | Ordenar Contactos por Nombre y Popularidad

El productor te pidió que agregues dos nuevos botones para ayudarles a ordenar sus contactos. Cuando hagas clic en uno de los botones, debería **ordenar la tabla por nombre (`name`)** (alfabéticamente), y cuando hagas clic en el otro, debería **ordenar por popularidad (`popularity`)** (el más alto primero).

Una vez que hayas ordenado el array, recuerda actualizar la variable ref que contiene los contactos.

Esto es lo que deberías tener al final de esta iteración:

<details>
  <summary> Ver imagen dentro - Iteración 4 </summary>

![Screenshot - Iteration 6](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-4.png)

</details>
