# Resultados de tono por medio — NotebookLM

> Codificación manual asistida por IA (NotebookLM). Una pasada por medio.
> Escala: FAVORABLE / NEUTRAL / DESFAVORABLE / NO APARECE.
> Criterio de conservadurismo: ante la duda, NEUTRAL.
> Fuente de datos: ficheros .txt de `data/txt/` (artículos con cuerpo completo).

---

## Tabla resumen

| Medio | N arts. | Fav F | Neu F | Desf F | Fav R | Neu R | Desf R | Tono neto F | Tono neto R | Ratio vis. R/F | Marco |
|-------|--------:|------:|------:|-------:|------:|------:|-------:|:-----------:|:-----------:|:--------------:|-------|
| Marca          |     138 |   ~40 |   ~25 |     ~8 |   ~60 |   ~25 |     ~5 | **+32** | **+55** | 3,8× | David vs. Goliat |
| ABC            |      96 |     7 |   ~65 |      7 |     8 |   ~65 |      9 |   **0** |  **−1** | 2,6× | Confrontación total |
| El Confidencial |      51 |     3 |     3 |      8 |    25 |     4 |      0 |  **−5** | **+25** | 2,1× | Crisis institucional vs. candidatura salvadora |
| El Mundo        |      62 |     6 |   ~23 |      8 |    23 |   ~23 |      2 |  **−2** | **+21** | 2,9× | Pugna generacional / David vs. Goliat |
| elDiario.es     |       9 |     0 |     5 |      4 |     6 |     3 |      0 |  **−4** |  **+6** | 4,0× ⚠️ | Gestión en crisis vs. candidatura ilusionante |
| Europa Press    |      20 |     1 |    11 |      8 |    12 |     6 |      2 |  **−7** | **+10** | 13× ⚠️ | Candidatura salvadora vs. privatización opaca |
| OkDiario        |      97 |   ~31 |   ~32 |     ~2 |   ~21 |   ~32 |    ~12 | **+29** |  **+9** | 1,1× | Continuismo arrollador vs. alternativa ruidosa e inexperta |
| The Objective   |      24 |     1 |    17 |      6 |    10 |    12 |      2 |  **−5** |  **+8** | 15× ⚠️ | Crisis/desgaste vs. regeneración e ilusión |
| El Español      |      28 |    14 |     4 |      0 |     4 |     4 |      6 | **+14** |  **−2** | 0,57× ✅ | Certeza histórica vs. improvisación/peligro |
| ESPN Deportes   |      21 |     4 |     7 |      2 |     6 |     7 |      2 |  **+2** |  **+4** | 2,2× ⚠️ | Intercambio de golpes; gestión manchada vs. promesas caóticas |
| Heraldo.es      |      23 |     5 |     8 |      2 |     7 |     8 |      1 |  **+3** |  **+6** | 1,4× ⚠️ | Confrontación polarizada; estabilidad histórica vs. regeneración |
| Infobae         |      87 |   ~20 |   ~25 |     ~7 |   ~32 |   ~25 |     ~3 | **+13** | **+29** | 1,4× | Guerra mediática; gestión histórica vs. candidatura ilusionante |
| La Vanguardia   |      51 |     7 |     8 |     14 |    20 |     8 |      2 |  **−7** | **+18** | 1,2× | Fin de ciclo/desgaste vs. disrupción democrática ilusionante |
| Vozpopuli       |      20 |     3 |     3 |      4 |    10 |     3 |      0 |  **−1** | **+10** | 0,78× ⚠️ | Candidatura democratizadora vs. privatización calculadora |
| RTVE.es         |      23 |     2 |    11 |      2 |     7 |    11 |      1 |   **0** |  **+6** | 1,4× ⚠️ | Confrontación; gestión histórica en crisis vs. candidatura de cambio |
| Sport           |      78 |     6 |   ~27 |     18 |    25 |   ~27 |      2 | **−12** | **+23** | 1,6× | Crisis deportiva e institucional vs. "higiene democrática" / privatización |
| OneFootball     |      22 |     2 |     6 |      3 |     7 |     6 |      4 |  **−1** |  **+3** | 3,5× ⚠️ | Confrontación polarizada; desgaste institucional vs. ilusión/regeneración |
| Onda Cero       |      17 |     3 |    ~6 |      3 |     7 |    ~6 |      3 |   **0** |  **+4** | 1,8× ⚠️ | Polarización: blindaje institucional vs. urgencia democrática/privatización |
| Mundo Deportivo |      88 |    14 |   ~25 |     11 |    32 |   ~25 |      6 |  **+3** | **+26** | 1,6× | Regeneración democrática vs. autoritarismo/privatización; crisis institucional |
| Libertad Digital |      32 |     9 |    13 |      0 |     4 |    13 |      6 |  **+9** |  **−2** | 1,7×† | Defensa histórica vs. candidatura de sospecha/desestabilización |
| LaSexta          |      11 |     7 |     3 |      0 |     1 |     3 |      2 |  **+7** |  **−1** | 0,5× ⚠️ | Gestión histórica amenazada por confrontación desestabilizadora |
| La Razón         |      24 |    20 |     4 |      0 |     0 |     4 |      5 | **+20** |  **−5** | 0,05×† | Gestión mesiánica/histórica vs. desestabilizadores con intereses ocultos |
| Expansión        |      33 |     9 |    ~8 |      7 |    18 |    ~8 |      3 |  **+2** | **+15** | 3,2× | Confrontación empresarial: modelo de propiedad, privatización, ACS vs. Cox |
| ESdiario         |      17 |     7 |     5 |      2 |     6 |     5 |      4 |  **+5** |  **+2** | 1,0× ⚠️ | Confrontación institucional: legado histórico vs. cambio democratizador |
| El Periódico     |     ~40 |     2 |   ~12 |     11 |    13 |   ~12 |      2 |  **−9** | **+11** | 1,6× | Crisis institucional/autoritarismo vs. regeneración democrática necesaria |
| El HuffPost      |      13 |     0 |     6 |      7 |     9 |     1 |      0 |  **−7** |  **+9** | 2,7× ⚠️ | Régimen desgastado/autoritario vs. candidatura ilusionante de renovación |
| El Desmarque     |      58 |    16 |     9 |      5 |    24 |     9 |      4 | **+11** | **+20** | 1,7× | Confrontación total: candidatura ilusionante vs. gestión histórica defensiva |
| El Debate        |      44 |    16 |    28 |      0 |     2 |    35 |      7 | **+16** |  **−5** | 0,9× | Gestión histórica protege el club vs. desestabilización externa/sospechosa |
| El Correo †      |      14 |     2 |     6 |      3 |     5 |     6 |      0 |  **−1** |  **+5** | 7× ⚠️ | Confrontación de modelos: continuismo histórico vs. candidatura ilusionante |
| Defensa Central  |      51 |   ~34 |   ~11 |      0 |    ~4 |   ~11 |    ~18 | **+34** | **−14** | 0,65× | Gestión histórica indiscutible vs. oposición inexperta/oportunista |
| COPE             |      81 |    12 |    18 |     14 |    34 |    18 |      3 |  **−2** | **+31** | 1,6× | Confrontación institucional: referéndum sobre privatización vs. socios |
| Cadena SER       |      82 |    16 |     5 |     17 |    38 |     5 |      6 |  **−1** | **+32** | 1,7× | Candidatura ilusionante/rupturista vs. gestión histórica desgastada |
| Antena 3         |      48 |     8 |     7 |      6 |    22 |     7 |      5 |  **+2** | **+17** | 2,1×† | Candidatura renovadora vs. gestión histórica defensiva/amenazada |
| 20Minutos        |      62 |    11 |    13 |     10 |    19 |    13 |      9 |  **+1** | **+10** | 2,8× | Confrontación: privatización vs. aventureros; gestión histórica vs. disrupción |

