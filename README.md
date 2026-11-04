# Inventario de Maquinarias

- `index.html`: el dashboard (un solo archivo).
- `data/maquinarias.json`: la base de datos (versión, ubicaciones y unidades con ID estable).
- `data/maquinarias.csv`: la misma base para abrir en Excel.

## Publicar en GitHub Pages
1. Crear un repositorio y subir estos archivos (conservando la carpeta `data/`).
2. Settings → Pages → Deploy from a branch → `main` / `(root)`.
3. Abrir `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Actualizar la base
1. Editar `data/maquinarias.json` (o reemplazarlo) y **subir el número de `version`**.
2. Al abrir el dashboard en cualquier equipo, detecta la versión nueva y la aplica sola.
3. Lo que se editó, agregó o eliminó localmente en ese equipo se respeta; el resto se actualiza.

Para convertir los cambios hechos en un equipo en la base compartida: botón **Exportar base (JSON)** y subir el archivo a `data/`.

## Guardar desde cualquier dispositivo (sincronización)
En el menú lateral: **Sincronización**. Pegá un token de GitHub (Settings → Developer settings → Fine-grained tokens), limitado a este repositorio y con permiso *Contents: Read and write*. El token queda solo en ese dispositivo.
Con la sincronización activa, cada alta, edición o baja se guarda en `data/maquinarias.json` y el resto de los dispositivos la recibe al abrir el dashboard.
`data/maquinarias.csv` no se actualiza solo: usá el botón **Exportar CSV** cuando lo necesites.
