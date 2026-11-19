# Modelos 3D SLEEP'N

Visores 3D interactivos de edificios y hoteles, levantados planta a planta a partir de sus planos, con mobiliario SLEEP'N editable. Es una web estática: HTML más imágenes, con three.js cargado desde jsDelivr, sin servidor ni compilación.

## Modelos

| Carpeta | Edificio | Fuente |
|---|---|---|
| `delicias16/` | Hotel Delicias 16 · Madrid (42 hab., 7 plantas) | Planos, sección y alzado del dossier comercial |

## Publicación

Se publica con GitHub Pages desde la rama `main`, en la raíz (Settings → Pages → Deploy from a branch → `main` / `(root)`).

## Añadir un modelo

1. Crea una carpeta con el `index.html` del visor y una `miniatura.jpg` (unos 750 × 630 px).
2. Añade una entrada en la lista `MODELOS` del `index.html` de la raíz.

## Guardado de las distribuciones

Fuera de Claude no hay base de datos compartida. Cada persona guarda sus cambios en su navegador (localStorage). Para compartir una distribución, se usa **Escenarios → Descargar .json** y quien la recibe la carga con **Importar JSON**.

## Delicias 16: precisión

- La escala de los planos rasterizados es de 50,67 px/m, ajustada con 10 estancias de la planta tipo; 9 de las 10 cuadran con el dossier dentro de ±1,6 %.
- Las cotas de cada planta salen de la sección A_09. El edificio tiene medios niveles entre el bloque trasero y el delantero.
- La pestaña **Datos** del visor compara cada estancia con el dossier y enumera los supuestos.
