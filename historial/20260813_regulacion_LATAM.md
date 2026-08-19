# Panorama Regulatorio BESS — LATAM

> **Estado de este archivo — corrida de vigilancia del 2026-08-13 (primera corrida real).**
>
> El contenido original de este archivo era un *seed* extraído de `BESS_POTENTIAL_CLIENTS_v2.xlsx` (corte 2026-08-12), sin validación. En esta corrida se validaron contra fuente oficial los ítems marcados **(a)**; el resto conserva su estatus de seed no verificado y sigue marcado como tal.
>
> **Clasificación de fuente usada en todo el documento:**
> - **(a)** Texto o resolución oficial confirmada directamente por esta vigilancia (documento primario o comunicado del regulador).
> - **(b)** Interpretación o análisis de esta vigilancia sobre texto oficial.
> - **(c)** Borrador, proyecto en consulta, anuncio o reporte secundario aún no confirmado contra fuente oficial.
> - **(seed)** Heredado del archivo de mercado interno, **no verificado** en esta corrida.

---

## Chile

### Reguladores / instituciones
- **Ministerio de Energía** — máxima autoridad ejecutiva: política energética nacional, planificación estratégica, decretos que regulan generación, transmisión, distribución y almacenamiento. *(seed)*
- **CNE — Comisión Nacional de Energía** — cuerpo técnico asesor: normas regulatorias, precios regulados, metodologías de servicios complementarios y almacenamiento; convoca las licitaciones de suministro. *(a)*
- **CEN — Coordinador Eléctrico Nacional** — operador del sistema: despacho, costo marginal, liquidaciones, validación de modelos EMT y verificación de instalaciones IBR GFM. *(a)*
- **SEC — Superintendencia de Electricidad y Combustibles** — fiscaliza la ley eléctrica, otorga concesiones, autoriza conexión física. *(seed)*
- **Panel de Expertos** — resuelve disputas técnicas y tarifarias vinculantes. *(seed)*
- **Ministerio del Medio Ambiente / SEA / SMA** — SEIA y RCA; el MMA además elabora el DS de metas REP para baterías. *(a)*

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Estado |
|---|---|---|---|---|
| Ley General de Servicios Eléctricos (LGSE) | Regulación de mercado | Marco original de generación/transmisión/distribución, sin almacenamiento contemplado originalmente. | Norma base. | (seed) |
| Ley N°20.936 | Regulación de mercado | Primera ley en reconocer sistemas de almacenamiento. Define SAE y CRCA. | Introduce categorías legales SAE/CRCA. | (seed) |
| Ley N°21.505 | Regulación de mercado | Permite a SAE stand-alone vender energía y recibir pagos por potencia de suficiencia. | Habilita el business case stand-alone. | (seed) |
| DS N°62 | Regulación de mercado | Pagos por potencia de suficiencia para generadores. | Tecnología de referencia: diésel. | (seed) |
| DS N°70 | Regulación de mercado | Modifica DS 62 y DS 125: baterías stand-alone reciben pagos por potencia según duración de descarga. | Tabla de reconocimiento por duración (SAE y CRCA). | (seed) |
| Ley N°21.721 | Transmisión | Acelera permisos de transmisión. | Complemento estratégico. | (seed) |
| DS N°125 | Regulación de mercado | SAE puede proveer SSCC; incluye BESS en despacho económico y formación de precios. | Habilita pago por servicios complementarios. | (seed) |
| DS N°37 | Transmisión | Conecta SAE a la planificación de transmisión. | BESS puede sustituir expansión de transmisión. | (seed) |
| MINVU 522 | Planificación urbana | Clasifica BESS stand-alone como "Infraestructura Energética" (Art. 2.1.29 OGUC). | Permiso de edificación, no concesión. | (seed) |
| Ley N°20.920 (REP) | REP | Baterías industriales ≥5 kg como producto prioritario. | Ver actualización REP más abajo. | (seed) |
| DS 88 | Regulación de mercado | BESS bajo 9 MW en régimen PMGD puede usar margen de capacidad disponible para carga. | Vía C&I distribuido. | (seed) |
| **NTSyCS** | Seguridad | Norma Técnica de Seguridad y Calidad de Servicio. **Modificada por REx CNE N°45/2026**, que incorpora el AT IBR y el AT de Estudio de Robustez como anexos técnicos de la propia NTSyCS. | **Norma primaria del marco técnico**; el AT IBR cuelga de ella. | (a) |
| REx CNE N°41-2025 | Seguridad | Requisitos sísmicos para BESS e instalaciones AT; referencia NCh 2369:2023 e IEEE 693:2018. | Obligatorio para permisos e ingeniería. | (seed) |
| DS N°148 | Seguridad | Residuos peligrosos, incluidos componentes de baterías de litio. | Operación y desmantelamiento. | (seed) |
| DS N°8 | Seguridad | Instalaciones eléctricas de consumo (fichas RIC). | — | (seed) |
| **REx CNE N°45/2026 — AT IBR** | Código de red | Ver detalle en la sección siguiente. | **Marco vinculante de GFM para todo SAE.** | (a) |

