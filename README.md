# Gasto Público en España (1980–2025) — Proyecto de datos y vídeo

Comparativa del dinero que el Estado español destina a **educación** (pública y concertada), **sanidad** (pública y privada), **Iglesia católica** e **infraestructuras de transporte**, desde 1980 hasta hoy, ajustada por el tamaño de la economía y la población.

Este repositorio es el **paquete de trabajo completo** para seguir editándolo con Claude Code en local: datos, metodología, fuentes, los tres artefactos visuales (HTML autónomo) y los guiones de vídeo.

---

## 1. Objetivo

Responder, con datos oficiales y de forma honesta, a la pregunta: **¿en qué gasta el dinero el Estado español y cómo ha cambiado en 45 años?** Y hacerlo entendible para cualquier persona mediante visualizaciones interactivas y piezas de vídeo.

## 2. Metodología (la regla de oro)

Comparar euros de 1980 con euros de hoy **engaña**, porque se acumulan tres efectos:

- **Inflación:** los precios se han multiplicado por ~6 (≈520 % acumulado 1980–2025).
- **Población:** de 37,5 a ~48,6 millones de habitantes (+30 %).
- **Riqueza:** la economía es ~17 veces mayor en euros corrientes.

Por eso la medida principal es el **% del PIB** (qué parte de todo lo que produce el país se dedica a cada cosa): neutraliza los tres efectos a la vez. Es la medida que usan OCDE, FMI y Eurostat. Como vista secundaria se ofrecen **euros corrientes**.

> **Fiabilidad:** datos de 2000 en adelante, sólidos (fuentes oficiales). 1995–2000, oficiales con cambios de metodología. **1980–1995, estimaciones** reconstruidas de literatura académica y series del Banco de España (marcadas como tales). Úsense como tendencia, no como contabilidad al céntimo.

## 3. Entregables (archivos de este repo)

| Archivo | Qué es |
|---|---|
| `artefactos/comparador.html` | Dashboard interactivo (6 pestañas) con gráficos, fichas, tablas y metodología. **Es la pieza central.** |
| `artefactos/guiones.html` | Guiones de vídeo navegables (corto, largo YouTube, ficha) con botón de copiar. |
| `artefactos/short.html` | Presentación vertical 9:16 autorreproducible (~65 s) con narración opcional (TTS), para grabar la pantalla. |
| `datos/dataset.md` | Todas las series de datos en tablas, con nivel de confianza. |
| `README.md` | Este documento maestro. |

Los HTML son **autónomos**: ábrelos con doble clic en el navegador. No necesitan servidor ni dependencias (solo fuentes de Google Fonts por internet).

## 4. Resumen de hallazgos

- **Educación pública:** de ~2,4 % del PIB (1980) → techo del 5,0 % (2009) → **4,5 % hoy**, por debajo de la media OCDE. La **concertada** ≈ 12 % del gasto educativo público (~7.500 M€/año).
- **Sanidad pública:** de ~4,2 % → 6,5 % pre-pandemia → **8,0 % en 2020** (COVID) → 7,0 % (2023). Con la privada (2,5 %), el total ronda el 9,5 % del PIB. España es de los países OCDE con **más peso privado** (~26 %).
- **Iglesia:** **429 M€ en 2024** vía casilla del 0,7 % del IRPF (sin dotación directa desde 2007). ≈ 0,03 % del PIB. **No incluye** financiación indirecta (profesores de religión, conciertos de colegios religiosos, capellanías, patrimonio, exenciones fiscales), mayor pero sin cifra oficial consolidada.
- **Infraestructuras de transporte:** cíclicas. 2,1 % del PIB en 2009 (≈24.000 M€) → 0,55 % en 2018 (−72 %) → ~1,0 % en 2025 (≈16.114 M€). Carreteras ≈ 55 % histórico, ~30 % hoy.

## 5. Fuentes principales

- **INE** — Contabilidad Nacional (PIB) y Padrón (población): <https://www.ine.es>
- **Ministerio de Educación, FP y Deportes** — Estadística del gasto público en educación.
- **Ministerio de Sanidad** — Sistema de Cuentas de Salud 2023: <https://www.sanidad.gob.es>
- **OCDE** — *Education at a Glance* y *Health at a Glance*.
- **Conferencia Episcopal Española** (Oficina de Transparencia) y **Agencia Tributaria** — asignación 0,7 % IRPF.
- **Funcas** (Matas & Vassallo) y **Ministerio de Transportes** — inversión en infraestructuras.
- **Banco de España** — series históricas de Contabilidad Nacional (1850–2024).