---

## Fichas por medio

### Marca
- **Artículos analizados:** 138
- **Florentino Pérez**
  - Favorables: ~40
  - Neutrales: ~25
  - Desfavorables: ~8
- **Enrique Riquelme**
  - Favorables: ~60
  - Neutrales: ~25
  - Desfavorables: ~5
- **Marco narrativo:** Confrontación inesperada ("David contra Goliat"). Celebra que "hay partido" tras 20 años sin urnas. Riquelme = audaz retador con ilusión; Florentino = legendario pero a la defensiva y desgastado.
- **Visibilidad (protagonismo en titular):**
  - Riquelme: 87 titulares (65 en solitario)
  - Florentino: 39 titulares (17 en solitario)
  - Ambos juntos: 22 titulares
  - **Ratio de visibilidad Riquelme/Florentino (en solitario): ~3,8×**
- **Notas:** El medio amplifica masivamente la campaña de Riquelme (fichajes, apoyos, análisis financiero). Florentino recibe tono favorable en actos y encuestas, pero desfavorable en piezas de opinión (elecciones "clandestinas", miedo al rival, uso de bots).

---

### ABC
- **Artículos analizados:** 96
- **Florentino Pérez**
  - Favorables: 7
  - Neutrales: ~65 (mayoría teletipos de agencia)
  - Desfavorables: 7 (pitos en Bernabéu, acusaciones crisis financiera, pasividad Negreira, motín interno, caso Laghari)
- **Enrique Riquelme**
  - Favorables: 8
  - Neutrales: ~65
  - Desfavorables: 9 (intereses ocultos, aval de Andorra/CNMV, herencia Calderón, reprimenda Junta Electoral, bulos Haaland)
- **Tono neto Florentino:** 7F − 7D = **0** (equilibrado)
- **Tono neto Riquelme:** 8F − 9D = **−1** (levemente desfavorable)
- **Visibilidad (protagonismo principal del artículo):**
  - Riquelme: 55 artículos (57%)
  - Florentino: 21 artículos (22%)
  - Generales/comparativos/proceso: 21 artículos (22%)
  - **Ratio de visibilidad Riquelme/Florentino: 2,6×**
- **Causa según el propio medio:** estrategia mediática agresiva de Riquelme (candidato desconocido que necesita exposición) vs. estrategia de mínimos riesgos de Florentino (favorito que no quiere desgastarse). El medio lo atribuye a las estrategias, no a una decisión editorial.
- **Marco narrativo:** Confrontación total ("el barro llega a las elecciones"). Gestión histórica e invencible del oficialismo vs. candidatura disruptiva e ilusionante. Atravesado por miedo a crisis institucional y posible privatización.
- **Notas:** Cobertura dominada por teletipos de agencia sin carga valorativa (~68%). Tono prácticamente neutro para ambos (0 vs. −1). Pero la visibilidad es muy asimétrica: Riquelme aparece como protagonista 2,6 veces más que Florentino. Esto puede reflejar la dinámica real de campaña (el retador genera más noticias) o una decisión editorial de dar más espacio al desafiante. Distinguir ambas causas es clave para H_A vs. H_B.

---

### El Confidencial
- **Artículos analizados:** 51
- **Florentino Pérez**
  - Favorables: 3 · Neutrales: 3 · Desfavorables: 8
  - **Tono neto: −5**
- **Enrique Riquelme**
  - Favorables: 25 · Neutrales: 4 · Desfavorables: 0
  - **Tono neto: +25**
- **Visibilidad:** Riquelme 29 arts. · Florentino 14 arts. · Generales 8 · **Ratio: 2,1×**
- **Marco narrativo:** Crisis institucional vs. candidatura salvadora. Florentino = autoritario, a la defensiva, privatizador; Riquelme = salvador democrático, ilusionante, empoderador del socio.
- **Notas:** El medio más desequilibrado hasta ahora. Riquelme tiene 0 artículos desfavorables; Florentino tiene 8. El tono hacia Florentino es explícitamente negativo (lenguaje catastrofista: "rocambolesca comparecencia", "atrinchera en su palco", "miedo a que le muevan la silla"). Predecido por el preregistro como pro-Riquelme? No estaba en la lista explícita, pero el patrón es inequívoco.

---

### El Mundo
- **Artículos analizados:** 62 (63 totales, 1 descartado por ser sobre política nacional)
- **Florentino Pérez**
  - Favorables: 6 · Neutrales: ~23 (compartidos) · Desfavorables: 8
  - **Tono neto: −2**
- **Enrique Riquelme**
  - Favorables: 23 · Neutrales: ~23 (compartidos) · Desfavorables: 2
  - **Tono neto: +21**
- **Visibilidad:** Riquelme ~35 arts. · Florentino ~12 arts. · Mixtos/generales ~15 · **Ratio: 2,9×**
- **Marco narrativo:** Pugna generacional y David contra Goliat. Riquelme = irruptivo, valiente, ilusionante. Florentino = poderoso, institucionalizado, a la defensiva, opaco.
- **Notas:** Patrón similar a El Confidencial: tono negativo hacia Florentino (8 desfavorables, lenguaje duro: "esperpéntica", "victimista", "soberbia") con crítica residual a Riquelme (2 desfavorables, vinculación caso Aldesa/Plus Ultra). El preregistro no predecía sesgo en El Mundo — los datos muestran inclinación pro-Riquelme moderada.

---

### elDiario.es
- **Artículos analizados:** 9 ⚠️ muestra pequeña — interpretar con cautela
- **Florentino Pérez**
  - Favorables: 0 · Neutrales: 5 · Desfavorables: 4
  - **Tono neto: −4**
- **Enrique Riquelme**
  - Favorables: 6 · Neutrales: 3 · Desfavorables: 0
  - **Tono neto: +6**
- **Visibilidad:** Riquelme 4 arts. propios · Florentino 1 art. propio · Comparativos 4 · **Ratio: 4,0×**
- **Marco narrativo:** Gestión en crisis/opaca vs. candidatura ilusionante de regeneración. Florentino = deuda, riesgo de privatización, desgaste. Riquelme = líder transparente, protector del socio.
- **Notas:** El patrón más extremo hasta ahora en tono: 0 favorables a Florentino, 0 desfavorables a Riquelme. Pero con solo 9 artículos la muestra es demasiado pequeña para extraer conclusiones firmes — un artículo representa el 11% del total. Sesgo de cobertura coherente con la línea editorial progresista del medio.

---