### 🔴 Actualización crítica — REx CNE N°45/2026 y el AT IBR *(verificado en esta corrida)*

**Fuente primaria (a):** texto del Anexo Técnico publicado por CNE — `cne.cl/wp-content/uploads/2026/02/2026.01.28_AT-IBR_RES45.pdf`; compendio ACERA "Grid-Forming en Chile" (mayo 2026).

- **Fecha correcta:** la Resolución Exenta CNE **N°45/2026** fue **publicada en el Diario Oficial el 3 de febrero de 2026** (el anexo está fechado 28-ene-2026). *Corrige el dato previo de este archivo, que decía "marzo 2026".*
- **Qué hace la REx 45/2026:** aprueba la **modificación de la NTSyCS**, crea el **AT IBR** (Anexo Técnico de Exigencias Mínimas de Instalaciones Basadas en Convertidores) y el **AT de Metodología para el Estudio de Análisis de Robustez**, y **modifica la NT de Servicios Complementarios**.
- **GFM ES OBLIGATORIO para almacenamiento.** El Artículo 3-12 del AT IBR dice textualmente: *"Todo Sistema de Almacenamiento de Energía o componente de almacenamiento de una CRCA que se interconecten al SEN deberá cumplir con ser una IBR GFM."* → **Corrige el dato previo de este archivo, que decía "GFM no obligatorio aún".**
- **Alcance:** IBR interconectadas o a interconectarse al Sistema de Transmisión del SEN.
- **Cambio de modo GFM↔GFL:** el Coordinador puede instruirlo a partir del Estudio de Análisis de Robustez, limitado a ajustes de software y comunicaciones (Art. 3-12).

**Exigencias técnicas destacadas para IBR GFM (Título 3) (a):**
- Tiempo de Reacción < 10 ms; Tiempo de Establecimiento < 20 ms.
- Sobrecorriente ≥ **1,3 p.u. por 5 segundos** sin comprometer la instalación — verificable **en el convertidor/PCS**, sin equipos adicionales (Oficio 337/2026).
- Regulación autónoma de tensión y frecuencia en el punto de conexión; FIV predominantemente constante en régimen transitorio.
- Respuesta inercial, control activo de salto de fase, control de amortiguamiento de potencia, control de inyección rápida de corriente.
- **Operación en isla eléctrica: obligatoria**, pero el alcance es *mantener* operación estable en isla, no necesariamente *formarla* (Oficio 337/2026).
- **Partida autónoma (black start): opcional.**
- Operación estable conectada a Red Débil.
- Registro de RoCoF y de ángulo de salto de fase (medio ciclo, resolución 10 µs).

**Régimen de exenciones y fechas críticas (a):**

| Fecha | Hito | Estado al 2026-08-13 |
|---|---|---|
| 3-feb-2026 | Publicación DO de REx CNE N°45/2026. Fecha de corte para exenciones por declaración en construcción. | Cumplida |
| 24-feb-2026 | Publicación del cronograma de adecuaciones para IBR GFL y SAE. | Cumplida |
| 25-mar-2026 | Oficio Ordinario CNE N°328/2026 (aplicación del Art. 7-2, solicitudes de exención SAE). | Cumplida |
| 30-mar-2026 | Oficio Ordinario CNE N°337/2026 (precisiones técnicas y transitorias). | Cumplida |
| 3-may-2026 | Plazo para que el Coordinador defina el cronograma de entrega de modelos EMT. | Cumplida |
| 6-may-2026 | CEN publica la *Guía para la Verificación de Instalaciones Basadas en Inversores Grid Forming* (foco BESS). | Cumplida |
| **3-jul-2026** | **Plazo límite para solicitar exención total o parcial del Título 3 (GFM) para SAE y componente de almacenamiento de CRCA.** | **VENCIDO** |
| **3-ago-2026** | **Entrada en operación límite para acogerse a la exención GFM. Desde esta fecha, los proyectos aplicables deben entregar modelo EMT validado antes de la entrada en operación.** | **VENCIDO** |
| 3-nov-2026 | Plazo para que IBR GFL presenten plan de adecuación (o informe de imposibilidad técnica). | Pendiente |
| 3-feb-2027 | Fecha límite de publicación del primer Estudio de Análisis de Robustez del SEN. | Pendiente |
| 3-may-2027 | Plazo para que el Coordinador publique el listado de niveles mínimos de cortocircuito y factores agregados de interacción IBR. | Pendiente |

