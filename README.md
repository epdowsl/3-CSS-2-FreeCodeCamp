<h1>#3 CSS-2</h1>


<h2>Proyecto de FreeCodeCamp con HTML y Git</h2>
En este curso voy a aprender HTML por parte de FreeCodeCamp. Y agradezco mucho por la información de calidad y más interesante que es muy práctico.

<h2>CSS</h2>
Este es un proyecto de práctica de colores en CSS.

Aqui se prácticara la combinación de colores, valores de rgb y uso de valores hexadecimables en CSS.

<h2>Valores del rgb</h2>
<h4>Valores primarios</h4>
  <p>rgb(255, 0, 0) = red<p>
  <p>rgb(0, 255, 0) = green<p>
  <p>rgb(0, 0, 255) = blue<p>

<h4>Valores segundarios</h4>
  <p>rgb(255, 255, 0) = yellow<p>
  <p>rgb(0, 255, 255) = lightblue<p>
  <p>rgb(255, 0, 255) = pink<p>

<h4>Valores terciarios</h4>
  <p>rgb(255, 127, 0) = orange<p>
  <p>rgb(0, 255, 127) = lightgreen<p>
  <p>rgb(127, 0, 255) = purple<p>
<h5>Otros valores terciarios</h5>
  <p>rgb(127, 255, 0) = chartreuse green<p>
  <p>rgb(0, 127, 255) = azure<p>
  <p>rgb(255, 0, 127) = rose<p>

<h4>Valores hexadecimales</h4>
<p>Los valores hexadecimales empiezan con el carácter #, siguiendo seis caracteres entre 0-9 y A-F. El primer par de caracteres representa el rojo, el segundo el verde y el tercero el azul.</p> 

Por parte de FreeCodeCamp sugiere que los valores hexadecimales se representan de la siguiente manera:

0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

Para los colores en hexadecimal, 00 es 0% de ese color, y FF es 100%. De tal manera que #00FF00 se traduce en 0% rojo, 100% verde y 0% azul, siendo equivalente a rgb(0, 255, 0).

<h4>Valores HSL</h4>
Este es otro formato para representa colores en CSS y su forma de presentarse los colores son de 3 valores, primero el matiz que va de 0 a 360 de matiz, el segundo es de porcentaje en saturación que va de 0 a 100% y el tercero es de porcentaje en ilumnación que va de 0 a 100%.

FreeCodeCamp comenta: 

El matiz (hue/h) rojo está en 0 grados, el verde en 120 y el azul en 240.
La saturación (saturation/s) es la intensidad de un color desde 0%, o gris, hasta 100% para color puro. Debes agregar el signo de porcentaje % a los valores de saturación y luminosidad.
La luminosidad (lightness/l) es lo brillante que parece un color, desde 0% o completamente negro, hasta 100%, completamente blanco, siendo neutro el 50%.

<h6>Ejemplo de valores y en código</h6>

hsl (h, s, l)

```
elemento {
background-color: hsl(240, 100%, 50%) /* Color azul */
}
```

<h4>Otras formas de combinar colores</h4>

Como hemos visto ha diferentes formas de cambiar colores en su forma plana, pero hay otras formas para cambiar de color de manera transitoria como los gradientes, o degradado, a la transición progresiva de un color a otro. ESta forma usa la función linear-gradient permite controlar la dirección de la transición a lo largo de una línea, y qué colores participan en el degradado.
Esta función lo que en realidad crea es un elemento image y se asocia normalmente con la propiedad background, la cual puede aceptar una imagen como valor.

Se representa de la siguiente manera:

```
elemento {
background: linear-gradient(gradientDirection, color1, color2, ...);
}
```

La función linear-gradient tiene en su valores los siguientes: gradientDirection es la dirección de la línea a lo largo de la cual tendrá lugar la transición, es decir, los grados 0 a 360deg, los demás son los argumentos de color, representando los colores usados en la transición. A continuación un ejemplo:

```
elemento {
  .red {
  background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0), rgb(0, 0, 255)); /* Los colores en dirección vertical, colores rojo y azul en sus extremos, el verde en medio y una pequeña combinación de los colores anteriores en los extremos del color verde.
}
```

<h4>Propiedades nuevas en este curso</h4>
<ul>
  <li>opacity: Puede controlar cuán opaco o transparente es un elemento. valores que se ponen en esta propiedad son 0-1.0 o también 0%-100%</li>
  <li>box-shadow: Permite aplicar una o más sombras alrededor de un elemento. Esta sería la sintaxis básica:</li>
    <p>Su sintesis es el siguiente:</p>
  
```
box-shadow: offsetX offsetY blurRadius spreadRadius color;
```

  
</ul>

<h4>Canal Alfa</h4>
El canal alfa es usado en entornos de colores en CSS y va a acompañado dentro de los valores como rgb o hsl, pero estos para que tengan el canal alfa tendran que tener "a" al final de ellos, por ejemplo, rgba o hsla. Es como la propiedad de opacity pero sin colocarle como propiedad y va en las funciones del rga o hsl, también funciona con 0-1.0 o 0%-100%.
