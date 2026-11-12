# Laboratorio de la Unidad de Control · Arquitectura de Computadores 03306 (UNED)

Recursos interactivos para estudiar cómo una CPU busca, decodifica y ejecuta instrucciones. Funcionan en cualquier navegador moderno (Chrome, Edge, Firefox), sin instalar nada.

**Creado por Ing. Heiner Guido Cambronero, Lic.**

**Abrir en línea:** https://heinergc.github.io/arquitectura-computadores-03306/

## Recursos

| Figura | Recurso | Qué es |
|---|---|---|
| R.1 | [CPU Quest: Misión Unidad de Control](recursos/cpu-quest.html) | Videojuego de seis misiones: componentes, señales de control, ciclo FETCH, ejecución de un programa, depuración y saltos condicionales. Guarda el progreso en el navegador. |
| R.2 | [Von Neumann en movimiento](recursos/von-neumann.html) | Animación ciclo a ciclo de un programa que suma 5 + 3, comparando el bus único de Von Neumann con los dos buses de Harvard. |
| R.3 | [Glosario bilingüe](recursos/glosario.html) | 60 términos en inglés y español en 5 categorías, con diagramas, el ejemplo `LOAD R1, [500]` y una simulación del ciclo de instrucción. |

La página de inicio ([index.html](index.html)) presenta los tres recursos, una ruta de estudio sugerida y una tabla con los conceptos del curso que trabaja cada uno.

## Uso local

Descarga o clona el repositorio y abre `index.html` en el navegador. No necesita servidor ni conexión, salvo la animación de Von Neumann, que carga su tipografía desde Google Fonts (sin conexión usa una tipografía del sistema).

## Estructura

```
index.html            portal (página de inicio)
recursos/             los tres recursos, cada uno en un solo archivo HTML
assets/fonts/         tipografías Source Serif 4 y Source Sans 3 (SIL Open Font License)
PRODUCT.md, DESIGN.md decisiones de producto y de diseño del portal
```

Material didáctico complementario basado en los conceptos de Unidad de Control y ciclo de instrucción (Stallings, capítulo 19). No es un documento institucional oficial de la UNED.
