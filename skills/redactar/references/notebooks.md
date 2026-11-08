# Notebooks Jupyter de trabajos prácticos

El notebook es la entrega y lo primero que lee el profesor. El markdown explica la teoría y narra el trabajo; el código está al servicio de esa narrativa. Al profesor le importa la explicación; el código le importa al autor.

## Narrativa

- La narración pedagógica es breve pero clara: pocas oraciones antes del código (qué se calcula y para qué) y la interpretación en la celda de observaciones, sin repetir en una lo que dice la otra. Una sección simple se explica en uno o dos párrafos cortos.
- Seguir la estructura y el estilo que el notebook ya tiene (niveles de título, celdas de "**Observaciones**:" después de los gráficos, notación de las ecuaciones).
- Las explicaciones siguen el encuadre que se dio en clase y en el paper del TP, con su misma notación y numeración de ecuaciones.
- Responder a la consigna con sus mismos términos.
- Declarar las hipótesis simplificadoras ("se asume transmisor y receptor sincronizados") y respetarlas. Distinguir conceptos que se confunden (detección y sincronización, por ejemplo).
- Cuando se agrega una herramienta de análisis (espectrograma, curva ROC), explicar qué es y qué muestra.
- Cada gráfico lleva su interpretación. Si dos métodos difieren, explicar por qué. Si el resultado contradice la intuición, decirlo y explicarlo.
- Los números que se citan en el texto salen de lo que ya está graficado o impreso. No volver a simular solo para leerlos.
- Al extender un notebook, escribir primero la explicación en markdown y después el código. Rellenar la estructura de celdas existente y no tocar las celdas que ya están, salvo que se pida.

## Figuras

- Solo figuras que aportan. Un 3D que no se aprecia "es al pedo"; si una dimensión extra aporta, conviene un gráfico interactivo.
- Graficar la magnitud de la fórmula y la salida real del algoritmo, no cantidades derivadas con aritmética extra.
- Ejes en magnitudes físicas con unidades (frecuencia en kHz, no el índice `q`).
- Escala logarítmica cuando los valores son casi cero (tasas de error).
- Elegir el valor del parámetro fijo para que la variación se vea.
- Si hay demasiados elementos, simplificar. Usar paneles y rótulos para que se distingan las partes.
- Cada entrada de la leyenda corresponde a una línea visible. Si dos curvas se superponen, distinguirlas por estilo u orden de dibujo.
- Comparaciones antes y después de cada paso (calibración, filtrado). Una prueba de sanidad simple y visual antes del experimento complejo.
- Mostrar la señal completa cuando importa el contexto (la trama entera con su preámbulo, no solo el payload).

## Código

- Menos código es más didáctico. Funciones con nombres claros que formen un pipeline legible.
- Implementar explícitamente lo que el TP pide implementar (las ecuaciones del paper) y usar bibliotecas para lo estándar (FFT).
- numpy idiomático y conciso está bien. No reemplazarlo por bucles muestra a muestra "para que sea didáctico" sin consultar.
- Nada que no funcione o no se use: se arregla o se saca.
- El notebook tiene que correr siempre, también sin el hardware o los datos del laboratorio.
- Si el usuario pregunta "¿por qué X?", explicar X. Una pregunta no es un pedido de borrarlo.
- No ejecutar el notebook ni celdas sin que lo pida, y avisar si algo va a tardar mucho.
