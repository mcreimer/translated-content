---
title: WindowBase64.atob()
slug: Web/API/atob
translation_of: Web/API/WindowOrWorkerGlobalScope/atob
original_slug: Web/API/WindowOrWorkerGlobalScope/atob
---
{{APIRef}}

La función **WindowBase64.atob()** descodifica una cadena de datos que ha sido codificada utilizando la codificación en base-64. Puedes utilizar el método {{domxref("window.btoa()")}} para codificar y transmitir datos que, de otro modo podrían generar problemas de comunicación. Luego de ser transmitidos se puede usar el método window\.atob() para decodificar los datos de nuevo. Por ejemplo, puedes codificar, transmitir y decodificar los caracteres de control como valores ASCII 0 a 31.

For use with Unicode or UTF-8 strings, see [this note at Base64 encoding and decoding](/es/docs/Web/JavaScript/Base64_encoding_and_decoding#The_.22Unicode_Problem.22) and [this note at `window.btoa()`](/es/docs/Web/API/window.btoa#Unicode_Strings).

## Syntax

```
var decodedData = window.atob(encodedData);
```

## Example

```js
var encodedData = window.btoa("Hello, world"); // encode a string
var decodedData = window.atob(encodedData); // decode the string
```

## Specifications

| Specification                                                                                        | Status                           | Comment                                                                                                                  |
| ---------------------------------------------------------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| {{SpecName('HTML WHATWG', '#dom-windowbase64-atob', 'WindowBase64.atob()')}} | {{Spec2('HTML WHATWG')}} | No change since the latest snapshot, {{SpecName("HTML5.1")}}.                                                   |
| {{SpecName('HTML5.1', '#dom-windowbase64-atob', 'WindowBase64.atob()')}}     | {{Spec2('HTML5.1')}}     | Snapshot of {{SpecName("HTML WHATWG")}}. No change.                                                             |
| {{SpecName("HTML5 W3C", "#dom-windowbase64-atob", "WindowBase64.atob()")}} | {{Spec2('HTML5 W3C')}}     | Snapshot of {{SpecName("HTML WHATWG")}}. Creation of `WindowBase64` (properties where on the target before it). |

## Browser compatibility

{{Compat("api.atob")}}

## See also

- [Base64 encoding and decoding](/Web/API/WindowBase64/Base64_encoding_and_decoding)
- [`data` URIs](/es/docs/data_URIs)
- {{domxref("window.btoa()")}}
- [Components.utils.importGlobalProperties](/es/docs/Components.utils.importGlobalProperties)
