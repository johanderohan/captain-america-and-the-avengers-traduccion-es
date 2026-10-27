# Captain America and the Avengers — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/mega-drive/captain-america-and-the-avengers)**.

Traducción al **español de España** de *Captain America and the Avengers*
(Mega Drive, 1992), el beat 'em up de Data East con licencia de Marvel.

La traducción se distribuye como **parche**: necesitas tu propia copia de la
ROM USA original. Este repositorio contiene únicamente este README;
el parche está en **[Releases](../../releases)**.

## Estado

Última versión: **[v1.3 — J1/J2 con la fuente azul en entrenamiento](../../releases/tag/v1.3)**.

| Parte | Estado |
|---|---|
| Historia | Las 17 páginas de introducción de las cinco fases y el epílogo desplazable |
| Diálogos | Los 38 globos de diálogo en partida |
| Fichas de héroe | Biografías, datos en sistema métrico y títulos grandes (Capitán América, Iron Man, Visión, Ojo de Halcón) |
| Rótulos de escena | «Escena N» y los cinco subtítulos, con letras nuevas dibujadas |
| Menús e interfaz | Título, opciones, entrenamiento, créditos y puntuaciones |
| Marcador de partida | PULSA START, ESPERA, PAUSA, FIN DEL JUEGO y VIC= |
| Ortografía | Tildes, ñ y signos españoles en los textos traducidos; orientación de ¿ y ¡ corregida |
| Revisión durante una partida | Parcial |

**Se conservan** el logotipo, el aviso legal del arranque, la ilustración
«HELP!» y las onomatopeyas dibujadas (KRAK, WHAM…).

### Comprobaciones y límites

La **v1.3** corrige J1/J2 en los diálogos de entrenamiento: J y cifra usan la
misma fuente azul degradada. Comprobados ambos diálogos con los cuatro personajes
y dos rondas de entrenamiento ganadas mediante entradas de mando. Se conservan
las exclamaciones verticales de v1.2 y el resto de correcciones.

La **v1.2** redibuja «¡» y «!» verticales en las tres fuentes de texto, manteniendo
el grosor, el color y el contorno. La fuente que recarga el entrenamiento recibe
los mismos glifos. Se repitieron las pruebas de signos, opciones, entrenamiento
con dos mandos, créditos y Segador con esta versión. Solo cambian cuatro recursos
de fuente respecto a v1.1; los textos y las mecánicas se conservan.

La v1.1 corrige incidencias detectadas por un jugador en la v1.0. Gracias a
Wave por sus capturas y avisos. Las notas anteriores de v1.0 exageraban la
cobertura de entrenamiento y créditos; esta revisión las sustituye.

Comprobaciones en **Genesis Plus GX** sobre la candidata de v1.1:

- Arranque frío y cambios de dificultad: dos ciclos completos, sin tildes residuales.
- Entrenamiento con dos mandos: entrada desde el menú, dos rondas ganadas,
  resultado, diálogo posterior y regreso al título, mediante entradas de mando.
- Los cuatro nombres en ambos diálogos de entrenamiento, mediante prueba dirigida.
- Las catorce pantallas de créditos y FIN, mediante acceso dirigido a sus estados.
- Fichas y ranking; margen de Ojo de Halcón, J grande y etiqueta SALUD PERDIDA.
- Globo del Segador con el jefe presente: 100 fotogramas sin tinta de la última
  línea tapada, frente a 65 píxeles tapados en v1.0. La ruta se alcanzó por depuración.
- Revisión editorial del corpus extraído y auditoría de los 38 globos: ninguno
  supera la altura original. No se han recorrido las 38 escenas durante una partida.
- Orientación de signos, 387 recursos comprimidos sin solapamientos, checksum,
  reconstrucción reproducible y reaplicación del parche byte a byte.

La J del HUD se ha redibujado con el grosor y degradado original y comprobado en
J1/J2 y FIN DEL JUEGO. La revisión sigue siendo parcial: **no hay partida completa
ni prueba en consola física**. Los accesos dirigidos y las auditorías no sustituyen
esos recorridos. Traducción y correcciones asistidas por IA, con feedback humano
parcial; no es una localización oficial.

## Cómo aplicar el parche

1. Descarga **[Captain-America-and-the-Avengers-es-ES-v1.3.xdelta](../../releases/download/v1.3/Captain-America-and-the-Avengers-es-ES-v1.3.xdelta)**.
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
   xdelta3 -d -s "Captain America and the Avengers (USA).md" Captain-America-and-the-Avengers-es-ES-v1.3.xdelta "Captain America and the Avengers (es-ES).md"
   ```

4. La ROM resultante ocupa también **1.048.576 bytes**. Su MD5 debe ser
   `f3c16589c3d64eda60ec58347582e738` y su SHA-256:
   `aabef6d66d844824987de78e665399abd429255be810e18de5d41137a4552f48`.
5. Inicia una partida nueva. No cargues un estado de emulador creado con otra versión.

Aplica cada versión sobre el **original USA**, no sobre una ROM traducida.

## Cambios por versión

- **v1.3** — J1/J2 usan la fuente azul del HUD también en los diálogos de
  entrenamiento, antes y después del combate; reemplaza la J blanca.

- **v1.2** — Exclamaciones de apertura y cierre verticales, con punto separado;
  sustituyen los signos inclinados heredados del original. Capturas renovadas.

- **v1.1** — Corrige ¿/¡, tildes residuales al cambiar dificultad, J del HUD,
  J1/J2, margen de la biografía y J grande de Ojo de Halcón, superposición del
  globo del Segador y alturas de otros tres globos. Completa entrenamiento,
  cargos de créditos y FIN. Aclara SALUD PERDIDA en el ranking y mejora dos frases.
- **v1.0** — Primera publicación; contenía los defectos corregidos en v1.1.

## Aviso

Proyecto de traducción por afición, sin ánimo de lucro y sin relación con
Data East ni Marvel. No se distribuye la ROM, solo un parche para una copia propia.

Si eres titular de los derechos y quieres que lo retire, abre una incidencia.
