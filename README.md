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

## Delicias 16: recorrido virtual y personas

- **Recorrido virtual**: se anda en primera persona por todo el edificio (W A S D o flechas, Mayús para correr, arrastrar para mirar, tocar el suelo para ir, mando en el móvil). Escaleras por continuidad de cota, panel del ascensor con las plantas y «Ir a…» para saltar a cualquier estancia.
- **Personas**: de 1 a 4 huéspedes por habitación con órdenes («ve de la cama a la ducha», «todos a la puerta», «baja a desayunar por la escalera»). Cada recorrido da el largo y el paso más estrecho, medido de lado a lado entre muros y muebles en una rejilla de 5 cm (±5 cm).
- **Desayunos (Eat'N, planta baja)**: plazas con el mobiliario frente al aforo de referencia del CTE (1,5 m²/persona sentada), recorridos del camarero de la cocina a cada mesa y simulación del servicio (cola del buffet, mesas, camareros). Los parámetros de la simulación son supuestos y están escritos en el propio panel.
