# Análisis intermedio de cobertura mediática
## Elecciones presidencia Real Madrid 2026 — Florentino Pérez vs. Enrique Riquelme

> **Estado:** análisis de fase preliminar sobre 34 medios y ~1.565 artículos codificados
> manualmente con NotebookLM (una pasada por medio, sin cegado formal).
> **Advertencia metodológica:** estos datos son orientativos. La codificación formal
> (multi-pasada con cegado, α de Krippendorff ≥ 0,80) está pendiente. Las conclusiones
> que siguen son hipótesis de trabajo, no veredictos.

---

## 1. Base de datos analizada

| Estadístico | Valor |
|---|---|
| Medios analizados | 34 |
| Artículos analizados | ~1.565 |
| Periodo cubierto | 12-may-2026 → 8-jun-2026 |
| Método de codificación | NotebookLM (una pasada por medio, sin cegado) |
| Escala de tono | −n (desfavorable) → 0 (neutro) → +n (favorable) |

### Tabla de datos completos

| Medio | N | Tono F | Tono R | Diferencial R−F | Ratio vis. R/F |
|-------|--:|:------:|:------:|:---------------:|:--------------:|
| Sport | 78 | −12 | +23 | **+35** | 1,6× |
| COPE | 81 | −2 | +31 | **+33** | 1,6× |
| Cadena SER | 82 | −1 | +32 | **+33** | 1,7× |
| El Confidencial | 51 | −5 | +25 | **+30** | 2,1× |
| La Vanguardia | 51 | −7 | +18 | **+25** | 1,2× |
| El Mundo | 62 | −2 | +21 | **+23** | 2,9× |
| Mundo Deportivo | 88 | +3 | +26 | **+23** | 1,6× |
| Marca | 138 | +32 | +55 | **+23** | 3,8× |
| El Periódico | ~40 | −9 | +11 | **+20** | 1,6× |
| Europa Press | 20 | −7 | +10 | **+17** | 13× ⚠️ |
| El HuffPost | 13 | −7 | +9 | **+16** | 2,7× |
| Infobae | 87 | +13 | +29 | **+16** | 1,4× |
| Antena 3 | 48 | +2 | +17 | **+15** | 2,1×† |
| Expansión | 33 | +2 | +15 | **+13** | 3,2× |
| The Objective | 24 | −5 | +8 | **+13** | 15× ⚠️ |
| Vozpopuli | 20 | −1 | +10 | **+11** | 0,78× |
| elDiario.es | 9 | −4 | +6 | **+10** | 4,0× |
| El Desmarque | 58 | +11 | +20 | **+9** | 1,7× |
| 20Minutos | 62 | +1 | +10 | **+9** | 2,8× |
| RTVE.es | 23 | 0 | +6 | +6 | 1,4× |
| El Correo † | 14 | −1 | +5 | +6 | 7× ⚠️ |
| OneFootball | 22 | −1 | +3 | +4 | 3,5× |
| Onda Cero | 17 | 0 | +4 | +4 | 1,8× |
| Heraldo.es | 23 | +3 | +6 | +3 | 1,4× |
| ESPN Deportes | 21 | +2 | +4 | +2 | 2,2× |
| ABC | 96 | 0 | −1 | −1 | 2,6× |
| ESdiario | 17 | +5 | +2 | −3 | 1,0× |
| LaSexta | 11 | +7 | −1 | −8 | 0,5× |
| Libertad Digital | 32 | +9 | −2 | −11 | 1,7×† |
| El Español | 28 | +14 | −2 | −16 | 0,57× |
| OkDiario | 97 | +29 | +9 | −20 | 1,1× |
| El Debate | 44 | +16 | −5 | −21 | 0,9× |
| La Razón | 24 | +20 | −5 | −25 | 0,05×† |
| Defensa Central ‡ | 51 | +34 | −14 | −48 | 0,65× |