Enlaces concretos consultados en `datos/dataset.md`.

---

## 6. Guion CORTO · vertical 9:16 (TikTok / Reels / Facebook) · ~58 s

Formato para verse **sin sonido**: el texto en pantalla cuenta la historia; la locución la refuerza. Un corte por bloque. Para 30 s, deja solo Gancho + Iglesia + Cierre.

| Momento | Texto en pantalla | Locución |
|---|---|---|
| 0–3 s · Gancho | ¿A DÓNDE VA EL DINERO DEL ESTADO? | ¿A dónde va de verdad el dinero del Estado español? Mira esto. |
| 3–12 s · Regla | La trampa: 1980 ≠ hoy · Precios ×6 · Población +30 % · Economía ×17 | Comparar euros de hace 45 años es un engaño. Por eso lo medimos en porcentaje del PIB. |
| 12–24 s · Bienestar | SANIDAD 4 % → 8 % (COVID) · EDUCACIÓN ×2 desde 1980 | La sanidad pública pasó del 4 al 8 por ciento del PIB en la pandemia. La educación se ha duplicado… pero seguimos por debajo de Europa. |
| 24–36 s · Ladrillo | OBRA PÚBLICA: pico 2009 → −72 % en 2018 | La inversión en carreteras y trenes tocó techo en 2009 y se hundió un 72 por ciento con la crisis. |
| 36–50 s · Iglesia | IGLESIA: 429 M€ vía IRPF (2024) · …pero el coste real es mayor | ¿Y la Iglesia? 429 millones por la casilla del IRPF en 2024. Aunque su coste real para el Estado es mayor… y nadie lo suma en una sola cifra. |
| 50–58 s · Cierre | Datos oficiales · Gráfico interactivo 👇 · Sígueme para más | Todo con datos oficiales. Tienes el gráfico interactivo para verlo tú mismo. Sígueme para más. |

**Texto de publicación:** ¿Sabes a dónde va de verdad el dinero del Estado? Lo he mirado desde 1980 con datos oficiales. La sanidad, la educación, las carreteras y la Iglesia… hay sorpresas.
**Hashtags:** #España #datos #economía #sanidad #educación #política #divulgación #impuestos

---

## 7. Guion LARGO · YouTube · locución limpia (~7–8 min)

> Solo texto para leer en alto. Los títulos **no se locutan**. Ritmo ~140 palabras/minuto; pausa tras cada cifra.

**Introducción**
Cada año, el Estado español reparte cientos de miles de millones de euros. Pero, ¿a dónde va realmente ese dinero? ¿Gastamos hoy más o menos que hace 45 años en colegios, en hospitales, en carreteras… o en la Iglesia? En este vídeo lo vemos con datos oficiales, desde 1980 hasta hoy. Vamos allá.

**La trampa de los euros**
Antes de empezar, una advertencia que lo cambia todo. Comparar euros de 1980 con euros de hoy es engañoso, por tres motivos que ocurren a la vez. Primero, los precios: se han multiplicado por seis; lo que costaba un euro en 1980 cuesta seis en la actualidad. Segundo, la población: hemos pasado de 37 a casi 49 millones de habitantes. Y tercero, la economía: hoy es diecisiete veces más grande medida en euros. Por eso, para comparar de forma justa, usamos una sola vara de medir: el porcentaje del Producto Interior Bruto. Es decir, de todo lo que produce el país en un año, qué parte dedica a cada cosa. Esa medida neutraliza la inflación, el aumento de la población y el crecimiento de la riqueza, todo a la vez. Es la misma que usan la OCDE, el Fondo Monetario Internacional y Eurostat.

**Visión general**
Con esa vara de medir, esta es la fotografía completa. Tres grandes partidas comparables: sanidad, educación e infraestructuras, todas en porcentaje del PIB. El patrón es claro. La sanidad y la educación suben de forma sostenida a lo largo de las décadas: es la construcción del Estado del bienestar. En cambio, la inversión en infraestructuras dibuja una montaña: crece con la expansión económica y se desploma tras la crisis de 2010. La Iglesia queda fuera de esta imagen por una razón de escala: el dinero directo que recibe es unas 150 veces menor, así que la veremos por separado.

