---
title: <marquee>
slug: Web/HTML/Element/marquee
tags:
  - Elemento
  - HTML
  - Referencia
  - Web
  - etiqueta
  - marquee
  - marquesina
  - obsoleta
translation_of: Web/HTML/Element/marquee
original_slug: Web/HTML/Elemento/marquee
---
{{HTMLRef}}{{obsolete_header}}

## Resumen

La etiqueta html `<marquee>` se utiliza para insertar un area de texto en movimiento. También se la conoce como marquesina.

## Atributos

- {{htmlattrdef("behavior")}}
  - : Establece cómo se desplazará el texto en la etiqueta marquee. Los valores posibles son scroll, slide, y alternate. Si no hay un valor especificado, el valor por defecto establecido es scroll.
    Scroll: Hara que lo que este en la marquesina se mueva de derecha a izquierda, de manera ininterrumpida.
    Slide: Una vez que completa el recorrido de derecha a izquierda(por defecto) se detiene.
    Alternate: Se movera de una esquina a la otra, dando el efecto de rebote.
- {{htmlattrdef("bgcolor")}}
  - : Establece el color de fondo, puede utilizarse el nombre, o su valor hexadecimal.
- {{htmlattrdef("direction")}}
  - : Establece la dirección en la que el texto contenido se desplazará. Los valores posibles son left (para moverse hacia la izquierda), right (para moverse a la derecha), up (hacia arriba) y down (hacia abajo). Si no se especifica un valor, por defecto será left.
- {{htmlattrdef("height")}}
  - : Establece la altura de la etiqueta en pixeles, o en un valor porcentual.
- {{htmlattrdef("hspace")}}
  - : Establece el margen horizontal.
- {{htmlattrdef("loop")}}
  - : Establece el número de veces que la marquesina realizará el desplazamiento. Sino se especifica esta propiedad, por defecto es -1, lo que quiere decir que la marquesina se desplazará continuamente.
- {{htmlattrdef("scrollamount")}}
  - : Establece el valor de movimiento para cada intervalo en pixeles. Por defecto su valor es 6.
- {{htmlattrdef("scrolldelay")}}
  - : Establece el intervalo entre cada desplazamiento, en milisegundos. El valor por defecto es 85. Nota: Cualquier valor inferior a 60 será ignorado, (puesto que el valor minimo es 60) y se establecerá 60 en su lugar. Salvo que se especifique`truespeed.`
- {{htmlattrdef("truespeed")}}
  - : Por defecto, si los valores de `scrolldelay son inferiores a 60 serán ignorados. Pero si truespeed está presente, esos valores inferiores a 60 serán aceptados.`
- {{htmlattrdef("vspace")}}
  - : Establece el margen vertical en pixeles o en un valor porcentual.
- {{htmlattrdef("width")}}
  - : Establece el ancho de la etiqueta en pixeles o un valor porcentual.

## Controladores de eventos

- {{htmlattrdef("onbounce")}}
  - : Este evento se lanza cuando la marquesina llegó al final del desplazamiento. Ésto solo se activa cuando el atributo `behavior`está establecido en `alternate`.
- {{htmlattrdef("onfinish")}}
  - : Este evento se lanza cuando la marquesina repitió el desplazamiento la cantidad de veces establecidas en el atributo `loop`. El evento se lanza solo si el atributo `loop` tiene un valor mayor a 0.
- {{htmlattrdef("onstart")}}
  - : Este evento se lanza cuando la marquesina comienza su desplazamiento.

## Métodos

- start
  - : Comienza el desplazamiento de la marquesina.
- stop
  - : Para el desplazamiento de la marquesina

## Ejemplos

```html
<marquee>Este texto se mueve de derecha a izquierda</marquee>

<marquee direction="up">Este texto se mueve de abajo hacia arriba</marquee>

<marquee direction="down" width="250" height="200" behavior="alternate" style="border:solid">
  <marquee behavior="alternate">
    Este texto rebotará dentro de la marquesina.
  </marquee>
</marquee>
```

{{EmbedLiveSample("Examples", 600, 450)}}

## Especificaciones

| Specification                                                                                                    | Status                           | Comment                                                                                                     |
| ---------------------------------------------------------------------------------------------------------------- | -------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| {{SpecName('HTML WHATWG', 'obsolete.html#the-marquee-element-2', '&lt;marquee&gt;')}} | {{Spec2('HTML WHATWG')}} | Marcada como obsoleta en favor de CSS. Comportamiento esperado definido por razones de retrocompatibilidad. |
| {{SpecName('HTML5 W3C', 'obsolete.html#the-marquee-element-0', '&lt;marquee&gt;')}} | {{Spec2('HTML5 W3C')}}     | Marcada como obsoleta en favor de CSS. Comportamiento esperado definido por razones de retrocompatibilidad. |

## Navegadores compatibles

{{Compat("html.elements.marquee")}}
