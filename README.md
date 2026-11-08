# skills-facultad

Skills de [Claude Code](https://claude.com/claude-code) para trabajos de la facultad.

## Skills

### `redactar`

Redacta, completa, reescribe o revisa material universitario en español: monografías, informes de trabajos prácticos, contenido en Typst o LaTeX y celdas markdown de notebooks Jupyter.

El objetivo es un texto que el docente pueda leer de corrido sin perderse:

- una idea por sección, sin relleno ni exceso de detalles.
- cada término definido en su primer uso, para un lector sin contexto.
- citas que respaldan ideas, no una por oración.
- registro formal, oraciones completas y encadenadas.
- rigor sin exhaustividad: nada falso ni sin fuente, pero tampoco cada matiz que se encontró al investigar.

También define cómo trabajar: leer el material de la cátedra y las secciones vecinas, acordar la idea principal y la estructura antes de redactar, respetar las notas y correcciones del usuario y mantener los mensajes del chat cortos.

Incluye guías específicas para Typst, notebooks Jupyter y trabajos grupales con repositorio, issues y PRs.

Ejemplos de pedidos:

- "Arranquemos con la subsección de keep-alive del desarrollo."
- "Un compañero escribió la sección del método de Welch y la redacción no es la mejor. Reescribila."
- "La sección de potencia del notebook no tiene explicación. Escribí el markdown que falta."

## Instalación

### Como plugin

```
/plugin marketplace add b-Tomas/skills-facultad
/plugin install facultad@facultad
```

La skill queda disponible como `/facultad:redactar`. Para traer los cambios nuevos del repositorio:

```
/plugin marketplace update facultad
```

### Copiando la carpeta

```sh
git clone https://github.com/b-Tomas/skills-facultad.git
cp -r skills-facultad/skills/redactar ~/.claude/skills/
```

La skill queda disponible como `/redactar`. Para usarla solo en un proyecto, copiar la carpeta a `.claude/skills/` dentro de ese proyecto. Para actualizarla, hacer `git pull` en el clon y volver a copiar la carpeta, o reemplazar la copia por un enlace simbólico al clon para que tome los cambios sola:

```sh
ln -s "$PWD/skills-facultad/skills/redactar" ~/.claude/skills/redactar
```

En ambos casos, Claude también la usa por su cuenta cuando se le pide escribir o corregir texto de un trabajo de la facultad.

## Licencia

MIT