### Europa Press
- **Artículos analizados:** 20 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 1 · Neutrales: 11 · Desfavorables: 8
  - **Tono neto: −7**
- **Enrique Riquelme**
  - Favorables: 12 · Neutrales: 6 · Desfavorables: 2
  - **Tono neto: +10**
- **Visibilidad:** Riquelme 13 arts. propios · Florentino 1 art. propio · Comparativos 6 · **Ratio: 13×**
- **Marco narrativo:** Candidatura ilusionante/salvadora vs. privatización opaca y crisis financiera. Elecciones enmarcadas como "referéndum existencial" sobre la soberanía del socio.
- **Notas:** ⚠️ Llamativo porque Europa Press es una agencia de noticias, se supone neutral por definición. Sin embargo muestra el peor tono neto para Florentino de todos los medios hasta ahora (−7) y el ratio de visibilidad más extremo (13×). Los 8 artículos desfavorables a Florentino amplifican acusaciones de Riquelme "sin filtro" según el propio análisis. Esto merece vigilancia especial: si Europa Press va sesgada, sus despachos contaminan a todos los medios que los republiquen (efecto multiplicador).

---

### OkDiario
- **Artículos analizados:** 97
- **Florentino Pérez**
  - Favorables: ~31 · Neutrales: ~32 · Desfavorables: ~2
  - **Tono neto: +29**
- **Enrique Riquelme**
  - Favorables: ~21 · Neutrales: ~32 · Desfavorables: ~12
  - **Tono neto: +9**
- **Visibilidad:** Riquelme ~39 arts. · Florentino ~36 arts. · Generales ~22 · **Ratio: 1,1×** (prácticamente equilibrado)
- **Marco narrativo:** Continuismo arrollador vs. alternativa ruidosa e inexperta. Florentino = patriarca indiscutible, garante de estabilidad. Riquelme = inicialmente ilusionante, termina bajo sombra de descrédito por desmentidos.
- **Notas:** ✅ **Primer medio que invierte el patrón**: más favorables a Florentino (31) que a Riquelme (21), y más desfavorables a Riquelme (12) que a Florentino (2). También es el único con visibilidad equilibrada (1,1×). Los 12 desfavorables a Riquelme se centran en desmentidos concretos (Manchester City/Haaland, Nadal, Kroos, Casillas, Mijatovic). Coincide exactamente con la predicción del preregistro: OkDiario pro-Florentino.

---

### The Objective
- **Artículos analizados:** 24 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 1 · Neutrales: 17 · Desfavorables: 6
  - **Tono neto: −5**
- **Enrique Riquelme**
  - Favorables: 10 · Neutrales: 12 · Desfavorables: 2
  - **Tono neto: +8**
- **Visibilidad:** Riquelme 15 arts. propios · Florentino 1 art. propio · Compartidos 8 · **Ratio: 15×**
- **Marco narrativo:** Confrontación por el modelo de propiedad. Florentino = desgastado, debilitado (Superliga, caso Negreira, falta de títulos). Riquelme = campaña mediática agresiva, promesas transformadoras.
- **Notas:** ⚠️ Muestra pequeña (24 arts.). Patrón pro-Riquelme moderado en tono (+8 vs −5). El ratio de visibilidad (15×) es el más extremo registrado pero con solo 15 vs 1 artículo en solitario, poco fiable. Hay autocrítica interna: un artículo de opinión ("navajazos") es desfavorable para ambos, y otro critica las promesas de Riquelme como "chuscas".

---

### El Español
- **Artículos analizados:** 28 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 14 · Neutrales: 4 · Desfavorables: 0
  - **Tono neto: +14**
- **Enrique Riquelme**
  - Favorables: 4 · Neutrales: 4 · Desfavorables: 6
  - **Tono neto: −2**
- **Visibilidad:** Florentino 14 arts. · Riquelme 8 arts. · Generales 6 · **Ratio R/F: 0,57×** (Florentino domina)
- **Marco narrativo:** Certeza del éxito histórico vs. improvisación y peligro. Florentino = solvencia, legado, independencia económica, víctima de ataques. Riquelme = intento vacío, desestabilizador, vinculado al pasado oscuro (Calderón), promesas imposibles.
- **Notas:** ✅ **Segundo medio pro-Florentino**, confirmando la predicción del preregistro. Es también el **único medio donde Florentino domina la visibilidad** (ratio 0,57× inverso). 0 artículos desfavorables a Florentino, 6 desfavorables a Riquelme. El espejo exacto de El Confidencial pero en la dirección opuesta.

---

### ESPN Deportes
- **Artículos analizados:** 21 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 4 · Neutrales: 7 · Desfavorables: 2
  - **Tono neto: +2**
- **Enrique Riquelme**
  - Favorables: 6 · Neutrales: 7 · Desfavorables: 2
  - **Tono neto: +4**
- **Visibilidad:** Riquelme 13 arts. · Florentino 6 arts. · Mixtos 2 · **Ratio: 2,2×**
- **Marco narrativo:** Confrontación abierta / intercambio de golpes. Florentino manchado por crisis deportiva y sospechas de privatización. Riquelme ilusionante pero con promesas desmentidas y caos mediático.
- **Notas:** ⚠️ Muestra pequeña. El medio más equilibrado en tono después de ABC (+2 vs +4). Ambos candidatos reciben el mismo número de artículos desfavorables (2 cada uno). Medio latinoamericano con cobertura más distante y menos implicada editorialmente.

---

### Heraldo.es
- **Artículos analizados:** 23 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 5 · Neutrales: 8 · Desfavorables: 2
  - **Tono neto: +3**
- **Enrique Riquelme**
  - Favorables: 7 · Neutrales: 8 · Desfavorables: 1
  - **Tono neto: +6**
- **Visibilidad:** Riquelme 10 arts. · Florentino 7 arts. · Generales 6 · **Ratio: 1,4×**
- **Marco narrativo:** Confrontación abierta y polarizada ("guerra de cromos"). Estabilidad histórica vs. candidatura regeneradora que alerta sobre privatización.
- **Notas:** ⚠️ Muestra pequeña. De los medios analizados, es el más equilibrado junto con ESPN y ABC. Ambos candidatos reciben tono positivo (ambos con tono neto positivo). La diferencia (3 vs 6) es mínima. Curioso: los 2 desfavorables a Florentino incluyen citas de Ramón Calderón ("gagá", "senil"), que son especialmente duras pero proceden de una fuente externa, no de la línea editorial propia.

---

### Infobae
- **Artículos analizados:** 87 (91 totales, 4 irrelevantes descartados)
- **Florentino Pérez**
  - Favorables: ~20 · Neutrales: ~25 · Desfavorables: ~7
  - **Tono neto: +13**
- **Enrique Riquelme**
  - Favorables: ~32 · Neutrales: ~25 · Desfavorables: ~3
  - **Tono neto: +29**
