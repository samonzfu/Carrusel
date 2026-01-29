## Uso básico

### 1. Estructura HTML

Crea un contenedor con la clase **jocarsacarrusel** y coloca dentro las imágenes:

```html
<div class="jocarsacarrusel">
  <img src="imagen1.jpg" alt="Imagen 1">
  <img src="imagen2.jpg" alt="Imagen 2">
  <img src="imagen3.jpg" alt="Imagen 3">
</div>
```

No es necesario añadir botones ni secciones manualmente.
El script se encarga de todo.

### 2. Resultado

* Las imágenes se agrupan en un carrusel horizontal
* Se crean automáticamente dos botones:

  * ◀ Anterior
  * ▶ Siguiente
* El desplazamiento se realiza con animación

## Requisitos

* Todas las imágenes deben tener el mismo tamaño
* Tamaño por defecto del carrusel:

  * Anchura: **1280px**
  * Altura: **720px**

Si usas imágenes de otro tamaño, debes modificar el CSS y la variable `anchura` en el JS.

## Personalización

### Cambiar tamaño del carrusel

En el archivo CSS:

```css
.jocarsacarrusel {
  width: 1280px;
  height: 820px;
}
.jocarsacarrusel section img {
  width: 1280px;
  height: 720px;
}
```

En el archivo JS:

```js
var anchura = 1280;
```

Los tres valores deben coincidir.

## Cómo funciona internamente

* El script:

  * Detecta las imágenes del contenedor
  * Las mueve a una `<section>` interna
  * Crea los botones de navegación
  * Desplaza la sección usando `left` y `transition`

No necesitas llamar a ninguna función manualmente.

## Compatibilidad

* Funciona en navegadores modernos
* No compatible con Internet Explorer antiguo

## Licencia

Uso libre para proyectos personales o educativos.

```
::contentReference[oaicite:0]{index=0}
```

