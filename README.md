# EPED-TRAQ-AR

Mapa de la República Argentina dividido por provincias y agrupado en **5 áreas operativas**
con carga equilibrada de hospitales públicos pediátricos / referentes pediátricos
(36 centros en total, 6–8 por área).

## Contenido

| Archivo | Descripción |
|---|---|
| `index.html` | Mapa interactivo autocontenido (SVG inline, tooltips por provincia, listado por área) más un segundo mapa **estático de cobertura** que colorea cada provincia según si sus hospitales del estudio tienen usuarios registrados (completa / parcial / solo otras instituciones / sin registros). Funciona abriéndolo directo en el navegador o vía GitHub Pages. |
| `data/hospitales.json` | Listado estructurado de los 36 hospitales con provincia, localidad, perfil y área asignada. |

## Las 5 áreas

| Área | Región | Provincias | Hospitales |
|---|---|---|---|
| 1 | Metropolitana | CABA, Buenos Aires | 8 |
| 2 | NEA · Litoral | Santa Fe, Entre Ríos, Corrientes, Misiones, Chaco, Formosa | 7 |
| 3 | NOA | Jujuy, Salta, Tucumán, Catamarca, Santiago del Estero, La Rioja | 6 |
| 4 | Centro · Cuyo | Córdoba, San Juan, Mendoza, San Luis, La Pampa | 7 |
| 5 | Patagonia | Neuquén, Río Negro, Chubut, Santa Cruz, Tierra del Fuego | 8 |

36 hospitales no se reparten exactos entre 5 áreas: el rango 6–8 (promedio 7,2) es la
partición más pareja posible manteniendo áreas geográficamente contiguas.

## Fuentes

- Listado de hospitales: provisto por el equipo del estudio (septiembre 2026).
- Geometrías provinciales: [Natural Earth](https://www.naturalearthdata.com/) 1:10m
  (dominio público), simplificadas. Las Islas Malvinas se representan como parte de la
  provincia de Tierra del Fuego, Antártida e Islas del Atlántico Sur.