**Regla específica para SAE (a):** solo quedaron exentos de las exigencias GFM los proyectos que cumplieran **copulativamente** declaración en construcción al 3-feb-2026 **y** entrada en operación antes del 3-ago-2026.

**Lectura de esta vigilancia (b):** ambas ventanas de exención ya cerraron. Desde el 3-ago-2026, **todo SAE nuevo que se interconecte al SEN debe ser IBR GFM y entregar modelo EMT validado por el Coordinador antes de la entrada en operación**. La capacidad GFM certificada dejó de ser un diferenciador comercial y pasó a ser condición de conexión.

**Requisitos de interconexión para IBR GFL (a):** SCR ≥ 3 y ESCR ≥ 1,5 en el punto de conexión (Art. 4-8), no aplicable a GFL con declaración en construcción al 3-feb-2026. El Oficio 337/2026 admite cumplirlos mediante soluciones tecnológicas complementarias permanentes.

**Modelos EMT (a):** deben ser de fabricante original (OEM), compatibles con el software del Coordinador, y validados antes de la entrada en operación (para instalaciones posteriores al 3-ago-2026). Instalaciones existentes sin modelo OEM pueden entregar modelos genéricos validados por especialista.

### Otras novedades Chile *(verificadas en esta corrida)*

- **Licitación de Suministro 2026/01 (a).** La CNE aprobó las **Bases Definitivas el 17-jul-2026**. Volumen: **2.835 GWh/año** en dos bloques de 15 años (SB1: 1.575 GWh/año, 2029–2043; SB2: 1.260 GWh/año, 2030–2044). Las bases **excluyen carbón, coque de petróleo, diésel y fuel oil N°6 como combustibles de respaldo** y **mantienen los sistemas de almacenamiento como recurso de respaldo válido**. Cronograma: consultas cierran 28-ago-2026; bases finales y respuestas 2-oct-2026; presentación de ofertas 4-dic-2026; **adjudicación en enero 2027**.
- **Ley REP — DS de metas para baterías (a).** El MMA, mediante **REx N°4225/2026**, **extendió seis meses el plazo para elaborar el DS** que fijará metas de recolección y valorización de baterías bajo Ley 20.920: nuevo plazo **29-ene-2027**. El MMA aún debe definir qué categorías/subcategorías quedan afectas, lo que determina si las baterías de proyectos BESS a escala de red entran o no en el régimen.
- **Servicios complementarios de robustez (c).** En marzo 2026 la CNE licitó el estudio "Definición de nuevos Servicios Complementarios que contribuyan a la robustez del SEN" y el Coordinador emitió el Informe de Propuesta de SSCC 2026. Categorías en discusión: respuesta inercial, rampas de potencia activa, fortaleza de tensión / potencia de cortocircuito, y adecuaciones a partida autónoma. **Aún sin norma que las valorice.**

### Políticas públicas relevantes *(seed, no verificadas en esta corrida)*
- **Plan Nacional de Almacenamiento — Terrenos Fiscales**: arriendo directo en terrenos fiscales del Norte Grande (Tarapacá, Antofagasta, Atacama), sin licitación pública.
- **Segunda Fase de la Agenda de Transición Energética**: storage como pilar explícito.
- **Estudio de Almacenamiento CEN (2023)**: 1.000–4.000 MW óptimos (2026–2032), duración 6–8h, 13,2 GWh diarios.

### Nota de estructura
Las licitaciones de suministro chilenas contratan **energía (GWh/año)**; el BESS entra por lógica de mercado, por su rol como respaldo elegible y por el mandato técnico del AT IBR — no por un mandato de contratación de capacidad de almacenamiento.

---

## Argentina