**Educación**
Empecemos por los colegios. En 1980, recién estrenada la democracia, España dedicaba a la educación pública alrededor del 2,4 por ciento del PIB: la mitad que hoy. Con la universalización de la enseñanza, el gasto creció con fuerza durante los años ochenta y noventa, hasta alcanzar su techo histórico en 2009: un 5 por ciento del PIB. Después llegaron los recortes. Hoy estamos en torno al 4,5 por ciento, todavía por debajo de la media de los países de la OCDE. Dentro de ese gasto hay una partida que conviene conocer: la enseñanza concertada, es decir, colegios de titularidad privada financiados con dinero público. Suponen unos 7.500 millones de euros al año, cerca del 12 por ciento de todo el gasto educativo público. En comunidades como el País Vasco, Madrid o Navarra ese porcentaje es bastante mayor. Y un matiz importante: lo que las familias pagan de su bolsillo en la enseñanza privada no concertada no es gasto del Estado, y por eso no entra en esta cuenta.

**Sanidad**
La sanidad es hoy la mayor partida social del país. Despegó con la Ley General de Sanidad de 1986, que creó un sistema sanitario público y universal. El gasto público pasó de alrededor del 4 por ciento del PIB en 1980 a un 6,5 por ciento justo antes de la pandemia. Y entonces llegó la COVID. En 2020, el gasto sanitario público saltó hasta el 8 por ciento del PIB, el nivel más alto jamás registrado. En 2023 se situó en el 7 por ciento. Si a esa cifra le sumamos la sanidad privada —los seguros y lo que los hogares pagan directamente, en torno a un 2,5 por ciento más— el país dedica a la salud cerca del 10 por ciento de todo lo que produce. Un dato llama la atención: España es uno de los países de la OCDE con mayor peso de la sanidad privada. Aproximadamente uno de cada cuatro euros que se gastan en salud es dinero privado, no público.

**La Iglesia**
Llegamos al asunto más debatido: cuánto dinero destina el Estado a la Iglesia católica. Conviene aclarar cómo funciona. Desde 2007, el Estado ya no entrega una dotación directa a la Iglesia. Su financiación pública procede de la casilla del 0,7 por ciento del IRPF, que cada contribuyente decide marcar, o no, en su declaración de la renta. En 2024, esa casilla aportó 429 millones de euros, la cifra más alta de la historia, con más de 9 millones de personas marcándola. Ahora bien, hay que ser honestos: esos 429 millones son únicamente la asignación del IRPF. El coste público real es considerablemente mayor si se suman otras partidas: los profesores de religión en la escuela pública, los conciertos de los colegios religiosos, las capellanías en el ejército, los hospitales y las prisiones, la conservación del patrimonio y las exenciones fiscales. El problema es que esas partidas están repartidas entre muchas administraciones, no se consolidan en una única cifra oficial, y su cálculo es objeto de disputa política. Por eso no las incluimos en el gráfico: preferimos señalar su existencia antes que ofrecer un número inventado. En proporción, la asignación vía IRPF equivale a apenas el 0,03 por ciento del PIB: otra escala por completo frente a la sanidad o la educación.

**Infraestructuras**
Última gran partida: las infraestructuras de transporte, es decir, carreteras, ferrocarril, puertos y aeropuertos. Es la más cíclica de todas, un auténtico espejo de la economía. En 2009, en pleno despliegue del AVE y de las autovías, la inversión alcanzó el 2,1 por ciento del PIB: unos 24.000 millones de euros. Luego vino el ajuste. Para 2018, la inversión se había hundido un 72 por ciento, hasta apenas el 0,55 por ciento del PIB. En los últimos años se recupera: en 2025 ronda los 16.000 millones, cerca del 1 por ciento del PIB, aunque todavía muy por debajo de los niveles de 2009 en términos reales. De todo ese dinero, las carreteras se han llevado históricamente algo más de la mitad; hoy, en torno a un tercio.

**Metodología**
Una palabra sobre el rigor de estos datos. Las cifras proceden de fuentes oficiales: el Instituto Nacional de Estadística, los ministerios de Educación y de Sanidad, la OCDE, la Agencia Tributaria, la Conferencia Episcopal y el Banco de España. Los datos desde el año 2000 son sólidos. Los de los años ochenta y primeros noventa son estimaciones reconstruidas a partir de literatura académica y series históricas, y así aparecen señaladas. Deben leerse como tendencias fiables, no como contabilidad al céntimo.

