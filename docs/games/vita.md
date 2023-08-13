---
layout: default
title: PS Vita
parent: Juegos
nav_order: 3
---

# PS Vita

Por qué PS Vita y no PSP es básicamente porque: ahora mismo la encuentras al mismo precio y la PS Vita ofrece mucho más rendimiento (además de juegos exclusivos) que la PSP.

## Hack sin ordenador

1. Asegúrate de que está actualizado con el último firmware (3.74).
2. Abre el navegador y escribe `deploy.psp2.dev`. O usa `lptutoriales.es/henlo` si lo quieres en español.
3. Click en **Unlock** o **Liberar mi Vita**.
4. Instala Vitadeploy (+ autoplugin2 si es la español) y después, Henkaku.
5. Cierra, ve a los ajustes > Ajustes de Henkaku > "Activar Homebrew inseguro".
6. Asegúrate de ir a Ajustes de ahorro de energía y cambia el modo espera a 30 min hasta que la tengas hackeada, para que no entre en reposo.
7. Abre VitaDeploy y click en "Install different OS" o "Instalar un SO diferente" en español. Una vez aquí, ve a "paquete actualización de PlayStation" y click en "Enso". **Esto hará el hack permanente**. Volvemos atrás y damos a "Instalación 3.65 rápida".
8. Una vez terminado, ve a Ajustes > Ajustes de Henkaku > Versión para Spoofing > Poner "3.74". Con esto podrás conectarte a juegos online.


### Apps a instalar

- VitaShell: para pasar archivos por FTP. **Lo puedes sustituir por ftpeverywhere**
- PKGj: para descagar juegos.
- Autoplugin: para instalar plugins. Si no has instalado por la versión español, vas a tener que instalarlo.
- BatteryFixer: para arreglar posibles errores de batería.
- Adrenaline: para jugar juegos de PSP.
- Adrenaline Bubbles Manager: para añadir acceso directo a los juegos en la screen de vita en vez de acceder a Adrenaline y arrancar el juego.

#### Plugins

Para instalarlos necesitas el Autoplugin.

- NoNpDrm: para poder usar juegos de PKGj sin problemas. **Obligatorio**
- reFOOD: para correr programas que no pueden ser desencriptados adecuadamente. **Obligatorio**
- ftpeverywhere: para acceder al ftp hagas lo que hagas (sin abrir la app de ficheros). **Obligatorio**
- ds4vita: si quieres usar tu DualShock 4 en la ps vita.
- Framecounter: si quieres controlar la tasa de frames.
- PSV-VSH MENU: para abrir el menú overclock desde el botón select.
- LCD Colour Space Changer: para emular colores de OLED.
- udcd_uvc: para hacer streaming del video por cable.

## Descargar juegos

Para esto vas a necesitar un sd2vita y una microsd.

### Usando PKGj

1. Abre VitaDeploy > Misceláneo > Formatear Tarjeta. Formatea la tarjeta nueva.
2. Reinicia.
3. Ve a los ajustes > almacenamiento > usar YAMT.
4. Reinicia.
5. Ve a VitaDeploy > File Manager. Copia todo el contenido de la carpeta UX0 dentro de UMA0. 
6. Vuelve a los ajustes de almacenamiento. Cambia UX0 a SD2Vita (para cambiar la por defecto) y UMA0 a Almacenamiento Interno.
7. Instala PKGj desde "App downloader" en VitaDeploy. Con las nuevas actualizaciones, puedes descargar tanto PS Vita como PSP. Solo tienes que usar los filtros, ¡incluso puedes filtar por región!
8. Al abrir la primera vez, tienes que abrir el menu derecho (triángulo) y click en "Refresh" para que descargue todas las opciones.

### Usando NoPaySation

Este programa es de PC y vas a tener que descargar y pasar a la vita los contenidos. Si te da pereza, opta por PKGj.

1. Descarga [pkg2zip](https://github.com/mmozeiko/pkg2zip). Sigue [este tut](https://www.reddit.com/r/VitaPiracy/comments/724ccu/tutorial_how_to_use_pkg2zip_on_macos/) si usas Mac.
1. Descarga los `.tsv` de las categorías que quieras en la web.
2. Descarga la app para tu sistema y abre la app.
3. Abre File > Options. Aquí te saldrán las rutas para cada categoría, donde tendrás que apuntar al fichero descargado. Tienes que apuntar a una carpeta para que coja los games, DLCs, Updates…
4. Configura el directorio donde quieres que se descarguen. Esta opción está algo más abajo, donde pone "Download and unpack dir".
5. Donde pone "Any pkg dec tool" tienes que apuntar al pkg2zip de antes. **Solo si tienes windows**
6. Elige el juego y haz click en download and unpack.

Mi recomendación es que lo hagas en un PC y no en Mac, ya que los conversores son `.exe` y pueden dar fallos.