> † Ratio afectado por factor externo (ver fichas). ‡ Fan media; se excluye de las medias ponderadas principales.
> † El Correo: diario regional (País Vasco); se incluye como dato informativo.

---

## 2. Estadísticos agregados

### 2.1 Tono neto ponderado (por N artículos)

| Conjunto | N total | Tono neto F (media pond.) | Tono neto R (media pond.) | Gap R−F |
|---|---:|:---:|:---:|:---:|
| **Todos los medios** | ~1.565 | **+6,8** | **+17,5** | **+10,7** |
| **Sin Defensa Central** | ~1.514 | **+5,9** | **+18,5** | **+12,6** |
| **Solo nacionales (sin Correo)** | ~1.551 | **+6,7** | **+17,5** | **+10,8** |

**Interpretación:** En el conjunto del corpus, Florentino Pérez recibe un tono medio ligeramente positivo (+6,8), pero Riquelme recibe un tono significativamente más favorable (+17,5). La brecha es de ~11 puntos en toda la escala — sustancial y consistente.

### 2.2 Distribución por bloque editorial

Criterio: diferencial R−F ≥ +8 = pro-Riquelme; ≤ −8 = pro-Florentino; entre −7 y +7 = neutro/equilibrado.

| Bloque | N medios | % corpus | Artículos cubiertos |
|---|:-:|:-:|---:|
| **Pro-Riquelme** (diff ≥ +8) | **19** | 56% | ~940 |
| **Equilibrado** (−7 ≤ diff ≤ +7) | **8** | 24% | ~299 |
| **Pro-Florentino** (diff ≤ −8) | **7** | 21% | ~327 |

> Si se excluye Defensa Central (fan media): 6 medios pro-Florentino, ~276 artículos.

### 2.3 Visibilidad global (artículos donde el candidato es sujeto principal)

| Candidato | Artículos totales como protagonista | % del total con sujeto identificado |
|---|---:|---:|
| Enrique Riquelme | ~742 | **63%** |
| Florentino Pérez | ~444 | **37%** |
| **Ratio global R/F** | — | **1,67×** |

Riquelme domina como protagonista en **27 de 34 medios**. Los 7 en que Florentino iguala o supera: La Razón, El Debate, Defensa Central, El Español, LaSexta, Vozpopuli, ESdiario.

---

## 3. Análisis de tono

### 3.1 Distribución de artículos desfavorables

Un indicador especialmente revelador es la **asimetría en artículos con tono neto 0 para uno de los candidatos**:

**Medios con 0 desfavorables a Florentino:**
La Razón, El Debate, El Español, Libertad Digital, LaSexta, Defensa Central (6 medios, todos pro-Florentino).

**Medios con 0 desfavorables a Riquelme:**
El Confidencial, elDiario.es, El HuffPost, La Razón (0 favorables), Defensa Central (0 favorables).

Esta estructura "suelo en cero" es característica de cobertura con agenda: un medio con sesgo raramente critica al candidato favorecido.

### 3.2 Casos extremos por dimensión

| Métrica | Valor extremo pro-Riquelme | Valor extremo pro-Florentino |
|---|---|---|
| Mayor diferencial | Sport +35 | Defensa Central −48 |
| Tono neto R más alto | Marca +55 | — |
| Tono neto F más alto | — | Defensa Central +34 / OkDiario +29 |
| Tono neto F más bajo | Sport −12 | — |
| Mayor silencio del rival | Europa Press (1 art. F) | La Razón (1 art. R) |

### 3.3 Marco narrativo compartido

El **marco de "privatización"** aparece en ≥15 de 34 medios de ideologías muy distintas (COPE, SER, Sport, El Confidencial, La Vanguardia, Expansión, 20Minutos, etc.). Su origen es la propia campaña de Riquelme — él lo acuñó y los medios lo adoptaron. Que aparezca en COPE (conservadora) y elDiario.es (izquierda) simultáneamente indica que el frame viajó desde el candidato hacia los medios, no de unos medios a otros.