**Conclusión**
En resumen: a lo largo de 45 años, España ha apostado de forma creciente por la sanidad y la educación, aunque todavía por debajo de sus vecinos europeos. La inversión en obra pública sube y baja al ritmo del ciclo económico. Y el dinero directo a la Iglesia es pequeño en la parte que puede medirse con claridad. Si te ha servido para entender mejor a dónde va el dinero de todos, suscríbete y déjame en los comentarios qué partida te ha sorprendido más. Los datos están sobre la mesa; las conclusiones, cada uno las suyas. Nos vemos en el próximo vídeo.

### Ficha para YouTube

**Títulos sugeridos**
- ¿A DÓNDE VA TU DINERO? Lo que España gasta en sanidad, educación e Iglesia (1980–2025)
- 45 años de gasto público en España, explicados con datos
- Sanidad, colegios, carreteras e Iglesia: en qué gasta de verdad el Estado español

**Descripción**
Un recorrido con datos oficiales por el gasto del Estado español entre 1980 y hoy: educación pública y concertada, sanidad pública y privada, financiación de la Iglesia e inversión en infraestructuras. Todo medido en porcentaje del PIB para comparar de forma justa. Fuentes: INE, Educación, Sanidad, OCDE, Agencia Tributaria, Conferencia Episcopal y Banco de España.

**Capítulos**
```
00:00  Introducción
00:25  La trampa de los euros: por qué medimos en % del PIB
01:15  Visión general
01:55  Educación y concertada
02:55  Sanidad pública y privada
03:55  La Iglesia: el 0,7 % y lo que no se ve
05:05  Infraestructuras
05:50  Metodología y fuentes
06:20  Conclusión
```

---

## 8. Especificación del short 9:16 (`artefactos/short.html`)

Presentación autorreproducible. Pulsar ▶ y grabar la pantalla (capturando audio de la pestaña si se quiere la narración TTS). Línea de tiempo:

| Escena | Dur. | Contenido | Narración (TTS) |
|---|---|---|---|
| 0 | 7 s | Gancho: "¿A dónde va el dinero del Estado?" | sí |
| 1 | 12 s | Regla: ×6 precios / +30 % población / ×17 economía → % PIB | sí |
| 2 | 12 s | Sanidad 4→8 % · Educación ×2 | sí |
| 3 | 11 s | Infra: 2,1 % (2009) → −72 % (2018) | sí |
| 4 | 14 s | Iglesia: 429 M€ (2024) · el coste real es mayor | sí |
| 5 | 9 s | Cierre + CTA | sí |

**Total ≈ 65 s.** Modo oscuro fijo (para que se vea igual en cualquier dispositivo). Narración mediante Web Speech API del navegador (es-ES); conmutable con el botón "Voz".

### Opciones de audio (recomendación)
1. **Voz TTS del navegador (incluida):** rápida, pero calidad sintética. Graba capturando el audio de la pestaña.
2. **Tu voz (recomendado para calidad):** graba el short en silencio y añade tu locución en el editor (CapCut, Premiere) usando el texto del §6/§7.
3. **TTS profesional (ElevenLabs, etc.):** genera el audio con el texto del guion y móntalo en el editor.

---

## 9. Cómo continuar con Claude Code (ideas)

Prompts útiles para seguir en local:
- "Añade al dashboard (`artefactos/comparador.html`) una pestaña de **pensiones** y **defensa** para comparar magnitudes."
- "Afina la serie 1980–1995 de sanidad con datos del Banco de España y marca cada punto con su fuente."
- "Convierte `artefactos/short.html` en 6 imágenes PNG 1080×1920 (una por escena) para montarlas en un editor."
- "Genera una versión de 30 s del short (Gancho + Iglesia + Cierre)."
- "Exporta el dashboard a un PDF estático para imprimir."

## 10. Avisos y limitaciones

- Las cifras pre-1995 son estimaciones; los años intermedios de las líneas se interpolan visualmente entre puntos reales.
- "Gasto público" en educación y sanidad incluye todas las administraciones (Estado + Comunidades Autónomas).
- La financiación **indirecta** de la Iglesia no se cuantifica por falta de cifra oficial consolidada.
- "Infraestructuras" se refiere a **transporte** (no a toda la obra pública), para tener serie homogénea 1985–2025.
- Reproducibilidad del TTS: depende de las voces en español instaladas en el navegador/sistema.