### Reguladores / instituciones
- **Secretaría de Energía (SE)** — autoridad de política; convocó y adjudicó AlmaGBA y AlmaSADI. *(a)*
- **CAMMESA** — OED; en AlmaSADI actúa como **Comprador** de los Acuerdos de Almacenamiento. *(a)*
- **CFEE** — consejo asesor; administra el FNEE. *(seed)*
- **Ente Nacional Regulador del Gas y la Electricidad** (fusión ENRE + ENARGAS, Decreto 452/2025). *(seed)*
- **EDENOR / EDESUR** — compradoras en AlmaGBA. *(seed)*
- **Transener** — transportista troncal 500 kV. *(seed)*

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Estado |
|---|---|---|---|---|
| Ley N°15.336 | Marco general | Ley fundacional del sector; jurisdicción federal vía SADI. | Base legal de las resoluciones SE. | (seed) |
| Ley N°24.065 | Mercado mayorista | Crea el MEM competitivo. Decreto 450/2025 restauró principios marginalistas. | Base legal citada por toda resolución BESS. | (seed) |
| Ley N°27.742 (Ley Bases) | Inversión privada | Delegó al Ejecutivo la actualización del marco eléctrico. | Habilitó Decreto 450/2025 y Res. 400/2025. | (seed) |
| Ley N°26.190 y N°27.191 | Renovables | Meta 20% renovables para consumidores ≥300 kW. | Demanda cautiva MATER; híbridos BESS. | (seed) |
| SE Res. N°36/2023 y N°906/2023 (RenMDI / ALMA MDI) | Renovables / híbrido | 633,7 MW adjudicados en 98 proyectos. | Primer marco contractual con datos técnicos de BESS. | (seed) |
| **SE Res. N°67/2025 — AlmaGBA** | Storage stand-alone | Primera licitación exclusiva de storage stand-alone. 713 MW adjudicados en ago-2025. | "Storage Generation Contract". Duración mínima de descarga 4h (HAC). Compradores: EDENOR/EDESUR. | (seed) |
| SE Res. N°344, 361, 384/2025 | Storage stand-alone | Formalizan la adjudicación de AlmaGBA. | Capacidad hasta USD 12.500/MW/mes; energía USD 10/MWh fijo hasta 2037. | (seed) |
| **SE Res. N°50/2026 — AlmaSADI (convocatoria)** | Storage stand-alone | **Publicada en el Boletín Oficial el 2-mar-2026.** Convocatoria nacional (todo el SADI). **CAMMESA es el Comprador** (no solo garante). | Ver detalle abajo. | (a) |
| **SE Res. N°155/2026 — AlmaSADI (adjudicación)** | Storage stand-alone | **Publicada el 7-jul-2026.** Formaliza la adjudicación de AlmaSADI e instruye a CAMMESA a notificar y suscribir los Acuerdos de Almacenamiento. | Ver detalle abajo. | (a) |
| SE Res. N°400/2025 — Normalización MEM | Reforma MEM | Vigente desde 1-nov-2025. Crea Mercado a Término de Energía y Capacidad. | BESS de AlmaGBA/AlmaSADI como "Nueva Generación". | (seed) |
| Decreto N°450/2025 | Reforma estructural | Restaura principios marginalistas; transición de 24 meses (hasta jul-2027). | Distribuidoras deben contratar ≥75% de su demanda a largo plazo. | (seed) |
| Decreto 513/2025 | Incentivo fiscal | Arancel de importación de sistemas de batería de litio a 12,6%. | Reduce CAPEX importado. | (seed) |
| RIGI — Ley 27.742, Título VII | Incentivo de inversión | Proyectos >USD 200M; estabilidad fiscal y regulatoria 30 años. | Clusters BESS grandes o renovable+storage integrados. | (seed) |

### 🔴 Actualización — AlmaSADI adjudicada *(verificado en esta corrida)*

**Fuente (a):** comunicado oficial `argentina.gob.ar` (7-jul-2026); Res. SE N°155/2026; Res. SE N°50/2026 (BO 2-mar-2026).

**Convocatoria (Res. SE N°50/2026):**
- Potencia convocada: **700 MW**, con cupos regionales: **Buenos Aires 150 MW, NEA 250 MW, NOA 120 MW, Centro 100 MW, Cuyo 100 MW, La Pampa 50 MW**.
- Tamaño de proyecto: **10–150 MW por nodo**.
- **Duración mínima de descarga: 4 horas consecutivas** para BESS nuevas.
- **Plazo de los Acuerdos de Almacenamiento: 15 años**, contados desde la habilitación comercial o el 1-ene-2027, lo que ocurra primero. → **Corrige el dato previo de este archivo, que decía "contratos a 10 años".**
- Comprador: **CAMMESA**.
- Cronograma: apertura sobre "A" 8-may-2026; apertura sobre "B" (oferta económica) 5-jun-2026; **notificación de adjudicación 19-jun-2026**; suscripción de acuerdos desde 25-jun-2026.

**Resultado de la adjudicación (Res. SE N°155/2026, 7-jul-2026):**
- **700,5 MW adjudicados en 20 proyectos de 5 empresas**: GENNEIA (7), DQD Energy (8), 360 Energy Solar (3), ALUAR (1), INTERMEPRO (1).
- Distribución: PBA 185 MW; NOA 150 MW; NEA Chaco-Formosa 161,5 MW; NEA Misiones-Corrientes 50 MW; Litoral Entre Ríos 50 MW; Litoral Santa Fe 36 MW; Pampa 68 MW.
- **Sobre-suscripción masiva: 235 ofertas por 8.338 MW** (≈12× el cupo), de 37 empresas.
- **Precio promedio adjudicado: USD 8.427/MW-mes** (vs. hasta USD 12.500/MW/mes en AlmaGBA).
- Inversión estimada de la etapa: **USD 700 millones**.

