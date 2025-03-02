---
title: HTMLLIElement
slug: Web/API/HTMLLIElement
tags:
  - API
  - HTML DOM
translation_of: Web/API/HTMLLIElement
---

{{ APIRef("HTML DOM") }}

La interfaz **HTMLLIElement** expone las propiedades y los métodos específicos (más allá de los definidos por la interfaz regular {{domxref ("HTMLElement")}} que también tiene disponible por herencia) para manipular elementos de la lista.

## Propiedades

_Hereda las propiedades de su elemento primario, {{domxref ("HTMLElement")}}._

- {{domxref("HTMLLIElement.type")}} {{deprecated_inline}}
  - : Es un {{domxref ("DOMString")}} que representa el tipo de las viñetas, "disco", "cuadrado" o "círculo". Como la forma estándar de definir el tipo de lista es a través de la propiedad CSS {{cssxref ("list-style-type")}}, use los métodos CSSOM para establecerlo a través de un script.
- {{domxref("HTMLLIElement.value")}}
  - : Es un largo que indica la posición ordinal del elemento de lista dentro de un {{HTMLElement ("ol")}} dado. Refleja el atributo {{htmlattrxref ("valor", "li")}} del elemento HTML {{HTMLElement ("li")}} y puede ser menor que 0. Si el elemento {{HTMLElement ("li")}} Elemento no es hijo de un elemento {{HTMLElement ("ol")}}, la propiedad no tiene ningún significado.

## Metodos

_No specific method; inherits properties from its parent, {{domxref("HTMLElement")}}._

## Especificaciones

{{Specifications}}

## Compatibilidad con Navegadores

{{Compat("api.HTMLLIElement")}}

## Ver también

- El elemento HTML que implementa esta interfaz: {{HTMLElement("li")}}
