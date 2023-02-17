---
title: Recursos
layout: default
nav_order: 7
---

# Recursos

## Índice
{: .no_toc .text-delta }

1. TOC
{:toc}

## Dificultad animes

Puedes ver el ranking de dificultad [aquí](https://jpdb.io/anime-difficulty-list).

## Juegos

En esta sección te voy a dar una lista de juegos recomendados que puedes usar para mejorar tu lectura o tu audio. Encontrarás un tabla donde verás si…

- Tiene furigana o no.
- Tiene audio log. Esto significa que puedes abrir el log (de todos los diálogos ya dichos) y volver a escucharlos todas las veces que quieras. ¡Y tienen el texto también! **Muy útil si no hemos pillado bien una palabra.**
- Tiene voice acting. Hay muchos juegos que, aunque tengan diálogos en japonés, no hablan = solo hay texto para leer. ¿Recuerdas los viejos Pokemon donde solo podías leer?

### Switch

| Nombre        | Nombre japonés          | ¿Voice / audio log? | ¿Voice / audio acting? | ¿furigana?
|:-------------|:------------------|:--------|:------------|:-------------|
| 13 sentinels: aegis rim           | 十三機兵防衛圏 | ✅ | ✅ | ❌ |
| Ni no kuni           | 二ノ国 | ❌ | ✅ | ✅ |
| Famicom detective club           | ファミコン探偵倶楽部 | ❌ | ✅ | ✅ |
| Buddy mission bond           | バディミッション BOND | ✅ | ✅ | Algunos |
| Persona 3 portable           | P3P | ✅ | ✅ | ❌ |
| Persona 4 golden           | P4G | ✅ | ✅ | ❌ |
| Persona 5 royal           | P5R | ✅ | ✅ | ❌ |
| Fire emblem: Fūin no Tsurugi           | ファイアーエムブレム封印の剣 | ✅ | ❌ | ❌ |
| Boku no natsuyasumi Tsurugi           | 僕の夏休み | ❌ | ❌ | ❌ |
| Yo-kai watch 1 y 4           | 妖怪ウォッチ | ❌ | ❌ | ✅ |
| Yokai gakuen Y           | 妖怪ウォッチJam: 妖怪学園Y 〜Nとの遭遇〜 | ✅ | ✅ | ✅ |
| Marco & the galaxy dragon           | マルコと銀河竜 | - | - | - |
| Dragon quest 11           | ドラゴンクエストXI 過ぎ去りし時を求めて | ❌ | ✅ | ✅ |
| Crayon shin chan           | クレヨンしんちゃん『オラと博士の夏休み』 | ❌ | ❌ | ✅ |
| Jack jeanne           | ジャックジャンヌ | - | - | - |
| Fuuraiki 4           | 風雨来記 | - | Casi no tiene voces | - |
| Triange strategy           | トライアングルストラテジー | ✅ | ❌ | ❌ |
| Akiba trip           | アキバズトリップ | ✅ | ❌ | ✅ |
| Megaton musashi           | メガトン級ムサシ | ❌ | ❌ | ✅ |
| Pokemon escarlata           | ポケットモンスター スカーレット | ❌ | ❌ | ✅ |
| Pokemon púrpura           | ポケットモンスター バイオレット | ❌ | ❌ | ✅ |
| Pokemon legends: arceus           | Pokémon LEGENDS アルセウス | ❌ | ❌ | ✅ <br> Usa kanjis antiguos que ya no se usan |
| Digimon survive           | デジモンサヴァイブ | ✅ | ✅ | ❌ |
| Blue reflection           | ブルー リフレクション 幻に舞う少女の剣 | ✅ | ✅ | ❌ |
| Danganronpa           | ダンガンロンパ | ✅ | ✅ | ❌ |
| Nekopara           | ネコぱら | ✅ | ✅ | ❌ |

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

## Dónde ver anime online

### Con subtítulos en japonés

- https://anisub.tv/
- http://animejpnsub.ezyro.com/?i=1
- https://animelon.com/
- https://9tsu.guru/
- https://nihonnobangumi.com/

### Con subtítulos en inglés (a veces tienes otros idiomas)

- https://zoro.to/home

### Con subtítulos en español

- https://www1.otakustv.com/

## Dónde leer manga online

### En japonés

- https://mangareader.to/
- https://bilingualmanga.net/
- https://djtguide.neocities.org/cor#manga
- https://itazuraneko.neocities.org/library/shousetu
- https://sai-zen-sen.jp/
- https://www.comico.jp/
- https://klmanga.com/ybed-jujutsu-kaisen-raw.html
- https://tonarinoyj.jp/
- http://mangareader.to/

### Decargar raws de manga

- https://dlraw.net/raw/
- https://dl-raw.co/category/novel/
- https://mangarawjp.io/%E7%B5%84%E9%95%B7%E5%A8%98%E3%81%A8%E4%B8%96%E8%A9%B1%E4%BF%82-raw-free/
- https://13dl.me/home/
- https://manga-zip.info/category/raw-manga/
- https://www.yaoiotaku.com/forums/topic/119747-happy-kuso-life-harada-jp/
- https://jraws.net/

## Gramática

- [Genki](https://genki3.japantimes.co.jp/en/student/)

## Dónde leer en japonés

### Historias para niños

- http://hukumusume.com/douwa/
- https://www.e-hon.jp/ehon_jp/index1.htm
- https://www.wasabi-jpn.com/japanese-lessons/fairy-tales-and-short-stories-with-easy-japanese/
- https://www.wasabi-jpn.com/japanese-lessons/materials-for-japanese-lessons-intensive-reading/

### Fácil

- https://matcha-jp.com/easy/
- https://www.nippontalk.com/en
- https://www.nhk.or.jp/school/ouchi/index.html
- https://tadoku.org/japanese/free-books/#l4

### Noticias

- https://www3.nhk.or.jp/news/easy/
- https://www3.nhk.or.jp/
- https://www.asahi.com/
- https://www.cnn.co.jp/
- https://www.nikkei.com/
- https://www.asahi.com/
- https://mainichi.jp/
- http://www.yomiuri.co.jp/
- https://alpha.japantimes.co.jp/
- https://kyoko-np.net/ (fake news)

### Light Novels

- https://yomujp.com/n3/
- https://syosetu.com/
https://watanoc.com/

### Literatura

- https://www.aozora.gr.jp/
- https://www.gutenberg.org/browse/languages/ja
- https://www.bauddha.net/#novel

### Otros

- https://www.clipstudio.net/oekaki
- https://toyokeizai.net/
- https://www.buzzfeed.com/jp#.sbzX5VlBA
- https://www.nippon.com/ja/
- https://www.orangepage.net/
- https://note.com/
- https://rocketnews24.com/
- https://b.hatena.ne.jp/
- https://www.1000moji.com/
- https://kinarino.jp/
- https://cancam.jp/
- https://www.lifehacker.jp/
- https://ameblo.jp/
- https://qiita.com/
- https://girlschannel.net/
- https://kakuyomu.jp/

## Comprobar % de uso de palabras

- https://furigana.info/
- https://tsukubawebcorpus.jp/search/

## Para segmentar frases

- https://ichi.moe/

## Listado de onomatopeyas

- https://onomatopedia.jp/
- https://japaslang.com/
- https://onomatopoeiamean.info/
- [Onomatodict-JP](https://github.com/matsumurae/onomatodict-jp)

## Si necesitas buscar respuesta…

https://oshiete.goo.ne.jp/

## Diccionarios

- https://app.kanjialive.com/search
- https://jisho.org/
- http://weblio.jp/
- https://ejje.weblio.jp/

## Dialectos de Japón

### Kansai

- http://static.kansaibenkyou.net/index.html

### Hakata (fukuoka)

- https://hougen.u-biq.org/fukuokaben.html
- https://www.tabikobo.com/tabi-pocket/japan/fukuoka/article58916.html