# Typst

## Referencias y bibliografía

- Referencias internas con `@etiqueta` (`@sec-modelo`, `@tab-resultados`). Antes de inventar una etiqueta, buscar las que ya existen en el proyecto (`grep -rn "<sec-" secciones/`) y seguir su convención.
- Citas bibliográficas con `@clave` al final de la oración que respaldan. Para una página, `@clave[p.~121]`.
- Las fuentes nuevas se agregan como entradas en el `.bib` del proyecto, siguiendo el formato de las existentes.

## Promesas y TODOs

Cuando el texto promete desarrollar algo en otra sección, dejar en la sección de destino un comentario con el formato que ya use el grupo. El usado hasta ahora es:

```typst
// TODO(prometido en Marco teórico, @sec-modelo) Analizar el compromiso que se mencionó al presentar el modelo.
```

Los TODOs nunca apuntan a archivos de trabajo que no se versionan (notas `.md` locales).

## Figuras

- Las figuras se hacen en Typst, para que el grupo pueda editarlas. No generar SVG o PNG con scripts externos.
- Para diagramas, usar paquetes de Typst Universe antes de escribir funciones propias (por ejemplo `chronos` para diagramas de secuencia, `cetz` para dibujos, `fletcher` para diagramas de nodos).
- Toda figura o tabla lleva `caption` y etiqueta, y el texto la referencia.

## Imports

Los `#import` van al principio del archivo, nunca junto a la figura en medio del texto. Si el proyecto incluye las secciones con `#include`, el import del archivo principal no llega a ellas, así que va al principio del archivo de la sección.

## Compilación

Compilar con el `typst` local (ver el comando en el README o en el comentario del archivo principal). No usar servicios en la nube ni instalar otra versión. Si no se puede compilar, pedirle al usuario que lo haga.

## Comentarios y esqueletos

Los archivos de sección suelen tener comentarios con notas, el pedido del profesor y TODOs. Al reemplazar un esqueleto con texto, esos comentarios se conservan.