- **Visibilidad:** Riquelme ~37 arts. · Florentino ~26 arts. · Mixtos ~24 · **Ratio: 1,4×**
- **Marco narrativo:** Confrontación y crisis institucional. "Guerra" entre gestión mercantil/privatizadora (Florentino) vs. candidatura romántica que devuelve el club a los socios (Riquelme).
- **Notas:** Infobae es latinoamericano (Argentina), lo que da perspectiva distante. Aun así muestra tono pro-Riquelme claro (+29 vs +13). Destaca que da cobertura a los audios de Florentino insultando a leyendas del club ("estafas", "zoquetes") — uno de los pocos medios que lo menciona explícitamente como desfavorable. La visibilidad es la más equilibrada de los medios pro-Riquelme (1,4×).

---

### La Vanguardia
- **Artículos analizados:** 51
- **Florentino Pérez**
  - Favorables: 7 · Neutrales: 8 · Desfavorables: 14
  - **Tono neto: −7**
- **Enrique Riquelme**
  - Favorables: 20 · Neutrales: 8 · Desfavorables: 2
  - **Tono neto: +18**
- **Visibilidad:** Riquelme 22 arts. · Florentino 19 arts. · Generales 10 · **Ratio: 1,2×** (casi equilibrado)
- **Marco narrativo:** Fin de ciclo y desgaste vs. disrupción democrática ilusionante. Florentino = autoritario, en crisis, privatizador. Riquelme = candidato de los socios, dinamizador.
- **Notas:** Visibilidad casi equilibrada (1,2×) pero tono muy asimétrico: 14 desfavorables a Florentino vs. solo 2 a Riquelme. La Vanguardia es el caso más claro de medio con visibilidad equilibrada pero encuadre editorialmente decantado — el sesgo no es de silencio a Florentino sino de encuadre negativo activo. Destacable: acusa al equipo de Florentino de usar IA para "fingir" el apoyo de Mourinho.

---

### Vozpopuli
- **Artículos analizados:** 20 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 3 · Neutrales: 3 · Desfavorables: 4
  - **Tono neto: −1**
- **Enrique Riquelme**
  - Favorables: 10 · Neutrales: 3 · Desfavorables: 0
  - **Tono neto: +10**
- **Visibilidad:** Florentino 9 arts. · Riquelme 7 arts. · Compartidos 4 · **Ratio R/F: 0,78×** (Florentino ligeramente más visible)
- **Marco narrativo:** Candidatura democratizadora e ilusionante vs. gestión histórica en vías de privatizar el club.
- **Notas:** ⚠️ Muestra pequeña. Caso interesante: Florentino tiene más presencia (9 vs 7 artículos) pero el encuadre de esos artículos es mayoritariamente negativo (ingeniería legal, presiones al Ibex, falta de transparencia). Riquelme tiene 0 desfavorables. El medio acusa explícitamente a Florentino de presionar al Ibex 35 para boicotear financieramente a su rival — acusación grave que merece verificación documental.

---

### RTVE.es
- **Artículos analizados:** 23 ⚠️ muestra pequeña
- **Florentino Pérez**
  - Favorables: 2 · Neutrales: 11 · Desfavorables: 2
  - **Tono neto: 0**
- **Enrique Riquelme**
  - Favorables: 7 · Neutrales: 11 · Desfavorables: 1
  - **Tono neto: +6**
- **Visibilidad:** Riquelme 11 arts. · Florentino 8 arts. · Mixtos 4 · **Ratio: 1,4×**
- **Marco narrativo:** Confrontación y guerra empresarial. Gestión histórica prolongándose tras crisis interna vs. candidatura ilusionante que promete democratizar el club.
- **Notas:** ⚠️ Muestra pequeña. RTVE es la televisión pública, se supone neutral por mandato institucional. Los datos muestran tono neto 0 para Florentino (equilibrado) pero +6 para Riquelme — una ligera inclinación. Los 2 desfavorables a Florentino incluyen calificativos fuertes ("machista", "hombre enfadado") en columnas de opinión. Con solo 23 artículos los resultados son poco concluyentes.

---

### Sport
- **Artículos analizados:** 78
- **Presencia por candidato:** Riquelme ~36 arts. · Florentino ~22 arts. · Generales/compartidos ~20
- **Florentino Pérez**
  - Favorables: 6 · Neutrales: ~27 (compartidos) · Desfavorables: 18
  - **Tono neto: −12** ⚠️ peor registro hasta ahora
- **Enrique Riquelme**
  - Favorables: 25 · Neutrales: ~27 (compartidos) · Desfavorables: 2
  - **Tono neto: +23**
- **Visibilidad:** Riquelme 36 arts. · Florentino 22 arts. · **Ratio: 1,6×**
- **Marco narrativo:** Crisis deportiva e institucional vs. necesidad de "higiene democrática". El proceso electoral se enmarca como un plebiscito sobre el modelo de socios: privatización opaca (Florentino) vs. renovación transparente (Riquelme). Las promesas de fichajes de Riquelme se presentan con ángulo positivo ("dinamita", "genial"); los desmentidos se recogen sin el mismo énfasis crítico.
- **Notas:** Sport es el medio con el **tono más negativo para Florentino** de todos los analizados (−12), con lenguaje explícito: "comparecencia surrealista", "esperpéntica", "trumpismo". Los 18 artículos desfavorables contrastan con solo 6 favorables — ratio desf/fav de 3× en contra de Florentino. Por contraste, Riquelme recibe 25 favorables y solo 2 desfavorables (por los desmentidos de Haaland y Klopp). La amplificación de la campaña de Riquelme (autobuses Champions: "pura dinamita") es llamativa dado que Sport es históricamente un medio barcelonés pro-Barça con motivos históricos para no ser favorable a Florentino. Esto hace difícil distinguir H_A de H_B en este caso: el sesgo podría ser convergente-estructural más que coordinado.

---

### Onda Cero
- **Artículos analizados:** 17 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~7 arts. · Florentino ~4 arts. · Comparativas/institucionales ~6
- **Florentino Pérez**
  - Favorables: 3 · Neutrales: ~6 (compartidos) · Desfavorables: 3
  - **Tono neto: 0**
- **Enrique Riquelme**
  - Favorables: 7 · Neutrales: ~6 (compartidos) · Desfavorables: 3
  - **Tono neto: +4**
- **Visibilidad:** Riquelme 7 arts. · Florentino 4 arts. · **Ratio: 1,75×**
- **Marco narrativo:** Fuerte polarización entre "blindaje institucional" (Florentino: garante de que el club no caiga en manos de inversores externos) vs. "urgencia democrática" (Riquelme: 20 años sin elecciones reales, riesgo de privatización opaca). Las críticas a Florentino provienen de artículos editoriales propios; los ataques a Riquelme provienen de entrevistas a Florentino reproducidas fielmente.
- **Notas:** ⚠️ Muestra pequeña (17 arts.). Onda Cero es el **tercer medio con tono neto 0 para Florentino** (junto a ABC y RTVE), lo que lo sitúa en el bloque de radio/TV relativamente equilibrado. Sin embargo, el tono neto hacia Riquelme es más positivo (+4), con los 7 artículos favorables siendo todos de producción propia. Los 3 desfavorables a Florentino son editoriales propios (columna de opinión, análisis de "dos años en blanco", acusación de venta del club), mientras que los 3 desfavorables a Riquelme reproducen declaraciones de Florentino. Esta asimetría de origen es metodológicamente relevante: ¿es lo mismo que el propio medio escriba una crítica a que reproduzca una acusación del rival?

