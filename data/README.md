# Datos de TraceLab

Las imágenes **no están en este repositorio** por su tamaño. Se descargan desde el enlace indicado abajo.

**Enlace de descarga:** `[COMPLETAR: enlace de Drive con permiso de lectura para cualquiera con el enlace]`
**Procedencia y licencia:** `[COMPLETAR: de dónde salieron las imágenes y bajo qué permisos se comparten]`

## Contenido

| Modalidad | Fácil | Intermedio | Difícil | Total |
|---|---|---|---|---|
| Mandalas | 300 | 300 | 300 | 900 |
| Siluetas | 100 | 100 | 100 | 300 |
| **Total** | | | | **1.200** |

Formatos: PNG y JPG.

## División (semilla 42)

| Conjunto | Imágenes | Uso |
|---|---|---|
| train | 600 | explorar y diseñar el comparador |
| val | 180 | explorar parámetros (tolerancia, pesos) |
| test | 180 | evaluación final, usada una sola vez |
| reto | 240 | banco de imágenes que ve el usuario en la app |

La división es estratificada por modalidad y nivel. Antes de dividir se agruparon los casi duplicados (dHash 32×32, distancia de Hamming ≤ 69) y cada grupo quedó completo en un mismo conjunto. El archivo `division_dataset_v2.csv` registra la asignación de cada imagen.

## Dibujos de personas

Los dibujos que las personas suben en la app se guardan **solo con consentimiento**, de forma anónima (`<imagen>__<código>.jpg`) y en la carpeta `Dataset/dibujos_usuarios/`. Esa carpeta está excluida del repositorio (`.gitignore`) para proteger la privacidad.
