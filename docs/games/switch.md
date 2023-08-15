---
layout: default
title: Switch & 3DS
parent: Juegos
nav_order: 1
---

# Switch & 3DS

## Homebrew (Switch)

{: .warning-title }
> ¡Alerta!
>
> Recuerda que es un hack temporal y se borrará si se apaga. Por eso, cada vez que saques la SD, tendrás que inyectar el payload.

Para esto vas a tener que mirar que versión de Switch tienes, ya que hay versiones que no pueden ser hackeadas sin chip. Lo puedes comprobar en https://ismyswitchpatched.com/.

Echa un vistazo a la guia de Waifu (https://www.cfwaifu.com/atmosphere-tinfoil/) para ver como instalar Atmosphere y Tinfoil.

### Como actualizar la versión (Atmosphere)

{: .important-title }
> Nota
>
> Actualmente la última versión es 1.5.4 para Atmosphere, 16 para Tinfoil y 16.0.3 del SO oficial de Switch. ¡Atmosphere ya admite el último SO!

Es fácil, solo tienes que sustituir los ficheros de la nueva versión en la SD. Una vez hecho, metes la SD y conectas la Switch por USB al PC. Abres TegraRcmGUI y cargas el `fusee.bin`. Y listo, se abrirá tu switch hackeada.

#### Actualizar SO

¡Sí, puedes tener la última versión del SO oficial ya que Atmosphere lo soporta! En la 1.5.4 ya admite 16.0.3. Para actualizar, te descargas el firmware [aquí](https://switchscene.org/resources/categories/firmwares-oficiales.7/) y lo pasas a la SD. **Si vas a actualizar Atmosphere, te recomiendo pasarlo todo a la vez.**

Una vez encendida, ve al Album (donde accedes al homebrew) y abre Daybreak. Selecciona el directorio, les das a "Preserve settings", "Install (FAT32 + exFAT)" y le das a que instale… ¡Y listo, una vez reinicie estará actualizada! Tienes una guía visual [aquí](https://switchscene.org/threads/gu%C3%ADa-para-actualizar-el-firmware-de-la-switch-con-daybreak.2663/).

#### Tinfoil no arranca con la nueva versión

Esto pasa… Y me ha pasado. Lo que tienes que hacer es volver a instalar Tinfoil de nuevo, de limpio. Pasa la última versión de Tinfoil a la SD y accede al menú de Album. Al iniciar Tinfoil, debería instalarse.

¿Y si no se instala? ¡También me ha pasado! Puedes optar por instalar el `.nsp` con Goldleaf. Si no tienes [HB Appstore](https://github.com/fortheusers/hb-appstore/releases) te recomiendo instalarlo, solo tienes que arrastrarlo a la carpeta `switch`.

#### Los juegos no arrancan con la nueva versión

Clásico, porque te faltan los sigpatches. Atmosphere no apoya el pirateo así que tendrás que instalar los sigpatches para que los juegos instalados piratas funcionen. En el [repo de Github](https://github.com/THZoria/AtmoPack-Vanilla/releases) tienes todas las versiones de SO y Atmosphere, mira que sea la misma que la tuya y lo copias a la SD. Esto sobreescribe archivos de dos carpetas: bootloader y Atmosphere.

**Eso sí, esto tienes que hacerlo con la Switch apagada para que coja los sigpatches después.**

### Inyectar payload

Como he dicho, cada vez que sacas la SD tienes que cargar el payload ya que es un hack temporal (no permanente). Es fácil:

1. Conecta la Switch por USB.
2. Abre TegraRcmGUI.
3. Carga el `fusee.bin` de la versión que tengas (mira el Github de Atmosphere).

### Instalar juegos por USB directamente

Se puede hacer con Goldleaf y Quark (https://www.cfwaifu.com/goldleaf-quark/) o con Tinfoil (https://www.cfwaifu.com/tinfoil-nut/).

### Pasar juegos por USB

Si tienes las últimas versiones de Atmosphere, tendrás el USB File Transfer. Con él, podrás conectar la Switch al PC sin tener que sacar la SD y pasar por cable los archivos.

En PC te saldrá la carpeta al instante, lo detecta sin problema. En Mac, no te va a salir en el sistema de ficheros… Pero puedes usar OpenMTP para conectarte, funciona perfectamente.

### Sobreescribir idioma de un juego

{: .warning-title }
> ¡Alerta!
>
> Esto solo funciona si tienes la Switch hackeada y con Atmosphere

La opción fácil es cambiar el idioma de la Switch por el idioma que quieras, pero esto hará que todos los juegos estén en ese idioma. Por si lo que quieres es solo UN juego, la solución es esta:

1. **Busca el ID** del juego. Si te lo has descargado, podrás verlo en el nombre del fichero. Puedes mirarlo también con GoldLeaf: manage console contents > SD card > "nombre del juego" > base game. Si está en la NAND, tendrás que ir a mirar a NAND USER.
2. Accede a la SD `atmosphere/contents`.
3. Crea una nueva carpeta con el ID del juego que hemos buscado antes.
4. Crea un nuevo fichero `config.ini`. Dentro debe tener:

```
[override_config] 
override_language = ja 
override_region = jpn
```

- **Las regiones son:** jpn, usa, eur, aus, chn, kor, twn
- **Los idiomas son:** ja, en-US, fr, de, it, es, zh-Hant, zh-Hans, zh-CN, ko, nl, pt, ru, zh-TW, en-GB, fr-CA, es-419

## Homebrew (3DS)



### Sobreescribir idioma de un juego

{: .warning-title }
> ¡Alerta!
>
> Debes tener la consola con homebrew y usar Luma.

Si un juego peta por tener un idioma que no comprende (que puede pasar)…

1. Busca el **ID** del juego. Esto lo puedes mirar en Luma u [online aquí](http://3dsdb.com/).
2. Ir a la carpeta `luma` de la SD.
3. Crear carpeta `titles` dentro.
4. Crear una carpeta con el ID del juego.
5. Crear un fichero `locale.txt` con `JPN JP` dentro.
