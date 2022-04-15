Notas sobre la lectura "SVG, transiciones y animaciones" parte 2
================================================================

## 0. REFERENCIAS --*first things first*--:
* [Valore de `transition-timing-function` en W3Schools](https://www.w3schools.com/cssref/css3_pr_transition-timing-function.asp)
* [Visualizador de curvas de Bezier](https://cubic-bezier.com/#.17,.67,.83,.67)
* [Referencia en MDN sobre propiedades CSS animables](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)
* [Catálogo de curvas de Bezier para asignar a `transition-timing-funcion`](https://easings.net)
* []()

## 1. APUNTES

### 1.1 TRANSICIONES (p.1 - 17)

Las transiciones son propiedades CSS que nos permiten cambiar el valor de una propiedad desde un valor inicial a uno final durante un periodo de tiempo determinado. Esto permite realizar efectos como cambiar tamaños, desplazar elementos, modificar colores, todo con un control del periodo en que sucede. Ejemplo simple con un `<div></div>`: 

```css
  div {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s;
  }

  div:hover {
    width: 300px;
  }
```

El ejercicio en el archivo *pagina-3.html* de este repositorio tiene una muestra de una transición aplicada a un archivo svg. La versión live y el código se pueden observar [acá](https://codepen.io/carlospizarro/pen/eYyPbXb)

Hay un segundo ejemplo sin código en este repositorio que muestra el agregado de varios valores-coma-separados en la propiedad `transition`. Se puede ver el codepen [acá](https://codepen.io/carlospizarro/pen/QWaZYvZ). 

    Durante las páginas 7-12 no hace nada útil excepto presentar la propiedad `transition-timing-function`

- (p.15) Los valores en *keyword* que se pueden asignar a la propiedad `transition-timing-funtion` corresponden a formas de la curva de Bezier y son: `ease-in`, `ease-out`, `ease` y `linear`. 
- (p.17) En resumen la propiedad `transition` es un *shorthand* para 4 propiedades: 

```css
.element {
  transition-property: all;
  transition-duration: 1s;
  transition-timing-function: cubic-bezier(0, 0.5, 1, 1);
  transition-delay: 1s;
} 
es lo mismo que: 

.element {
  transition: all 1s cubic-bezier(0, 0.5, 1, 1) 1s;
}
```

## 2. NOTAS PERSONALES


## 3. APUNTES

