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
