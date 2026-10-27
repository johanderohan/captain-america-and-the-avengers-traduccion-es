# Captain America and the Avengers — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/mega-drive/captain-america-and-the-avengers)**.

Traducción al **español de España** de *Captain America and the Avengers*
(Mega Drive, 1992), el beat 'em up de Data East con licencia de Marvel.

La traducción se distribuye como **parche**: necesitas tu propia copia de la
ROM USA original. Este repositorio contiene únicamente este README;
el parche está en **[Releases](../../releases)**.

## Estado

Última versión: **[v1.0 — Historia, menús y rótulos en castellano](../../releases/tag/v1.0)**.

| Parte | Estado |
|---|---|
| Historia | Las 17 páginas de introducción de las cinco fases y el epílogo desplazable |
| Diálogos | Los 38 globos de diálogo en partida |
| Fichas de héroe | Biografías, datos en sistema métrico y títulos grandes (Capitán América, Iron Man, Visión, Ojo de Halcón) |
| Rótulos de escena | «Escena N» y los cinco subtítulos, con letras nuevas dibujadas |
| Menús e interfaz | Título, opciones, entrenamiento, créditos y puntuaciones |
| Marcador de partida | PULSA START, ESPERA, PAUSA, FIN DEL JUEGO y VIC= |
| Ortografía | Á É Í Ó Ú Ü Ñ ¡ ¿ en todas las fuentes del juego (que solo tenían mayúsculas) |
| Revisión durante una partida | Parcial |

**Se conservan** el logotipo, el aviso legal del arranque, la ilustración
«HELP!» y las onomatopeyas dibujadas (KRAK, WHAM…).

### Comprobaciones y límites

Se han comprobado en **Genesis Plus GX** el título y los menús, la introducción de
la fase 1, las páginas de las fases 2 a 5 y el epílogo (forzados con una ROM de
ensayo que no se distribuye), el primer globo en partida, las cuatro fichas, los
créditos, el marcador (PULSA START, ESPERA, PAUSA, FIN DEL JUEGO) y una partida
automática de unos 1.500 pasos con la fase 1. Los 38 globos y los cinco rótulos de
escena se han revisado además fuera del juego, dibujando sus mapas.

El parche se ha aplicado sobre el original y el resultado coincide **byte a
byte** con la ROM preparada. El checksum de cabecera es válido.

No se ha jugado el juego completo ni se ha visto el modo de dos jugadores
(«VIC=»); tampoco se ha probado en consola física. La traducción y su revisión han
contado con asistencia de IA; no hay revisión humana independiente ni es una
localización oficial.

## Cómo aplicar el parche

1. Descarga **[Captain-America-and-the-Avengers-es-ES-v1.0.xdelta](../../releases/download/v1.0/Captain-America-and-the-Avengers-es-ES-v1.0.xdelta)**.
2. Comprueba que tienes la ROM USA **original, sin cabecera adicional y sin otros parches**:

   | Dato | Valor |
   |---|---|
   | Archivo de referencia | `Captain America and the Avengers (USA).md` |
   | Tamaño | 1.048.576 bytes (1 MiB) |
   | CRC32 | `E0639CA2` |
   | MD5 | `1dc96693afd74e7b0623a6e06fbdcf87` |
   | SHA-256 | `8bb44d7e014719c8048326bd7a416863ec5deb7c00b6abbddd5e1a52a12dd908` |

3. Aplica el parche con **[Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases)**
   o con `xdelta3`:

   ```bash
   xdelta3 -d -s "Captain America and the Avengers (USA).md" Captain-America-and-the-Avengers-es-ES-v1.0.xdelta "Captain America and the Avengers (es-ES).md"
   ```

4. La ROM resultante ocupa también **1.048.576 bytes**. Su MD5 debe ser
   `6404dca6ac24f2c39cc6630995929d30` y su SHA-256:
   `c10aa4c07f3025b4e3c605382dd17f9dc28eeef43558b7a778057ed606722671`.
5. Inicia una partida nueva. No cargues un estado de emulador creado con otra versión.

Aplica cada versión sobre el **original USA**, no sobre una ROM traducida.

## Cambios por versión

- **v1.0** — Primera publicación.

## Aviso

Proyecto de traducción por afición, sin ánimo de lucro y sin relación con
Data East ni Marvel. No se distribuye la ROM, solo un parche para una copia propia.

Si eres titular de los derechos y quieres que lo retire, abre una incidencia.