---

## 4. Patrones transversales

### 4.1 La dinámica del retador

En **29 de 34 medios**, Riquelme tiene más artículos como protagonista que Florentino. La explicación más parsimoniosamente estructural: el candidato desafiante necesita presentar su proyecto, lo que genera una cascada de noticias diarias (avales, fichajes, sede, programa) mientras el incumbente puede permanecer más institucional. Esta dinámica opera **independientemente de la ideología del medio** y es el mecanismo base de H_B.

Evidencia: el ratio de visibilidad promedio (1,67×) es prácticamente idéntico en medios de muy distinto signo — COPE 1,6×, SER 1,7×, Mundo Deportivo 1,6×, El Periódico 1,6×.

### 4.2 Convergencia COPE/SER

La Cadena SER (centro-izquierda, Grupo PRISA) y COPE (conservadora, Conferencia Episcopal) son rivales históricos en política. Sus coberturas de estas elecciones son **casi idénticas**:

| Emisora | Tono F | Tono R | Diferencial | Ratio vis. |
|---|:-:|:-:|:-:|:-:|
| COPE | −2 | +31 | +33 | 1,6× |
| Cadena SER | −1 | +32 | +33 | 1,7× |

La probabilidad de coordinación entre estas dos emisoras es prácticamente nula. Su convergencia es el argumento empírico más fuerte del corpus para **H_B** (convergencia de incentivos periodísticos independientes).

### 4.3 El bloque pro-Florentino: patrón ideológico

| Medio | Diferencial R−F | Perfil ideológico |
|---|:-:|---|
| Defensa Central | −48 | Fan media madridista |
| La Razón | −25 | Conservadora-católica |
| El Debate | −21 | Conservadora |
| OkDiario | −20 | Derecha digital |
| El Español | −16 | Centro-derecha |
| Libertad Digital | −11 | Derecha liberal |
| LaSexta | −8 | Progresista ⚠️ |

5 de 6 medios periodísticos pro-Florentino son de derechas. La excepción es LaSexta (muestra muy pequeña: 11 artículos), que podría ser ruido muestral. Este bloque tiene coherencia ideológica clara, lo que lo hace compatible tanto con H_A (coordinación entre medios afines) como con H_B (afinidad estructural con el madridismo conservador).

### 4.4 El bloque pro-Riquelme: amplitud ideológica

El bloque pro-Riquelme abarca un espectro ideológico que hace improbable la coordinación:

- **Izquierda:** elDiario.es (+10), El HuffPost (+16), El Periódico (+20), Sport (+35)
- **Centro-izquierda:** Cadena SER (+33), El Confidencial (+30), La Vanguardia (+25)
- **Centro:** El Mundo (+23), COPE (+33), Antena 3 (+15), RTVE (+6), Expansión (+13)
- **Derecha-liberal:** Vozpopuli (+11), The Objective (+13)
- **Deportivos/digitales:** Marca (+23), El Desmarque (+9), Mundo Deportivo (+23), Infobae (+16)
- **Internacional:** ESPN (+2), Infobae (+16)

La coexistencia de COPE, SER, elDiario.es y Vozpopuli en el mismo bloque es difícilmente explicable por coordinación editorial.

### 4.5 Sport vs. Mundo Deportivo: mismo tipo, distinta intensidad

Dos diarios deportivos barceloneses, mismo grupo de lectores objetivo, mismo ángulo anti-Real Madrid histórico, pero coberturas muy diferentes en intensidad:

| Medio | Tono F | Diferencial |
|---|:-:|:-:|
| Sport | −12 | +35 |
| Mundo Deportivo | +3 | +23 |

Si hubiera coordinación entre ellos, convergirían. La diferencia de 12 puntos en el tono hacia Florentino sugiere decisiones editoriales independientes, no sincronizadas.

### 4.6 Medios equilibrados como control

