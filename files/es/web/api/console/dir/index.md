---
title: Console.dir()
slug: Web/API/Console/dir
translation_of: Web/API/Console/dir
---
{{APIRef("Console API")}}

El método **`dir()`** de {{domxref("Console")}} despliega una lista interactiva de las propiedades del objeto JavaScript especificado. El resultado es presentado como un listado jerárquico con triángulos de despliegue que te dejan ver los contenidos de los objetos hijos.

Dicho de otra manera, `console.dir()` es la manera de ver todas las propiedades de un objeto JavaScript específicado por consola, mediante la cual el desarrollador puede facilmente obtener las propiedades del objeto.

{{AvailableInWorkers}}

![console-dir.png](/@api/deki/files/6081/=console-dir.png)

## Sintaxis

```
console.dir(objeto);
```

## Parámetros

- `objeto`
  - : Un objeto JavaScript cuyas propiedades deben ser mostradas como resultado.

## Especificaciones

| Especificación                                                                           | Estatus                          | Comentario         |
| ---------------------------------------------------------------------------------------- | -------------------------------- | ------------------ |
| {{SpecName("Console API", "#consoledirobject", "console.dir()")}} | {{Spec2("Console API")}} | Definición inicial |

## Compatibilidad en navegadores

{{Compat("api.console.dir")}}

## Ver también

- [Opera Dragonfly documentation: Console](http://www.opera.com/dragonfly/documentation/console/)
- [MSDN: Using the F12 Tools Console to View Errors and Status](http://msdn.microsoft.com/library/gg589530)
- [Chrome Console API reference](https://developers.google.com/chrome-developer-tools/docs/console-api#consoledirobject)
