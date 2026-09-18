# EPED-TRAQ-AR

Mapa de la República Argentina dividido por provincias y agrupado en **5 áreas operativas**
con carga equilibrada de hospitales públicos pediátricos / referentes pediátricos
(36 centros en total, 6–8 por área).

## Contenido

| Archivo | Descripción |
|---|---|
| `index.html` | Mapa interactivo autocontenido (SVG inline, tooltips por provincia, listado por área) más un segundo mapa **estático de cobertura** que colorea cada provincia según si sus hospitales del estudio tienen usuarios registrados (completa / parcial / solo otras instituciones / sin registros). Funciona abriéndolo directo en el navegador o vía GitHub Pages. |
| `data/hospitales.json` | Listado estructurado de los 36 hospitales con provincia, localidad, perfil y área asignada. |
| `data/usuarios_fuera_universo.json` | Usuarios registrados cuya institución declarada no es ninguno de los 36 hospitales del universo. |
| `data/divisiones.json` | Las cuatro divisiones del mapa interactivo (zonas, provincias y conteo de hospitales). |

## Divisiones del mapa interactivo

El mapa interactivo tiene un dropdown para elegir cómo se divide el país. Solo se muestra una
división a la vez; al cambiarla se recolorean las provincias, las etiquetas del mapa, las tarjetas
laterales y los tooltips. La elección queda guardada en el navegador.

| División | Zonas | Hospitales por zona | Criterio |
|---|---|---|---|
| 5 áreas operativas (por defecto) | 5 | 6–8 | División de trabajo del estudio: contigüidad y carga pareja |
| 4 zonas | 4 | 8–10 | Norte (NOA+NEA) · Centro Este · Centro Oeste · Sur |
| 3 macrozonas | 3 | 12 c/u | Santa Fe va al Norte y Cuyo + La Pampa al Sur para equilibrar |
| 5 regiones INDEC | 5 | 3–15 | Regionalización geográfica tradicional, sin equilibrio de carga |

Las fichas de hospitales siguen siempre la división operativa.

## Las 5 áreas operativas

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