**Lectura de esta vigilancia (b):** la caída del precio de capacidad respecto de AlmaGBA (≈−33%) y la sobre-suscripción de 12× indican un mercado argentino de storage stand-alone ya competitivo y con presión a la baja en CAPEX/OPEX ofertado. Para una próxima ronda, el precio de referencia relevante ya no es AlmaGBA sino AlmaSADI.

### Políticas públicas relevantes
- **RENPALMA** — Registro Nacional de Proyectos de Almacenamiento. *(seed)*

### Nota de estructura
AlmaSADI contrata directamente **capacidad de almacenamiento (MW, con 4h de descarga)** stand-alone, con CAMMESA como comprador — modelo distinto al chileno (energía) y al colombiano (producto en subasta).

---

## Colombia

### Reguladores / instituciones
- **MinMinas y Energía** — política energética; convoca la subasta de largo plazo (CLPE). *(a)*
- **CREG** — regula el MEM; **expidió el marco definitivo de SAEB** (ver abajo). *(a)*
- **UPME** — planificación (PEN 2024–2054); aprueba conexiones. *(seed)*
- **XM (ISA)** — operador del SIN (CND) y administrador del mercado (ASIC). *(seed)*
- **ANLA / SSPD** — licenciamiento ambiental / supervisión de utilities. *(seed)*
- **BMC — Bolsa Mercantil de Colombia** — operador de la subasta de largo plazo 2026. *(a)*

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Estado |
|---|---|---|---|---|
| Ley 143/1994 | Marco legal sectorial | Crea la CREG; modelo de pool competitivo. | Fundación del modelo de mercado. | (seed) |
| Ley 1715/2014 | Marco FNCER | Incentivos fiscales (deducción 50% renta, exención IVA, arancel cero, depreciación 33%/año). | Aplica a BESS acoplado a FNCER. | (seed) |
| Ley 2099/2021 | Marco FNCER | Extiende incentivos; primer reconocimiento legal del almacenamiento en planificación del SIN. | Base legal para storage. | (seed) |
| Res. CREG 071/2006 | Cargo por confiabilidad | OEF, precio de escasez, condición crítica. | Vía potencial para BESS. | (seed) |
| Res. CREG 098/2019 | Storage | Primer reconocimiento regulatorio del almacenamiento; habilitó pilotos. Vigencia limitada hasta dic-2022. | Antecedente, hoy superado por Res. 101 113/2026. | (a) |
| Res. CREG 101 066/2024 | Precios de escasez | Diferencia precios de escasez por tipo de planta. | Afecta competitividad de BESS en Confiabilidad. | (seed) |
| **Decreto 1091/2025** | Contratación de largo plazo | Directrices de política para contratación de largo plazo de generación y storage. | Habilita BESS standalone en subastas de largo plazo. | (seed) |
| **Decreto 0393/2026** | Política pública de almacenamiento | **Expedido el 10-abr-2026.** Lineamientos de política pública para integrar Sistemas de Almacenamiento de Energía (SAE) en el **SIN y en las ZNI**. Da a la CREG **12 meses** para la normativa regulatoria completa. | **Nueva pieza de cabecera** del marco de almacenamiento colombiano. | (a) |
| **Res. CREG 101 113 de 2026** | Marco técnico-comercial SAEB | **Expedida el 19-jun-2026.** *"Por la cual se definen los mecanismos para incorporar sistemas de almacenamiento de energía eléctrica con baterías -SAEB- en el Sistema Interconectado Nacional."* **Resolución definitiva que cierra la consulta pública del Proyecto CREG 701-103/2025.** | **Norma primaria de BESS en Colombia.** Ver detalle abajo. | (a) |
| ~~Res. CREG 701-103/2025~~ | Proyecto (cerrado) | Era el **proyecto** en consulta pública. **Ya no es el documento aplicable**: fue reemplazado por la Res. CREG 101 113 de 2026 tras el análisis de comentarios y las recomendaciones de la SIC. | Referencia histórica únicamente. | (a) |
| Res. MinMinas 40178/2026 | Contratación de largo plazo | Reglas generales para contratación de largo plazo de energía limpia. | Marco habilitante previo a la CLPE. | (seed) |
| **Res. MinMinas 40208/2026** | Subasta de largo plazo (CLPE) | Convoca la primera CLPE con almacenamiento como producto. **Ya ejecutada** — ver resultados abajo. | Hito ejecutado. | (a) |

### 🔴 Actualización — Res. CREG 101 113 de 2026 (marco definitivo SAEB) *(verificado en esta corrida)*

**Fuente (a):** gestor normativo CREG y comunicado oficial CREG (19-jun-2026).

