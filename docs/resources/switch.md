---
layout: default
title: Switch & 3DS
parent: Recursos
nav_order: 6
---

# Switch & 3DS

## ROMS

- nxbrew.com
- ziperto.com
- romsfun.com
- archive.org/download/nintendo-3ds-cia-complete-rom-pack-romset
- emuparadise.me
- romsmania.cc
- psvitavpk.com
- gameginie.com

## Sobreescribir idioma de un juego

### Switch

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

### 3DS

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