---

### OneFootball
- **Artículos analizados:** 22 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~14 arts. · Florentino ~4 arts. · Institucionales/comparativos ~4
- **Florentino Pérez**
  - Favorables: 2 · Neutrales: 6 · Desfavorables: 3
  - **Tono neto: −1**
- **Enrique Riquelme**
  - Favorables: 7 · Neutrales: 6 · Desfavorables: 4
  - **Tono neto: +3**
- **Visibilidad:** Riquelme 14 arts. · Florentino 4 arts. · **Ratio: 3,5×**
- **Marco narrativo:** Confrontación altamente polarizada. Desgaste institucional del oficialismo frente a la irrupción ilusionante de un candidato nuevo. Los 4 desfavorables a Riquelme provienen de ataques del propio equipo de Florentino (acusaciones de buscar "marca personal", desmentido del censo) y de la expulsión de Valdebebas.
- **Notas:** ⚠️ Muestra muy pequeña (22 arts.) — conclusiones poco fiables. Es el medio más equilibrado en tono de los analizados hasta ahora: −1 para Florentino vs. +3 para Riquelme. La asimetría de visibilidad (3,5×) es alta pero común al patrón general. Los 4 desfavorables a Riquelme incluyen el episodio de Valdebebas (expulsión de las instalaciones) y los desmentidos del censo — hechos concretos, no valoraciones editoriales. OneFootball es una plataforma de noticias de fútbol agregada con contenido mayoritariamente generado por usuarios y redactores externos, lo que puede explicar la menor coherencia editorial.

---

### Mundo Deportivo
- **Artículos analizados:** ~88
- **Presencia por candidato:** Riquelme ~45 arts. · Florentino ~28 arts. · Institucionales/compartidos ~15
- **Florentino Pérez**
  - Favorables: ~14 · Neutrales: ~25 (compartidos) · Desfavorables: ~11
  - **Tono neto: +3** (ligeramente positivo)
- **Enrique Riquelme**
  - Favorables: ~32 · Neutrales: ~25 (compartidos) · Desfavorables: ~6
  - **Tono neto: +26**
- **Visibilidad:** Riquelme ~45 arts. · Florentino ~28 arts. · **Ratio: 1,6×**
- **Marco narrativo:** Confrontación entre regeneración democrática y autoritarismo. Las elecciones como batalla para salvar el club de la privatización corporativa. Crisis institucional y deportiva como marco que justifica el cambio urgente. Florentino = tentáculos de poder, estatutos antidemocráticos, deuda disparada. Riquelme = emprendedor valiente, ilusionante, "Rey del Sol".
- **Notas:** Dato llamativo: **tono neto +3 para Florentino**, lo que lo convierte en uno de los pocos medios donde Florentino tiene saldo ligeramente positivo. Esto contrasta con el tono muy pro-Riquelme (+26) y con Sport (−12), su medio hermano barcelonés. Mundo Deportivo cubre los éxitos históricos de Florentino con reconocimiento genuino (7 Champions, Bernabéu, Mbappé), pero simultáneamente amplifica con dureza las acusaciones de privatización y autoritarismo. Los 11 desfavorables a Florentino incluyen encuadres fuertes: "tentáculos", parodias televisivas, caída económica "sin precedentes". Los 6 desfavorables a Riquelme son todos factuales (banca rechazó aval, Manchester City amenaza legal, agente de Klopp desmiente, plagio de la Ciudad del Socio). En conjunto: Mundo Deportivo reconoce el legado histórico pero lo enmarca en una narrativa de "pasado glorioso / presente en crisis", abriendo la puerta al cambio sin necesidad de anular los méritos anteriores.

---

### Libertad Digital
- **Artículos analizados:** 32 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~17 arts. · Florentino ~10 arts. · Institucionales/logística ~5
- **Florentino Pérez**
  - Favorables: 9 · Neutrales: 13 · Desfavorables: 0
  - **Tono neto: +9**
- **Enrique Riquelme**
  - Favorables: 4 · Neutrales: 13 · Desfavorables: 6
  - **Tono neto: −2**
- **Visibilidad:** Riquelme 17 arts. · Florentino 10 arts. · **Ratio: 1,7×† (ver nota)**
- **Marco narrativo:** Confrontación y defensa de la gestión histórica frente a un candidato desestabilizador. Florentino = mejor presidente de la historia, garante de la soberanía del club. Riquelme = sospechoso, rodeado de vinculaciones oscuras (Villarejo, corrupción), desacreditado por la banca y los desmentidos de Haaland.
- **Notas:** ✅ **Tercer medio pro-Florentino** (junto a OkDiario +29 y El Español +14). Patrón espejo del pro-Riquelme: 0 desfavorables a Florentino, 6 desfavorables a Riquelme. El encuadre de Riquelme incluye el vínculo con el comisario Villarejo y casos de corrupción — acusación grave no documentada en el preregistro como episodio verificable; requiere comprobación antes de incluirla como dato del estudio. **†Ratio visibilidad inflado:** la mayor presencia de Riquelme no refleja cobertura favorable sino seguimiento de sus polémicas y desmentidos. Es un caso claro donde visibilidad ≠ cobertura positiva — refuerza la necesidad de medir tono y visibilidad por separado (como establece el preregistro).

---

### LaSexta
- **Artículos analizados:** 11 ⚠️ muestra muy pequeña
- **Presencia por candidato:** Florentino ~6 arts. · Riquelme ~3 arts. · Institucionales/compartidos ~2
- **Florentino Pérez**
  - Favorables: 7 · Neutrales: 3 · Desfavorables: 0
  - **Tono neto: +7**
- **Enrique Riquelme**
  - Favorables: 1 · Neutrales: 3 · Desfavorables: 2
  - **Tono neto: −1**
- **Visibilidad:** Florentino ~6 arts. · Riquelme ~3 arts. · **Ratio R/F: 0,5×** (Florentino domina)
- **Marco narrativo:** Gestión histórica amenazada por una candidatura desestabilizadora. Florentino = guardián natural de la estabilidad, respaldado por los mitos del club. Riquelme = trámite administrativo o foco de hostilidad y faroles.
- **Notas:** ⚠️ Muestra muy pequeña (11 arts.) — conclusiones muy tentativas. **Resultado contraintuitivo**: LaSexta es conocida por su línea editorial progresista/izquierda, lo que haría esperar simpatía hacia el candidato "disruptor" y escepticismo hacia el "establishment". Sin embargo, es el **cuarto medio pro-Florentino** del corpus y el único de perfil ideológico claramente no conservador entre los que favorecen a Florentino. Posibles explicaciones: (1) la relación del grupo Atresmedia con el mundo del fútbol puede generar dinámicas distintas a las políticas; (2) con solo 11 artículos, el azar muestral puede distorsionar el resultado; (3) los 2 desfavorables a Riquelme reproducen ataques de Florentino (ver regla V1-R1), lo que podría reclasificar alguno como neutro en la codificación formal. Este caso merece revisión especial en la validación.

---