- **Dos categorías de participación de SAEB:**
  1. **SAEB como activos de red** (Título I) — conectados al STN, STR o SDL, identificados por necesidades del sistema. La resolución define cuándo son necesarios, cómo se desarrollan los proyectos, **cómo se remuneran según nivel de tensión**, sus obligaciones de calidad de servicio y cómo se gestiona la energía almacenada.
  2. **SAEB independientes** (Título II) — operan con **dos fronteras comerciales** (carga y descarga) y participan en el mercado mayorista **a través de un agente generador que los represente comercialmente**.
- El comunicado de la CREG también describe la participación de SAEB como **parte de recursos híbridos de generación** de cualquier capacidad.
- **Plazos:** procedimientos de liquidación y exclusión de pérdidas, 3 meses desde la entrada en vigor; proyectos en SDL, presentación con 18 meses de anticipación.
- **No deroga expresamente** resoluciones anteriores; complementa la Res. CREG 098/2019 (cuya vigencia estaba limitada a dic-2022) con un marco integral actualizado.
- La CREG declaró que esta resolución es **"un primer paso"**, y que continúa desarrollando resoluciones para **otras tecnologías de almacenamiento** y nuevos servicios, conforme al Decreto 0393/2026.

### 🔴 Actualización — resultados de la CLPE 2026 *(verificado en esta corrida)*

**Fuente (a):** informe de cierre de la BMC y comunicados MinEnergía; reportes de prensa especializada (jul–ago 2026).

- **Jornadas: 28 y 29 de julio de 2026.** Contratos a **15 años**, con obligaciones desde el **1-ene-2030**.
- **Producto 1 (energía convencional / inicio 2035): CANCELADO** — no alcanzó el mínimo de 3 competidores.
- **Producto 2 (solar FV): ADJUDICADO — 995 MW.**
- **Producto 3 (híbrido solar + almacenamiento): ADJUDICADO — 390 MWh-día de almacenamiento** (≈100 MW de SAEB) acoplados a ≈270 MW solares. Entrega en dos bloques: 8:00–18:00 (solar) y 18:00–22:00 (energía desplazada por batería). Precio de cierre ≈ **315,87 COP/kWh**.
- **Producto 4 (suministro nocturno 18–22h respaldado por almacenamiento): DESIERTO — sin adjudicaciones**, pese a recibir ofertas por 558 MWh-día contra una demanda de 5.990 MWh-día.
- **Adjudicatarios (4 empresas):** Bosques Solares de los Llanos 8, Celsia (Parque Solar Andrómeda), Enel Colombia y EPM. Los dos proyectos con almacenamiento fueron Bosques Solares de los Llanos 8 y Andrómeda (Celsia).

**Lectura de esta vigilancia (b):** el resultado separa nítidamente dos tesis de negocio. El **BESS acoplado a solar (Producto 3) es hoy bancable en Colombia**; el **respaldo nocturno / stand-alone (Producto 4) no encontró oferta adjudicable** — la demanda convocada (5.990 MWh-día) superó en más de 10× la oferta presentada (558 MWh-día) y aun así quedó desierta, lo que sugiere que las condiciones de precio o riesgo del producto no cerraron para los oferentes. Queda una necesidad de suministro nocturno explícitamente reconocida y no cubierta.

> ⚠️ **Discrepancia de fechas en fuentes secundarias:** algunas notas de prensa ubican las jornadas el 23–24 de julio y otras el 28–29 de julio de 2026. Se adoptó **28–29 de julio** por corresponder al informe de cierre de la BMC. Verificar contra el acto administrativo de adjudicación en la próxima corrida.

### Políticas públicas relevantes
- Incentivos FNCER activos (deducción de renta 50%, exclusión de IVA, arancel cero, depreciación acelerada hasta 33,3%/año), trámite UPME + certificación ANLA. *(seed)*

### Nota de estructura
El caso colombiano está enraizado en riesgo hidrológico (El Niño). El almacenamiento entra por **producto de subasta** (Producto 3, híbrido) y ahora también por **marco regulatorio propio** (Res. CREG 101 113/2026), que habilita SAEB como activo de red, híbrido o independiente.

---

## Perú

