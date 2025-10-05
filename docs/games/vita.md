---
layout: default
title: PS Vita
parent: Juegos
nav_order: 3
---

# PS Vita

Por qué PS Vita y no PSP es básicamente porque: ahora mismo la encuentras al mismo precio y la PS Vita ofrece mucho más rendimiento (además de juegos exclusivos) que la PSP.

## A empezar!

1. Asegúrate de que está actualizado con el último firmware (3.74).
2. Abre el navegador y escribe `deploy.psp2.dev`. O usa `lptutoriales.es/henlo` si lo quieres en español.
3. Click en **Unlock** o **Liberar mi Vita**.
4. Instala Vitadeploy (+ autoplugin2 si es la español) y después, Henkaku.
5. Cierra, ve a los ajustes > Ajustes de Henkaku > "Activar Homebrew inseguro". En los ajustes de Henkaku, ve a Versión para Spoofing > Poner "3.74". Con esto podrás conectarte a juegos online.
6. Asegúrate de ir a Ajustes de ahorro de energía y cambia el modo espera a 30 min hasta que la tengas hackeada, para que no entre en reposo.
7. Desactiva las actualizaciones automáticas, yendo a Sistema > Ajustes de inicio automático > Desactiva "Descargar archivo de actualización para el software de sistema" (primera opción).
8. Abre VitaDeploy y click en "Install different OS" o "Instalar un SO diferente" en español. Una vez aquí, ve a "paquete actualización de PlayStation". Aquí seleccionamos:
   1. Firmware destino: 3.65
   2. Configuración de taiHEN: R + YAMT (última opción)
   3. Instalar enso ACTIVADO
9. Una vez seleccionado todo, damos a "instalar fimrware seleccionado".
10. Cuando termine (va a tardar un rato), abrimos VitaDeploy y vamos a "Descargador de Apps". Aquí elegimos:
    1.  VitaShell (para pasar archivos por FTP o USB)
    2.  ITLS installer
    3.  Adrenaline (para jugar PSP)
    4.  PKGj (store de juegos).
11. Después de seccionar, volvemos arriba y damos a Descargar apps seleccionadas.
12. Al terminar, lo primero que haremos es abrir ITLS y seleccionar la primera opción. Una vez termine, podemos borrar la app.
13. Ahora, configuremos Adrenaline. Al abrir, pedirá instalar firmware de PSP. Damos todo X y esperamos, cuando esté listo configuramos la PSP y ya la tenemos.
14. Abre Autoplugin 2 > Plugins de PS Vita > Instalar plugins y elegimos "Adrenaline by TheOfficialFlow".
15. Ahora ya por fin, abrimos PKGj y hacemos refresh (triángulo y click en refresh). Ya puedes descargar lo que quieras!

## SD2VITA

1. Ve a VitaDeploy > Misceláneos > Formatear almacenamiento. Aquí debe ser:
   1. Objetivo: SD2Vita
   2. Formato: TexFAT
2. Le damos a Formatear y esperamos.
3. Al terminar reiniciamos. Vamos a Ajustes > Dispositivos > Storage Devices. **Recuerda marcar la opción Use YAMT.** En uma0 debe poner SD2Vita. De no ser así, le hacemos click y lo elegimos de la lista.
4. Volvemos a reiniciar…  Ahora debemos copiar y transferir ux0 a uma0. Entramos a VitaShell, y usarlo como memoria principal. En ese caso, tienes que ir a VitaShell, vamos a ux0, pulsamos triángulo y Select all, volvemos a pulsar triángulo y Copy. Vamos a uma0 y pegamos todo. Volvemos a Storage Devices y aqui cambiamos ux0 a SD2Vita y um0 a tu memoria por defecto.

**Es importante cambiar SD2Vita a ux0 porque los juegos de vita deben estar sí o sí en ux0, aunque puedes tener lo de PSP en uma0.**

## Rutas

- Juegos de vita: ux0:/app
- Saves vita: ux0:/user/00/savedata
- PSP ISO: ux0:/pspemu/iso
- PSP EBOOT: ux0:/pspemu/psp
- Saves PSP: ux0:/PSP/SAVEDATA
- PS1: ux0:pspemu/PSP/game

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