### La Razón
- **Artículos analizados:** 24 ⚠️ muestra pequeña
- **Presencia por candidato:** Florentino ~20 arts. · Riquelme ~1 art. · Institucionales ~3
- **Florentino Pérez**
  - Favorables: 20 · Neutrales: 4 · Desfavorables: 0
  - **Tono neto: +20**
- **Enrique Riquelme**
  - Favorables: 0 · Neutrales: 4 · Desfavorables: 5
  - **Tono neto: −5**
- **Visibilidad:** Florentino ~20 arts. · Riquelme ~1 art. · **Ratio R/F: 0,05×†** (cuasi-silencio de Riquelme)
- **Marco narrativo:** Gestión histórica y mesiánica del oficialismo. Florentino = único salvavidas del club. Riquelme = intereses bastardos, enemigos del Real Madrid, "historia más siniestra", "asamblea de la vergüenza". Lenguaje sin contrapeso ni neutralidad.
- **Notas:** ✅ **El medio más sesgado del corpus en dirección pro-Florentino**, superando a OkDiario (+29) en términos de asimetría: 20 favorables a F, 0 a R; 0 desfavorables a F, 5 a R. El ratio de visibilidad (0,05×) es el más extremo registrado — Riquelme prácticamente no existe como candidato, solo como amenaza. El lenguaje es abiertamente catastrofista para el rival: "demagogias populistas", "intereses bastardos", "enemigos del Real Madrid". A diferencia de OkDiario (que también cubre los eventos de Riquelme, aunque con encuadre crítico), La Razón directamente ignora su campaña. **†Ratio**: el único artículo sobre Riquelme es su entrega de avales — hecho institucional inevitable, no cobertura voluntaria de su campaña. Coincide con la línea editorial conservadora/madridista histórica del medio.

---

### Expansión
- **Artículos analizados:** 33 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~19 arts. · Florentino ~6 arts. · Equilibrados/institucionales ~8
- **Florentino Pérez**
  - Favorables: 9 · Neutrales: ~8 · Desfavorables: 7
  - **Tono neto: +2**
- **Enrique Riquelme**
  - Favorables: 18 · Neutrales: ~8 · Desfavorables: 3
  - **Tono neto: +15**
- **Visibilidad:** Riquelme ~19 arts. · Florentino ~6 arts. · **Ratio: 3,2×**
- **Marco narrativo:** Confrontación empresarial pura. El Real Madrid como empresa multinacional: ACS (Florentino) vs. Cox (Riquelme). La privatización debatida como decisión estratégica corporativa, no como traición al madridismo. Los fichajes analizados como operaciones financieras con retorno de inversión. Marco típico de prensa económica.
- **Notas:** El único medio del corpus que aborda el debate de privatización desde una perspectiva financiera neutral, sin carga emocional de "traición al socio". Sin embargo, el tono hacia Riquelme es claramente más positivo (+15 vs +2). Los 7 desfavorables a Florentino incluyen críticas concretas y verificables (reforma del Bernabéu que empeora comodidades, uso partidista del censo, silencio en caso Negreira) — no son solo amplificaciones de ataques del rival. Los 3 desfavorables a Riquelme sí proceden casi exclusivamente de declaraciones de Florentino (regla V1-R1 aplicable). La cobertura del valor bursátil de Cox ante las noticias electorales es una variable objetiva que ningún otro medio recoge — dato útil para el análisis económico del Módulo 4 de METODOLOGIA.md.

---

### ESdiario
- **Artículos analizados:** 17 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~6 arts. · Florentino ~6 arts. · Institucionales/compartidos ~5
- **Florentino Pérez**
  - Favorables: 7 · Neutrales: 5 · Desfavorables: 2
  - **Tono neto: +5**
- **Enrique Riquelme**
  - Favorables: 6 · Neutrales: 5 · Desfavorables: 4
  - **Tono neto: +2**
- **Visibilidad:** Riquelme ~6 arts. · Florentino ~6 arts. · **Ratio: 1,0×** (equilibrio perfecto)
- **Marco narrativo:** Confrontación institucional equilibrada. Legado histórico y estabilidad (Florentino) vs. transparencia, democratización y promesas ilusionantes (Riquelme). El debate de privatización aparece pero sin la carga catastrofista de otros medios.
- **Notas:** ⚠️ Muestra pequeña (17 arts.). ESdiario presenta el reparto de visibilidad más equilibrado del corpus (1,0×), junto a OkDiario (1,1×). En tono, es ligeramente pro-Florentino (+5 vs +2) pero ambos candidatos reciben cobertura positiva. Los 4 desfavorables a Riquelme incluyen un artículo de opinión propio ("salto al vacío") más tres amplificaciones de ataques de Florentino — por V1-R1, los tres reproducidos deberían reclasificarse como neutros en la codificación formal, lo que dejaría el tono neto R en ~+5, prácticamente igual a F. Caso de mayor equilibrio editorial del corpus junto a ABC.

---

### El Periódico
- **Artículos analizados:** ~40 (1 descartado por irrelevante)
- **Presencia por candidato:** Riquelme ~18 arts. · Florentino ~11 arts. · Compartidos/institucionales ~11
- **Florentino Pérez**
  - Favorables: 2 · Neutrales: ~12 · Desfavorables: ~11
  - **Tono neto: −9**
- **Enrique Riquelme**
  - Favorables: ~13 · Neutrales: ~12 · Desfavorables: 2
  - **Tono neto: +11**
- **Visibilidad:** Riquelme ~18 arts. · Florentino ~11 arts. · **Ratio: 1,6×**
- **Marco narrativo:** Crisis institucional vs. regeneración democrática. Florentino = autoritario, decadente, privatizador. Riquelme = oportunidad democratizadora, voz del socio. Las elecciones como momento histórico de rescate institucional.
- **Notas:** El Periódico es de Barcelona (Grupo Prensa Ibérica), lo que podría contribuir a menor simpatía estructural hacia el presidente del Real Madrid. Los 11 desfavorables a Florentino incluyen lenguaje editorial propio muy marcado: "delirante", "despropósito absoluto", "decadente", "machista" — encuadres fuertes de producción propia, no reproducciones de ataques del rival. Los 2 desfavorables a Riquelme son residuales: una columna de opinión que ridiculiza sus propuestas y una información factual de la Junta Electoral. La cobertura de Florentino es mayoritariamente reactiva/fiscalizadora, no proactiva — el medio no le sigue la agenda, le revisa las polémicas.

---

### El HuffPost
- **Artículos analizados:** 13 ⚠️ muestra pequeña
- **Presencia por candidato:** Riquelme ~8 arts. · Florentino ~3 arts. · Compartidos ~2
- **Florentino Pérez**
  - Favorables: 0 · Neutrales: 6 · Desfavorables: 7
  - **Tono neto: −7**
- **Enrique Riquelme**
  - Favorables: 9 · Neutrales: 1 · Desfavorables: 0
  - **Tono neto: +9**