### Reguladores / instituciones
- **MINEM** — política energética; elabora el Reglamento de Servicios Complementarios. *(a)*
- **OSINERGMIN** — normas técnicas, aprobación de procedimientos del COES. *(seed)*
- **ProInversión** — PNER; microrredes solar-storage rurales. *(seed)*
- **COES** — operador del SEIN; procedimientos técnicos (PR20). *(seed)*

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Estado |
|---|---|---|---|---|
| D.Leg. 25844 — Ley de Concesiones Eléctricas | Marco legal | Separa generación, transmisión y distribución. | No contempla almacenamiento. | (seed) |
| D.S. 009-93-EM — Reglamento LCE | Regulación de mercado | Despacho por mérito, tarifas, obligaciones. | Sin mención de almacenamiento. | (seed) |
| Ley 28832 | Regulación de mercado | Licitaciones de energía, OEF. | Marco modificado por Ley 32249. | (seed) |
| Res. OS 224-2021 | Regulación de mercado | Modifica el cálculo de costos variables del COES. | Mejora la señal de precio spot. | (seed) |
| RM 278-2023-MINEM — Hoja de Ruta Smart Grids | Política pública | Estrategia 2023–2030; reconoce el almacenamiento. | Sin normativa de desarrollo. | (seed) |
| **Ley 32249 — Modificación Ley 28832** | Regulación de mercado | Crea la figura del **Proveedor de Servicios Complementarios (PSC)**; habilita PPAs sin respaldo de potencia. Publicada en enero de 2025. | Marco legal que reconoce BESS standalone como PSC. | (seed) |
| **PR20 — Procedimiento técnico COES** | Requisito técnico | Obliga a aportar inercia sintética desde **2028**. | **Mandato técnico sin remuneración definida.** | (seed) |
| **Reglamento de Servicios Complementarios (MINEM)** | **PROYECTO — no aprobado** | Ver detalle abajo. | **Pieza pendiente más crítica del mercado peruano.** | (c) |
| Reglamentación de generación distribuida | Pendiente | Marco para GD, prosumidores y BESS behind-the-meter. | Su ausencia bloquea C&I y electrificación rural. | (seed) |

### 🟡 Estado del Reglamento de Servicios Complementarios *(revisado en esta corrida — sigue SIN confirmar como aprobado)*

- **(a) Confirmado:** mediante **Resolución Ministerial N°171-2026-MINEM/DM (19-abr-2026)**, el MINEM dispuso la publicación del **proyecto** de Decreto Supremo que aprueba el *Reglamento de los Servicios Complementarios* y modifica el Reglamento de la LCE, el Reglamento del Mercado Mayorista de Electricidad y el Reglamento del COES. Plazo de comentarios: **25 días calendario, vencido el 14-may-2026**.
- **(a) Contenido del proyecto:** crea un mercado de servicios complementarios con esquema de provisión y remuneración, mecanismos competitivos, y habilita la participación de nuevas tecnologías incluidos **sistemas de almacenamiento con baterías**. Amplía los agentes elegibles (generadores, transmisores, distribuidores, usuarios libres y otros autorizados por MINEM). Prevé que **MINEM tenga 120 días calendario** para adecuar la normativa técnica de operación en tiempo real, y el **COES 180 días calendario** para remitir a OSINERGMIN la propuesta de procedimientos técnicos.
- **(c) NO CONFIRMADO:** una nota de prensa especializada (Energía Estratégica / Latin Energy Group) reporta que Perú "publica uno de los reglamentos de la Ley 32249", pero **no fue posible confirmar el número ni la fecha del Decreto Supremo** contra El Peruano ni contra el portal de normas legales del MINEM en esta corrida. Fuentes de julio de 2026 seguían refiriéndose al texto como **proyecto**.

**Conclusión de esta vigilancia (b):** al 13-ago-2026 **no se puede dar por vigente** el Reglamento de Servicios Complementarios. El business case de BESS standalone en Perú sigue siendo **especulativo en su remuneración**, mientras el mandato técnico del PR20 (inercia sintética desde 2028) permanece firme. **La brecha mandato-vs-remuneración sigue abierta.** Es el ítem de mayor prioridad de verificación para la próxima corrida.

### Nota de estructura
El mandato técnico (PR20) va por delante de la remuneración. Es la brecha regulatoria más relevante a monitorear en este mercado.

---

## Uruguay

### Reguladores / instituciones
- **MIEM — Ministerio de Industria, Energía y Minería** (Dirección Nacional de Energía) — política energética. *(a)*
- **URSEA** — regulación técnica y tarifaria. *(seed)*
- **UTE** — utility estatal; distribuidora y compradora. *(a)*
- **ADME** — administrador del mercado eléctrico; **sanciona el precio spot horario** con que se remunera la energía inyectada. *(a)*

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Estado |
|---|---|---|---|---|
| **Decreto N°27/020** | Regulación de mercado | Habilita a **Suscriptores conectados a la Red de Distribución de Baja Tensión** a generar energía mediante una **instalación de baterías** operando en paralelo con la red. Redacción original: **sin inyección** a la red del Distribuidor. | Enfoque detrás del medidor / autoconsumo. | (a) |
| **Decreto N°147/023** | Regulación de mercado | **Publicado el 29-05-2023.** Modifica el Marco Regulatorio del Sistema Eléctrico Nacional (Decreto 276/002) para permitir que los Suscriptores **inyecten energía a la red**, y su **Artículo 3 modifica expresamente el Decreto 27/020**: la generación a partir de instalación de baterías en paralelo con la Red de Distribución de BT pasa a regirse por el **Artículo 12 Bis**. | **Cambia el régimen de "cero inyección" a inyección acotada.** Ver detalle abajo. | (a) |

