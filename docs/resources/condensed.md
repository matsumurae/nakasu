---
layout: default
title: Audio condensado
parent: Recursos
nav_order: 1
---

## Audio condensado

En esos momentos en los que no tenemos tiempo de ponernos a ver una serie, existe el audio condensado. No es más que el audio al que se le ha quitado todas esas partes que no tienen diálogo: esto hace el capítulo más corto.

**Podemos escucharlo en el coche, en el metro… ¡Donde quieras!**

- [Condensed Audio Catalog](https://condensedaudiocatalog.com/)
- [Carpeta Mega](https://mega.nz/folder/8HhhWDyJ#SHw5xsYxyhWUX536UcqkeQ)
- [Carpeta Drive](https://drive.google.com/drive/folders/1gDpwFl07a0EO_pTHLLVn_Waz2GXwwSE1)
- [Itazuraneko](https://itazuraneko.neocities.org/library/librarymain.html)

### Cómo extraer audio condensado

Es posible que no encuentres la serie que te gusta… Si eso pasa, puedes hacerlo tú mismo.

- Si es un anime / serie, utiliza [subs2cia](https://github.com/dxing97/subs2cia).
- Si es un video de youtube, utiliza [Youtube Condensed Audio](https://github.com/the-bose/youtube-condensed-audio).

#### Subs2cia

Para poder usar esto vas a necesitar Python 3 y ffmpeg. Si no lo tienes, busca en google cómo instalar Python en tu sistema. **Recuerda que todo se hace por comdandos.**

1. Primero tenemos que instalarlo usando `py -m pip install subs2cia` en Windows, `brew install python ffmpeg` en Mac o `pip3 install subs2cia` en Linux.
2. Una vez lo tenemos, solo tienes que usar `subs2cia condense -i "nombre.mkv`.
3. Puedes pasar los subs que prefieres usando `-tl idioma`: english, japanese, spanish… Tienes que ponerlo en inglés.
4. Puedes usarlo con multiples archivos usando un bucle `subs2cia condense -b -i *.mkv *.srt -I 0m 1m30s -I e2m +1m30s -tl ja -t 1500 -p 100`.

#### Youtube condensed audio

1. Solo tienes que ir a Github y descargar la release de tu sistema (Win o Mac).
2. Dentro de un archivo `config.txt` colocarás:
   1. `link` enlace al video o playlist
   2. `speed` si quieres tener los videos más rápidos o más lentos (por defecto 1).
3. Luego solo tienes que abrir el `.exe` o app para ejecutarlo. Recuerda que el archivo `config.txt` debe estar en el mismo lugar la aplicación.