- **Visibilidad:** Riquelme ~8 arts. · Florentino ~3 arts. · **Ratio: 2,7×**
- **Marco narrativo:** Confrontación entre régimen desgastado y candidatura democratizadora. Florentino = "trumpista", machista, privatizador, autoritario. Riquelme = salvador, valiente, ilusionante, devuelve la voz al socio.
- **Notas:** ⚠️ Muestra pequeña (13 arts.). El HuffPost presenta el patrón más extremo del bloque pro-Riquelme: **0 favorables a Florentino, 0 desfavorables a Riquelme**. Es el espejo exacto de La Razón (0 favorables a Riquelme, 0 desfavorables a Florentino) pero en dirección opuesta. Los 7 desfavorables a Florentino incluyen lenguaje editorial propio muy marcado ("estilo trumpista", "comentarios machistas", "menosprecia con acento mexicano") — todos de producción propia, no reproducciones del rival. Coherente con la línea editorial progresista del medio.

---

### El Desmarque
- **Artículos analizados:** 58
- **Presencia por candidato:** Riquelme ~31 arts. · Florentino ~18 arts. · Mixtos/contextuales ~9
- **Florentino Pérez**
  - Favorables: 16 · Neutrales: 9 · Desfavorables: 5
  - **Tono neto: +11**
- **Enrique Riquelme**
  - Favorables: 24 · Neutrales: 9 · Desfavorables: 4
  - **Tono neto: +20**
- **Visibilidad:** Riquelme ~31 arts. · Florentino ~18 arts. · **Ratio: 1,7×**
- **Marco narrativo:** Confrontación total entre modelos. Candidatura ilusionante y disruptiva (Riquelme) vs. gestión histórica defensiva (Florentino). Cobertura densa de cruces de declaraciones, retos, "artimañas" y contraofensivas.
- **Notas:** El Desmarque es uno de los medios más equilibrados dentro del bloque pro-Riquelme: da 16 favorables a Florentino (el mayor número del corpus después de Marca ~40 e Infobae ~20) y solo 4 desfavorables a Riquelme — con críticas concretas y factuales (desmentido Haaland, correcciones de la Junta, análisis de fiabilidad). El tono neto de +11 para Florentino es el segundo más alto en medios que aun así favorecen a Riquelme. Esto lo sitúa junto a Infobae y Mundo Deportivo como medios pro-Riquelme que reconocen genuinamente el legado de Florentino, en contraste con los que lo ignoran o atacan sistemáticamente. Coherente con un medio deportivo digital sin carga política explícita.

---

### El Debate
- **Artículos analizados:** 44
- **Presencia por candidato:** Florentino ~16 arts. · Riquelme ~14 arts. · Generales/logística ~14
- **Florentino Pérez**
  - Favorables: 16 · Neutrales: 28 · Desfavorables: 0
  - **Tono neto: +16**
- **Enrique Riquelme**
  - Favorables: 2 · Neutrales: 35 · Desfavorables: 7
  - **Tono neto: −5**
- **Visibilidad:** Florentino ~16 arts. · Riquelme ~14 arts. · **Ratio R/F: 0,9×** (casi equilibrado, leve ventaja Florentino)
- **Marco narrativo:** Gestión histórica que blinda el patrimonio del club vs. desestabilización externa con sospecha de intereses ocultos. Florentino = salvador, defensor. Riquelme = inexperiente, sospechoso, instrumento de terceros.
- **Notas:** ✅ **Quinto medio pro-Florentino** del corpus, con el segundo tono neto más alto para Florentino (La Razón +20, El Debate +16). Patrón clásico del bloque pro-Florentino: 0 desfavorables a Florentino, 7 desfavorables a Riquelme. Pero con una particularidad: es el único medio pro-Florentino donde la visibilidad está casi equilibrada (0,9×) — otros como La Razón (0,05×) o El Español (0,57×) silenciaban a Riquelme además de encuadrarlo negativamente. El Debate le da espacio pero lo encuadra con sospecha. Los 7 desfavorables a Riquelme incluyen reproducciones de ataques de Florentino (sujetos a V1-R1) y datos factuales (rechazo bancario, comunicado de la Junta), pero también opiniones de terceros como Mijatovic — esto último sí cuenta como encuadre editorial propio.

---

### El Correo †
- **Artículos analizados:** 14 ⚠️ muestra muy pequeña
- **†Nota de alcance:** El Correo es el diario regional del País Vasco (Grupo Vocento). Se incluye como dato informativo pero no se pondera igual que los nacionales en el análisis agregado.
- **Presencia por candidato:** Riquelme ~7 arts. · Florentino ~1 art. · Compartidos/neutrales ~6
- **Florentino Pérez**
  - Favorables: 2 · Neutrales: 6 · Desfavorables: 3
  - **Tono neto: −1**
- **Enrique Riquelme**
  - Favorables: 5 · Neutrales: 6 · Desfavorables: 0
  - **Tono neto: +5**
- **Visibilidad:** Riquelme ~7 arts. · Florentino ~1 art. · **Ratio: 7×** (ratio distorsionado por muestra mínima)
- **Marco narrativo:** Confrontación entre continuismo histórico (Florentino) y candidatura ilusionante/regeneradora (Riquelme). La privatización como eje de las críticas al presidente. Tono más moderado que otros medios pro-Riquelme.
- **Notas:** ⚠️ Muestra muy pequeña (14 arts.) y alcance regional. Los 3 desfavorables a Florentino son concretos y verificables (rueda de prensa "insólita", Bernabéu sin licencias, privatización). Los 0 desfavorables a Riquelme siguen el patrón de los medios más inclinados hacia él. El ratio 7× está completamente distorsionado: solo 1 artículo centrado en Florentino en todo el periodo. Con estas limitaciones el dato es orientativo, no conclusivo.

---

### Defensa Central
- **Artículos analizados:** 51
- **Presencia por candidato:** Florentino ~31 arts. · Riquelme ~20 arts.
- **Florentino Pérez**
  - Favorables: ~34 · Neutrales: ~11 · Desfavorables: 0
  - **Tono neto: +34** — el más alto del corpus
- **Enrique Riquelme**
  - Favorables: ~4 · Neutrales: ~11 · Desfavorables: ~18
  - **Tono neto: −14** — el más negativo del corpus
- **Visibilidad:** Florentino ~31 arts. · Riquelme ~20 arts. · **Ratio R/F: 0,65×**
- **Marco narrativo:** Gestión histórica indiscutible (Florentino supera a Santiago Bernabéu como mejor presidente) vs. oposición inexperta y oportunista vinculada a las épocas más oscuras del club. Riquelme retratado como un desestabilizador sin credibilidad.
- **Notas:** ✅ **El medio más sesgado del corpus en dirección pro-Florentino**, con el tono neto más alto para Florentino (+34) y el más negativo para Riquelme (−14) de todos los analizados. Sin embargo, este resultado es **metodológicamente esperado y no sorprendente**: Defensa Central es un medio de afición madridista, no un periódico de información general. Su función editorial es defender los intereses del Real Madrid, no informar con neutralidad. Su inclusión en el análisis principal debe ir acompañada de esta advertencia — es el equivalente al "fan media" y no puede compararse directamente con prensa generalista o deportiva profesional. Los 18 desfavorables a Riquelme incluyen desde desmentidos factuales (Haaland, Klopp) hasta críticas por ir a los toros en lugar de apoyar al filial — un nivel de escrutinio que no se aplica a Florentino en ningún artículo del medio.

