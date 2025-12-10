# ExamenPaginaWEB
## Ejercicio 1
### 1A. Pregunta ¿Por qué NO se centra el texto del h1 en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)
#### El titulo no queda centrado ya que flexbox reparte espacio entre bloques, no dentro del texto, y por tanto ese text align center solo centra el texto dentro de h1 no en cabecera.
### 1B. Ejercicio - Soluciona de dos formas diferentes
#### Con flex seria:

.site-header {
  display: flex;
  align-items: center;
}

.site-header h1 {
    flex:1; (Para que el h1 ocupe el espacio entero y por tanto este todo por igual y ya abajo lo centramos)
  text-align: center;
}
Y con grid:

.site-header {
  display: grid;
  grid-template-columns: auto auto auto; (Aqui creamos 3 columna ya que podemos observar que en la parte izquierda hay un menu desplegable y en la parte derecha el menu de navegacion, asi al hacer un grid column y el text align el texto quedara centrado)
  align-items: center;
}

.site-header h1 {
  grid-column: 2; (Aqui te coloca el titulo donde quieras ponerlo)
  text-align: center; (te alinea el texto)
}
### 1C. Ejercicio – Convertir la cabecera en dos filas
#### .site-header {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-template-rows: auto auto auto;
  align-items: center;
  
}
h1 + nav {
    margin-top: 30px;
}
.site-header h1 {
  grid-column: 2;
  grid-row: 1;
  text-align: center;
  
}
h1 > nav {
    margin-top: 30px;
}
.main-nav {
    
  grid-row: 2;
  grid-column:2;
  text-align: center;
  list-style: none;
}
.main-nav ul {
  list-style: none;
}
### 1D. Ejercicio - Dar relieve y separacioón visual al header
#### .site-header {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-template-rows: auto auto auto;
  align-items: center;
  background-color: gray;
  border-bottom: solid black;
}
## Ejercicio 2 — Reorganización del header con tres elementos

## Ejercicio 3 — Miniaturas, zoom y enlace a la imagen original
### 3A. Crear miniaturas
#### Yo ya lo hice con un generador para que todas esten echas de igual tamaño e igual anchura, se tendria que hacer lo mismo pero con un ancho de 200 px por ejemplo.
### 3B. Efecto hover
#### Con el box shadow con un generador de sombras se pone la sombra por detras, luego con un border solid black le pongo bordes y con transform scale (1.03) le pongo un mini ZOOM
## Ejercicio 4 - Informe de evidencias del proyecto (defensa técnica simple)
### 4.1. Introduccion
- El tema de mi WEB es acerca de motos.
- He incluido la Historia general del motociclismo, seguido de unas miniaturas de motos de diferentes tipos con su respectiva tabla de cada modelo con sus especificaciones y caracteristicas y terminando con un formulario para mas informacion y informacion para ponerse a contacto conmigo.
- Mi idea de diseño era que transmita ganas de leerlo una vez visualizandolo, con colores no muy llamativos pero sin quitarle esencia.
### 4.2. Evidencias de HTML5

