# KanjiWidget dictionaries

Paquetes de datos descargables para [KanjiWidget](https://github.com/jefaz0/kanji-widget-android).

Este repositorio no contiene bases de datos en el historial Git. Los paquetes se publican exclusivamente como archivos adjuntos de cada **Release**.

## Uso por la aplicación

La aplicación incluye el paquete base en inglés y los datos de trazos necesarios para funcionar sin conexión desde el primer inicio.

Cuando el idioma del sistema lo requiera, KanjiWidget descarga automáticamente el paquete de idioma correspondiente desde la última Release y valida su tamaño y suma SHA-256 antes de activarlo. Los paquetes descargados quedan guardados en el dispositivo; las búsquedas siguen siendo locales e instantáneas.

## Assets previstos por Release

- `manifest.json`
- `dictionary_en_top10.db`
- `dictionary_es_en_top10.db`
- `dictionary_fr_en_top10.db`
- `dictionary_pt_en_top10.db`

Los archivos `.db` son datos SQLite generados. No deben subirse como archivos normales al repositorio.

## Publicar una versión

1. Generar los paquetes y el `manifest.json` con las herramientas del repositorio principal.
2. Crear una Release con etiqueta, por ejemplo, `v1`.
3. Adjuntar el manifiesto y los paquetes de esa versión.
4. Publicar la Release. La aplicación usará el manifiesto para conocer tamaños, hashes e idiomas disponibles.

## Licencias y atribuciones

Consulta [ATTRIBUTIONS.md](ATTRIBUTIONS.md).