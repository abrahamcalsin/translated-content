---
title: String.prototype.small()
slug: Web/JavaScript/Reference/Global_Objects/String/small
tags:
  - Deprecated
  - HTML wrapper methods
  - JavaScript
  - Method
  - Prototype
  - String
translation_of: Web/JavaScript/Reference/Global_Objects/String/small
original_slug: Web/JavaScript/Referencia/Objetos_globales/String/small
---

{{JSRef("Objetos_globales", "String")}}

{{deprecated_header}}

## Resumen

Causa que una cadena se muestra con una fuente pequeña, como si estuviese dentro de una etiqueta {{HTMLElement("small")}}.

## Sintaxis

```
cadena.small()
```

## Descripción

Usa el método `small` para formatear y mostrar una cadena en un documento.

## Ejemplos

### Ejemplo: Usando métodos de `string` para cambiar el tamaño de una cadena

```js
var cadenaMundo="¡Hola mundo!"

console.log(cadenaMundo.small())
console.log(cadenaMundo.big())
console.log(cadenaMundo.fontsize(7))
```

Este ejemplo produce el mismo resultado que el siguiente código HTML:

```html
<small>¡Hola mundo!</small>
<big>¡Hola mundo!</big>
<fontsize=7>¡Hola mundo!</fontsize>
```

### Vea También

- {{jsxref("String.prototype.fontsize()")}}
- {{jsxref("String.prototype.big()")}}
