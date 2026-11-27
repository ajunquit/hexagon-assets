# Identidad de Hexagon

Colores y uso de la marca en las interfaces de la suite. La implementación vive en
`hexagon-template-ng` ([ADR 0072](https://github.com/ajunquit/hexagon-template-ng/blob/main/docs/adr/0072-un-acento-tres-niveles-de-boton-y-modo-oscuro-elevado.md)).

## Isotipo

Un anillo hexagonal de cuatro facetas, cada una con su degradado
([hexagon-isotipo.png](hexagon-isotipo.png)):

| Faceta              | Desde     | Hasta     |
| ------------------- | --------- | --------- |
| Superior derecha    | `#7EEAE7` | `#3FC6CD` |
| Inferior derecha    | `#0AA2B3` | `#00596B` |
| Inferior izquierda  | `#2B95E9` | `#1E55C2` |
| Superior izquierda  | `#2ACAF6` | `#3290EA` |

Los turquesas y los azules son la **firma de la marca**: el isotipo, su animación de espera y los
fondos de acceso. No se usan para pintar controles.

## Un solo acento

La interfaz usa **un color de acento**, el primario: **`#2264cb`**, casi la faceta azul más
profunda del isotipo (`#1E55C2`). Marca solo lo que se puede pulsar o lo que está seleccionado.
Nombres, títulos y barras de desplazamiento van en colores neutros.

| Uso                                   | Claro                   | Oscuro                              |
| ------------------------------------- | ----------------------- | ----------------------------------- |
| Relleno de acción (texto blanco)      | `#2264cb` (5,6:1)       | `#2264cb` (5,6:1)                   |
| Texto o ícono en el acento            | `#2264cb`               | `#90b2e5` (primario + 50 % blanco)  |
| Tono suave (fondo secundario)         | primario al 15 %        | primario al 15 %                    |

Un producto de la suite puede tener su propio primario; los tonos se derivan de él con las
mismas reglas.

## Neutros

| Superficie                    | Claro     | Oscuro    |
| ----------------------------- | --------- | --------- |
| Página                        | `#f0f5f9` | `#0f1d2e` |
| Tarjetas, cabecera y menú     | `#ffffff` | `#15263a` |
| Texto                         | `#111c2d` | blanco al 90 % |

En oscuro, las superficies elevadas son **más claras** que la página, como en Apple.

## Colores de estado

| Estado      | Color     |
| ----------- | --------- |
| Éxito       | `#137333` |
| Advertencia | `#a34e08` |
| Error       | `#b91c1c` |
| Información | `#0369a1` |
| Neutro      | `#475569` |

Todos cumplen AA (4,5:1) con texto blanco y como texto sobre su tono suave. El neutro (gris
pizarra) es para estados, nunca para rellenar una acción.

## Botones: tres niveles

| Nivel          | Aspecto                                       | Uso                                           |
| -------------- | --------------------------------------------- | --------------------------------------------- |
| **Principal**  | Relleno del primario, texto blanco            | La acción que la persona vino a hacer. Una por grupo |
| **Secundario** | Tono suave del primario, texto del primario   | La alternativa: cancelar, volver, restablecer |
| **Terciario**  | Sin fondo, solo texto o ícono                 | Más acciones (⋮), limpiar (×), enlaces        |

Una acción destructiva puede ir rellena en rojo; entonces es la principal de su grupo. No se usan
botones con borde ni elevados.

## Tipografía

**Plus Jakarta Sans** (400, 500, 600, 700), con la fuente del sistema como respaldo.