### 🔴 Corrección de identificación normativa *(verificado en esta corrida)*

El documento antes referido en este archivo como **"Decreto 2020"** es en realidad el **Decreto N°27/020** (decreto 27 del año 2020). Además, **no está en su redacción original**: fue modificado por el **Decreto N°147/023 (29-05-2023)**.

**Régimen vigente confirmado (a) — fuente: IMPO (Registro Nacional de Leyes y Decretos, Uruguay):**
- **Sin baterías:** la inyección anual del Suscriptor no puede superar su consumo anual.
- **Con instalación de baterías:** la inyección está limitada al **30% del consumo** anual — trato más restrictivo que el de generación sin almacenamiento.
- **Remuneración:** la energía inyectada, hasta el límite aplicable, se paga **al precio spot horario sancionado por ADME**. Los excedentes por sobre el límite se penalizan gradualmente.
- **Nivel de tensión:** Baja Tensión (explícito para baterías).
- **Umbral administrativo:** hasta **150 kW** basta el registro; por encima se requiere autorización ministerial.

**Lectura de esta vigilancia (b):** Uruguay **sí** tiene hoy un régimen de inyección remunerada para almacenamiento detrás del medidor, con techo del 30% del consumo y precio spot — es decir, un marco de autoconsumo con storage, no un mercado de almacenamiento. El techo del 30% y la remuneración a spot acotan estructuralmente el tamaño del segmento C&I con baterías.

### Otros desarrollos *(no regulatorios, contexto de mercado)*
- **(c) Contratación de BESS por UTE — zona Valentines.** En diciembre de 2025 UTE resolvió una **contratación directa** con la constructora Stiler para el **arrendamiento de un sistema de almacenamiento con O&M por 15 años**, por un monto del orden de **USD 63 millones**, para resolver problemas de calidad de servicio, tensión y racionamiento en la zona de Valentines. La modalidad (contratación directa, tras una licitación previa fallida en San Gregorio de Polanco) generó cuestionamientos del sector privado. **Es una decisión de compra de la utility, no un marco regulatorio ni una licitación abierta de almacenamiento.** No verificado contra resolución oficial de UTE en esta corrida.

### Nota de estructura
Marco de storage **marcadamente menos desarrollado** que los otros cuatro mercados: **no existe ley, licitación ni mandato de almacenamiento stand-alone a escala de red** equivalente a AlmaSADI (Argentina), Producto 3 de la CLPE (Colombia) o el AT IBR (Chile). El único marco con reglas claras es el de autoconsumo en BT (Decretos 27/020 + 147/023). **Prioridad de vigilancia: detectar si UTE/ADME/MIEM estructuran una licitación o un marco de almacenamiento a escala de red.**

---

## Registro de verificación de esta corrida (2026-08-13)

**Fuentes primarias / oficiales consultadas:**
- Chile: `cne.cl` — texto del AT IBR aprobado por REx CNE N°45/2026; compendio ACERA "Grid-Forming en Chile" (mayo 2026); comunicados CNE sobre Bases Definitivas Licitación 2026/01; comunicado MMA sobre REx N°4225/2026 (Ley REP baterías).
- Argentina: `argentina.gob.ar` (comunicado de adjudicación AlmaSADI, 7-jul-2026); Res. SE N°50/2026 (BO 2-mar-2026) y Res. SE N°155/2026 (BO 7-jul-2026).
- Colombia: `creg.gov.co` y gestor normativo CREG (Res. 101 113 de 2026, 19-jun-2026); Decreto 0393 de 2026 (10-abr-2026); informe de cierre CLPE de la Bolsa Mercantil de Colombia.
- Perú: `busquedas.elperuano.pe` (RM N°171-2026-MINEM/DM); portal de normas legales del MINEM.
- Uruguay: `impo.com.uy` — Decreto N°147/023 y su modificación al Decreto N°27/020.

**No verificado en esta corrida (conserva estatus seed):** el listado completo de normas chilenas previas a 2026 (LGSE, Leyes 20.936 / 21.505 / 21.721, DS 62/70/125/37/88/148/8, MINVU 522, REx 41-2025), las normas argentinas anteriores a AlmaSADI, las normas colombianas anteriores al Decreto 1091/2025, y el marco peruano previo a la Ley 32249.