---

### COPE
- **Artículos analizados:** 81
- **Presencia por candidato:** Riquelme ~42 arts. · Florentino ~27 arts. · Compartidos/institucionales ~12
- **Florentino Pérez**
  - Favorables: 12 · Neutrales: 18 · Desfavorables: 14
  - **Tono neto: −2**
- **Enrique Riquelme**
  - Favorables: 34 · Neutrales: 18 · Desfavorables: 3
  - **Tono neto: +31**
- **Visibilidad:** Riquelme ~42 arts. · Florentino ~27 arts. · **Ratio: 1,6×**
- **Marco narrativo:** Confrontación institucional enmarcada como referéndum sobre el modelo de club. Elecciones = plebiscito sobre privatización vs. socios. Sistema electoral de Florentino = "emboscada" y trampa de 187 millones. Riquelme = candidatura ilusionante y renovadora.
- **Notas:** ⚠️ **Resultado contraintuitivo de alto interés.** COPE es la radio de la Conferencia Episcopal, históricamente asociada a la derecha conservadora española, el mismo espectro ideológico que OkDiario (+29 F), La Razón (+20 F) o Libertad Digital (+9 F). Sin embargo, COPE aparece con **tono neto −2 para Florentino y +31 para Riquelme** — el segundo tono pro-Riquelme más alto del corpus tras Marca (+55). Esto rompe completamente el patrón ideológico del bloque pro-Florentino. Posibles explicaciones: (1) COPE tiene una sección deportiva (El Partidazo, Tiempo de Juego) con línea editorial independiente de la línea política general; (2) el deporte en COPE tiende a dar voz al "retador" para generar debate y audiencia; (3) los 14 desfavorables a Florentino incluyen crítica a la "emboscada electoral" — un marco narrativo posiblemente adoptado por periodistas deportivos sin filtro ideológico del medio. Este caso es relevante para H_A vs. H_B: si hubiera coordinación pro-Riquelme, COPE sería el candidato más improbable para participar en ella dado su perfil ideológico. Su inclinación apunta más a H_B (convergencia independiente de incentivos periodísticos deportivos).

---

### Cadena SER
- **Artículos analizados:** 82
- **Presencia por candidato:** Riquelme ~45 arts. · Florentino ~27 arts. · Generales/institucionales ~10
- **Florentino Pérez**
  - Favorables: 16 · Neutrales: 5 · Desfavorables: 17
  - **Tono neto: −1**
- **Enrique Riquelme**
  - Favorables: 38 · Neutrales: 5 · Desfavorables: 6
  - **Tono neto: +32**
- **Visibilidad:** Riquelme ~45 arts. · Florentino ~27 arts. · **Ratio: 1,7×**
- **Marco narrativo:** Candidatura ilusionante y rupturista vs. gestión histórica desgastada por crisis institucional y deportiva. Riquelme = respiro democrático, devuelve el poder al socio. Florentino = enormes logros pasados pero descontento creciente, opacidad y posible privatización.
- **Notas:** ⚠️ **Convergencia inesperada con COPE.** La Cadena SER (Grupo PRISA, línea editorial de centro-izquierda) y COPE (línea conservadora-católica) son rivales históricos en radio. Sin embargo producen coberturas casi idénticas: SER −1/+32 · COPE −2/+31. Esta convergencia entre medios ideológicamente opuestos es **el argumento más fuerte del corpus para H_B** (convergencia de incentivos independientes): dos emisoras que nunca coordinan en política adoptaron el mismo encuadre deportivo. La explicación más parsimoniosa es que ambas siguen la misma lógica periodística deportiva — el retador genera más noticias y más audiencia que el favorito defensivo, independientemente de la línea editorial. Los 17 desfavorables a Florentino incluyen crítica a la "esperpéntica" rueda de prensa (lenguaje editorial propio, no solo reproducción del rival).

---

### Antena 3
- **Artículos analizados:** 48
- **Presencia por candidato:** Riquelme ~27 arts. · Florentino ~13 arts. · Mixtos/institucionales ~8
- **Florentino Pérez**
  - Favorables: 8 · Neutrales: 7 · Desfavorables: 6
  - **Tono neto: +2**
- **Enrique Riquelme**
  - Favorables: 22 · Neutrales: 7 · Desfavorables: 5
  - **Tono neto: +17**
- **Visibilidad:** Riquelme ~27 arts. · Florentino ~13 arts. · **Ratio: 2,1×†**
- **Marco narrativo:** Candidatura ilusionante/renovadora vs. gestión histórica amenazada. Riquelme = salvación frente a la privatización. Florentino = defensivo, protegiendo legado.
- **Notas:** †El ratio de visibilidad 2,1× tiene una explicación institucional parcial: Riquelme apareció en **El Hormiguero** (programa de la propia cadena Atresmedia), lo que generó cobertura cruzada autorreferencial. Esto infla la presencia de Riquelme en los artículos digitales de Antena 3 con un incentivo que no es estrictamente editorial. Para el análisis de sesgo hay que descontar los artículos que simplemente cubren la aparición en El Hormiguero. El tono (+2 F / +17 R) es pro-Riquelme moderado, con ambos candidatos recibiendo tono positivo neto — patrón similar a El Desmarque y Expansión. Los 6 desfavorables a Florentino incluyen el error de IA con Mourinho (hecho verificable y concreto) y ataques de Calderón (voz externa, sujeto a V1-R1). Los 5 desfavorables a Riquelme son todos factuales (rechazo bancario, Junta Electoral).

---

### 20Minutos
- **Artículos analizados:** 62
- **Presencia por candidato:** Riquelme ~36 arts. · Florentino ~13 arts. · Generales/procedimentales ~13
- **Florentino Pérez**
  - Favorables: 11 · Neutrales: 13 · Desfavorables: 10
  - **Tono neto: +1**
- **Enrique Riquelme**
  - Favorables: 19 · Neutrales: 13 · Desfavorables: 9
  - **Tono neto: +10**
- **Visibilidad:** Riquelme ~36 arts. · Florentino ~13 arts. · **Ratio: 2,8×**
- **Marco narrativo:** Confrontación entre dos miedos simétricos: privatización del club (argumento de Riquelme) vs. caída en manos de "aventureros sin escrúpulos" (argumento de Florentino). Gestión histórica vs. disrupción ilusionante.
- **Notas:** 20Minutos es uno de los medios más equilibrados en cobertura crítica: 10 desfavorables a Florentino y 9 a Riquelme — casi paridad de escrutinio. En tono neto es moderadamente pro-Riquelme (+10 vs +1), pero ambos candidatos reciben tanto cobertura favorable como crítica. El detalle de que cubren también la "vida personal y sentimental" de Riquelme (no mencionado en ningún otro medio) es un indicador de que el retador generó interés humano más allá de lo político-deportivo. Un medio gratuito y de amplia difusión, lo que le da peso de audiencia aunque menor presencia en el debate de élite.

---

*Pendientes: AS, Telecinco, Economía Digital, Demócrata, Superdeporte, Tribuna.com, El Periódico de España, DAZN, beIN SPORTS, El Independiente, Telemadrid, Goal.com, MARCA Usa, infoLibre*