8 medios se sitúan en la zona neutral (|diff| ≤ 7):

| Medio | Diferencial | Tipo |
|---|:-:|---|
| ABC | −1 | Prensa general conservadora |
| ESdiario | −3 | Digital conservadora |
| ESPN Deportes | +2 | Internacional deportivo |
| Heraldo.es | +3 | Regional (Aragón) |
| Onda Cero | +4 | Radio privada |
| OneFootball | +4 | Plataforma digital fútbol |
| RTVE.es | +6 | TV pública |
| El Correo† | +6 | Regional (País Vasco) |

La existencia de este bloque neutro, que incluye la televisión pública (RTVE) y una radio privada grande (Onda Cero), es coherente con H_0 parcial — hay medios que no muestran sesgo sistemático. También es consistente con H_B: medios que siguen la dinámica del retador en visibilidad pero mantienen equilibrio en tono.

---

## 5. Implicaciones para las hipótesis del preregistro

### Respecto a H_0 (no hay sesgo sistemático)

**No se puede sostener H_0 en el conjunto del corpus.** El diferencial ponderado de +10,7 puntos, presente en 19 de 34 medios, con 27 medios en los que Riquelme domina la visibilidad, es demasiado consistente para ser ruido. Sin embargo, H_0 **sí se sostiene para el subconjunto de 8 medios equilibrados** (~20% del corpus en artículos). El veredicto es: sesgo agregado claro, pero no universal.

### Respecto a H_A (coordinación entre medios)

**Los datos son inconsistentes con coordinación amplia.** Los argumentos:
1. La convergencia COPE/SER (medios que no coordinan en política) bajo H_A requeriría un mecanismo de coordinación que cruce trincheras ideológicas históricas — muy improbable.
2. La amplitud ideológica del bloque pro-Riquelme (izquierda + derecha + deportivos + internacionales) no tiene estructura de red coordinada evidente.
3. La diferencia de intensidad entre Sport y Mundo Deportivo (dos medios del mismo grupo natural) es inconsistente con coordinación.
4. El vocabulario compartido ("privatización", "ilusionante") aparenta coordinación pero tiene origen en la propia campaña de Riquelme, no en intercambio entre redacciones.

H_A **no puede descartarse para el subconjunto pro-Florentino** (5 medios de derecha con coherencia alta), aunque tampoco puede afirmarse sin evidencia documental (intercambios, líneas editoriales compartidas, instrucciones de grupo).

**H_A para Europa Press:** si la agencia EFE de facto está sesgada (ratio 13×, −7/+10), su impacto se multiplica por todos los medios que republican sus despachos. Esto podría crear apariencia de coordinación bajo H_B. Merece investigación específica.

### Respecto a H_B (convergencia de incentivos independientes)

**H_B es la hipótesis mejor respaldada por los datos actuales.** Los mecanismos identificados:

1. **Dinámica del retador:** el candidato desafiante genera más noticias estructuralmente. Opera en todos los medios sin coordinación.
2. **Frame de privatización:** acuñado por Riquelme y adoptado independientemente por medios de espectros opuestos. Funciona como gancho periodístico sin necesidad de coordinación.
3. **Incentivo de audiencia:** el "showman" (Haaland, Klopp, Hormiguero) genera clics; cubrir sus promesas es racional individualmente aunque resulte favorecedor.
4. **Afinidad estructural:** medios barceloneses (Sport, MD, El Periódico) tienen historia de antagonismo con el Madrid — sesgo pre-existente, no coordinado.
5. **Afinidad ideológica izquierda:** el frame de "privatización + democratización" resuena naturalmente en medios progresistas.

**H_B compatible también con el bloque pro-Florentino:** la afinidad estructural de medios conservadores con el madridismo institucional es una forma de convergencia de incentivos (identitaria + ideológica), no necesariamente coordinación.

---

## 6. Limitaciones del análisis actual

