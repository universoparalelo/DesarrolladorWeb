# SOBRE CSS

## HERENCIA

- Hay estilos que se aplican a los hijos de una etiqueta
- Hay estilos que no respetan esa cadencia
- Podemos elegir entre el primer hijo :firstchild o el ultimo :lastchild para dar estilos a una etiqueta hija en forma de pseudo-clase
- Podemos elegir que todos los hijos <span> tengan cierto estilo pero no sus nietos o bisnietos
- Podemos dar estilos a etiquetas hermanas
- Ejemplos
- li:firts-child
- li:last-child
- li:second-child
- article ul
- article > ul
- article ~ ul
- article + ul

## CASCADA

- El estilo que se queda para cierta etiqueta es la ultima que se escribió
- El nivel de especificidad importará muchisimo para este punto

## ESPECIFICIDAD

- Según la forma en que se seleccionan las etiquetas serán mas importantes unas que otras (de mas importantes a menos):
- Nivel 1: !important
- Nivel 2: estilos en linea en HTML
- Nivel 3: ID
- Nivel 4: class
- Nivel 5: selector de etiqueta

## UNIDAD DE MEDIDA

- Pixel: no es absoluto, depende de la resolucion de cada pantalla
- Porcentaje: es relativo al tamaño de tu computadora
- Viewport: toma la altura de la ventana, puede llegar a sobrar si colocamos margenes en el body


## MODELO DE LA CAJA

- Inline: elementos que se acomodan uno al lado del otro, estilos como width y height no les afectan
- Block: elementos que se acomodan con un salto de linea, o uno debajo del otro, estos si se ven afectados por estilos tales como width y height
- Padding: aplicado a una etiqueta contenedora es el espacio que hay entre la etiqueta contenedora y sus hijos
- Margin: aplicado a un contenedor es el espacio que entre hay entre el contenedor y su super contenedor 
- Box-sizing: border-box; 

## DESBORDAMIENTO

- overflow: visible | hidden | scroll | auto;
- text-overfow: clip | ellipsis;

## POSICIONAMIENTO

- position: static | absolute (top & left & right & bottom) | relative (aplicado al contenedor) | fixed (en la pantalla) | sticky (en el contenedor);

## Z-INDEX

- z-index: numero;
- Debe tener un posicionamiento relativo o fixed

## FLEX

- Unidireccional

### CONTENEDOR

- display: flex;
- flex-direction: row | column | row-reverse | column-reverse | flex;
- flex-wrap: nowrap | wrap; 
- flex-flow: row nowrap; (version abreviada de flex-direction y flex-wrap)

- justify-content: center | space-around | space-between | space-evenly | flex-end | flex-start;
- gap: 16px (ejemplo);
- align-items: center | space-around | space-between | space-evenly | flex-end | flex-start; 
- align-content: center | space-around | space-between | space-evenly | flex-end | flex-start;

### HIJO/S

- Valores por defecto
- flex-grow: 0; (los elementos no crecen)
- flex-shrink: 1; (los elementos pueden reducir su tamaño a un tamaño mas pequeño que su flex-basis)
- flex-basis: auto; (los elementos tienen un tamaño base en auto)

- Valor que engloba estos tres anteriores
- flex: auto;

- Valores independientes
- flex: numero;
- order: numero;
- align-self: center | space-around | space-between | space-evenly | flex-end | flex-start;

## GRID

- Bidireccional

### CONTENEDOR

- display: block;
- grid-template-columns: 100px;
- grid-template-columns: 100px 100px;
- grid-template-columns: auto 100px;
- grid-template-columns: 50% 100px 10vw auto;
- grid-template-row: 100px 100px;
- grid-auto-rows: 100px;
- grid-template-columns: repeat(3,1fr);
- grid-template-rows: repeat(3,100px);
- grid-template-columns: minmax(100px, 1fr) 1fr 1fr;
- grid-column-gap: 10px;
- grid-row-gap: 10px;
- gap: columnas filas;
- grid-template-column: repeat(
    auto-fill, 
    minmax(200px, 1fr)
);
- grid-template-area: 
    "header header header" 
    "aside main main" 
    "footer footer footer";
- justify-item: stretch | normal | start | end;
- align-item: stretch | normal | start | end;

#### FRACCION

- 1fr == 100% 
- 1fr 1fr == 50% 50%
- 1fr 1fr 1 fr == 33% 33% 33%
- 1fr 2fr 1fr == 25% 50% 25% 

### HIJO/S 

- grid-column-start: 1;
- grid-column-end: 2;
- grid-row-start: 1;
- grid-row-end: 2;
- grid-column-start: span 2;
- grid-row-start: span 3;
- grid-column: 2 / 4;
- grid-row: 1 / 2;
- grid-are: < nombre para el area >
- justify-item: stretch | normal | start | end;
- align-item: stretch | normal | start | end;

## PAGINAS DE REFERENCIA

- [Curso CSS Manz](https://lenguajecss.com/css/#cheatsheets/)
- [Link para ir a la pagina de MDN](https://developer.mozilla.org/es/)
- [Flex froggy](https://flexboxfroggy.com/)
- [Retos de programacion](https://codember.dev/) 
- [Bento Grids](https://bentogrids.com/)
- [Grid garden](https://cssgridgarden.com/)