1. **Una sola pasada, sin cegado.** NotebookLM conocía los nombres de los candidatos. El riesgo de sesgo de codificación está presente, especialmente en los rangos intermedios. El α de Krippendorff formal está pendiente.

2. **Granularidad de escala.** La escala usada (conteo de artículos favorable/neutro/desfavorable) no captura la intensidad dentro de cada categoría. Un artículo "levemente favorable" pesa igual que uno "muy favorable".

3. **Medios con muestra pequeña.** 11 medios tienen ≤ 22 artículos. Sus resultados son orientativos. En particular: LaSexta (11 arts., único progresista pro-Florentino) requiere más artículos para conclusión fiable.

4. **Medios pendientes.** Faltan aún: AS, Telecinco, y medios más pequeños (Demócrata, Goal.com, beIN Sports, Superdeporte, etc.). AS es potencialmente importante por volumen.

5. **Regla V1-R1 no aplicada formalmente.** Algunos artículos clasificados como "desfavorables" son reproducciones de ataques del rival (no encuadre editorial propio). La aplicación formal de V1-R1 redistribuiría algunos artículos hacia "neutro", probablemente mejorando ligeramente el tono de Riquelme en medios pro-Florentino y el de Florentino en medios pro-Riquelme.

6. **El Correo y Defensa Central:** incluidos con advertencia. Defensa Central (fan media) altera las medias ponderadas. Se recomienda excluirlo del análisis principal y tratarlo en nota metodológica separada.

---

## 7. Pendientes prioritarios antes del análisis final

| Prioridad | Tarea |
|---|---|
| 🔴 Alta | Analizar AS (potencialmente el segundo medio deportivo en volumen) |
| 🔴 Alta | Verificar si Europa Press está sesgada como agencia (H_A específico) |
| 🟡 Media | Completar Telecinco, 20Minutos ya hecho |
| 🟡 Media | Aplicar V1-R1 formalmente y recalcular tonos ajustados |
| 🟡 Media | Analizar el episodio Haaland/Klopp en V4 (tratamiento de desmentidos por medio) |
| 🟢 Baja | Incorporar medios menores pendientes (Demócrata, Goal.com, beIN, etc.) |

---

## 8. Resumen ejecutivo (para el informe final)

> De los 34 medios y ~1.565 artículos analizados, el corpus muestra un **sesgo
> agregado pro-Riquelme consistente pero no universal**: 19 medios favorecen a
> Riquelme (56%), 8 son equilibrados (24%), y 7 favorecen a Florentino (21%).
> El tono neto ponderado es +6,8 para Florentino y +17,5 para Riquelme (brecha
> de ~11 puntos). La visibilidad de Riquelme supera la de Florentino en 27 de
> 34 medios (ratio global 1,67×).
>
> **H_0** (no hay sesgo) no se sostiene para el conjunto, pero sí para ~8 medios
> que actúan como control (ABC, RTVE, Onda Cero, ESdiario, Heraldo, ESPN).
>
> **H_A** (coordinación) es **poco probable** como explicación general: la
> convergencia COPE/SER y la amplitud ideológica del bloque pro-Riquelme son
> incompatibles con coordinación editorial amplia. No puede descartarse para
> el subconjunto de 5-6 medios conservadores pro-Florentino.
>
> **H_B** (convergencia de incentivos independientes) es la hipótesis **mejor
> respaldada**: la dinámica del retador, el frame de privatización de origen
> en la propia campaña, y los incentivos de audiencia operan de forma
> independiente en medios de espectros ideológicos opuestos. El sesgo, de
> existir, es mayoritariamente **estructural y convergente**, no coordinado.
>
> **Advertencia:** estas conclusiones son preliminares (una pasada, sin cegado
> formal). El análisis definitivo requiere codificación multi-pasada con α ≥ 0,80.

---

*Generado: 2026-06-08. Datos: `data/resultados/tonos_por_medio.md`.*
