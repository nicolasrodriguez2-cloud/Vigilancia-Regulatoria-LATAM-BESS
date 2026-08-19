# Panorama Regulatorio BESS — LATAM

> **Última corrida de vigilancia:** 2026-08-13 (primera corrida real del agente de Vigilancia Regulatoria).
>
> **Origen histórico:** este archivo nació como seed extraído de `BESS_POTENTIAL_CLIENTS_v2.xlsx` (corte 2026-08-12). La corrida del 2026-08-13 validó los ítems críticos contra fuente oficial y corrigió los que estaban mal. Los ítems que **no** fueron validados individualmente en esta corrida conservan su estatus de seed y están marcados como tales.

### Convención de clasificación de fuente
Cada afirmación relevante lleva una de estas marcas:

- **(a)** — texto o resolución oficial confirmada contra la fuente primaria.
- **(b)** — interpretación o análisis de esta vigilancia.
- **(c)** — anuncio, borrador, proyecto o reporte de prensa aún **no** oficializado o no verificado contra fuente primaria.
- **(seed)** — heredado del archivo de mercado interno, todavía sin validar por esta vigilancia.

---

## Chile

### Reguladores / instituciones
- **Ministerio de Energía** — máxima autoridad ejecutiva: política energética nacional, planificación estratégica, decretos que regulan generación, transmisión, distribución y almacenamiento.
- **CNE — Comisión Nacional de Energía** — cuerpo técnico asesor: normas regulatorias, precios regulados (precio nudo, semestral), metodologías de servicios complementarios y almacenamiento.
- **CEN — Coordinador Eléctrico Nacional** — operador del sistema: despacho en tiempo real, costo marginal, liquidaciones económicas, aprobación de acceso a la red para proyectos nuevos incluyendo BESS. Emite las guías de verificación técnica derivadas de la NTSyCS.
- **SEC — Superintendencia de Electricidad y Combustibles** — fiscaliza cumplimiento de la ley eléctrica, otorga concesiones, autoriza conexión física de instalaciones de generación y almacenamiento.
- **Panel de Expertos** — cuerpo colegiado independiente, resuelve disputas técnicas y tarifarias vinculantes (peajes de transmisión, costos de servicios complementarios).
- **Ministerio del Medio Ambiente / SEA** — administra el SEIA; todo proyecto de generación o almacenamiento sobre umbral definido requiere Resolución de Calificación Ambiental (RCA).

### Jerarquía documental aplicable a requisitos IBR/GFM — **corregido 2026-08-13**

**(a)** La **NTSyCS (Norma Técnica de Seguridad y Calidad de Servicio) es la norma primaria.** El **AT-IBR es un Anexo Técnico *de* la NTSyCS**, no un instrumento paralelo ni sustituto. El propio Artículo 1-1 del Anexo lo dice de forma literal:

> *"El Anexo Técnico tiene por objeto establecer las exigencias técnicas mínimas **complementarias a las establecidas en la Norma Técnica de Seguridad y Calidad de Servicio**, para las Instalaciones Basadas en Convertidores…"*

Ambos textos —la NTSyCS modificada y el AT-IBR— fueron aprobados por **la misma resolución: REx CNE N°45, de 28 de enero de 2026** (documentos fechados "Enero de 2026"; publicación en Diario Oficial: **3 de febrero de 2026** según registro BCN Ley Chile).

> ⚠️ **Corrección respecto del seed.** El seed afirmaba que el AT-IBR era "norma primaria para requisitos IBR/GFM — no está en la NTSyCS" y lo fechaba en marzo de 2026. **Ambas afirmaciones son incorrectas.** Al citar requisitos IBR/GFM en Chile, la referencia correcta es: *NTSyCS (norma primaria) → Anexo Técnico AT-IBR (exigencias mínimas complementarias)*, ambos aprobados por REx CNE N°45/2026.

> ⚠️ **Dato a confirmar:** una fuente secundaria (newsletter Garrigues, jul-2026) fecha la REx N°45 el **28 de febrero de 2026** y le atribuye además la aprobación de la Norma Técnica de Servicios Complementarios. El nombre de archivo oficial de la CNE (`2026.01.28_AT-IBR_RES45.pdf`) y el encabezado del documento ("Enero de 2026") apuntan al **28 de enero de 2026**. Se adopta la fecha del documento oficial; el desfase queda señalizado.

### **GFM es obligatorio para todo BESS que se interconecte al SEN — corregido 2026-08-13**

**(a)** **Artículo 3-12 del AT-IBR**, texto literal:

> *"Todo Sistema de Almacenamiento de Energía o componente de almacenamiento de una CRCA que se interconecten al SEN deberá cumplir con ser una IBR GFM."*

El mismo artículo faculta al Coordinador, a partir de los resultados del **Estudio de Análisis de Robustez del SEN**, a instruir el cambio de modo de operación entre IBR GFM e IBR GFL, con plazo de implementación definido; esa modificación se limita a ajustes de software y adecuaciones de comunicaciones.

> ⚠️ **Corrección respecto del seed.** El seed decía "GFM no obligatorio aún, pero referenciado explícitamente". **Es obligatorio.** Aplica a SAE stand-alone y a la componente de almacenamiento de una CRCA. **(b)** En la práctica esto significa que en Chile ya no hay ruta de conexión al sistema de transmisión del SEN para un BESS grid-following puro: el requisito GFM pasó de diferenciador comercial a condición de entrada.

#### Exigencias mínimas para IBR GFM (Título 3 del AT-IBR) — **(a)**
El Título 3 impone, entre otros: Controlador de Tensión autónomo (Art. 3-2 a 3-4), control de inyección rápida de corriente (3-5), Controlador Frecuencia/Potencia (3-6), respuesta inercial (3-7), control activo de salto de fase (3-8), control de amortiguamiento de potencia (3-9), capacidad de operar en Isla Eléctrica (3-10) y capacidad de Partida Autónoma / black start (3-11).

Parámetros de desempeño del Controlador de Tensión en operación normal (Art. 3-3): Tiempo de Reacción < 200 ms; Tiempo de Crecimiento < 1 s; Tiempo de Establecimiento < 5 s; Banda de Establecimiento < ±5%; sobreoscilación ≤ 5%; Estatismo Permanente ajustable entre 2% y 10%.

#### Régimen transitorio (Título 7 del AT-IBR) — **(a)**
Todos los plazos corren desde la **publicación en el Diario Oficial de la resolución que aprueba el Anexo** (3-feb-2026 según BCN; fechas derivadas marcadas como estimadas):

| Art. | Disposición | Plazo | Fecha estimada |
|---|---|---|---|
| 7-1 | Entrada en vigencia del Anexo | desde publicación en DO | 3-feb-2026 |
| 7-1 | Exigencias GFM (Títulos 3, 5 y 6) **no aplican** a instalaciones con Entrada en Operación dentro de los 6 meses siguientes a la publicación, ni a las declaradas en construcción antes de la publicación (sujeto a Art. 7-2) | 6 meses | ~3-ago-2026 (vencido) |
| 7-2 | SAE / componente de almacenamiento de CRCA declarados en construcción antes de la publicación pero con Entrada en Operación posterior a los 6 meses: **sí deben cumplir el Título 3**. Podían solicitar exención justificada a la Comisión con estudio técnico | 5 meses para solicitar exención | ~3-jul-2026 (**vencido**) |
| 7-4 | El Coordinador debe definir cronograma de entrega de modelos EMT; el cronograma no puede extenderse más de 1 año desde su emisión. Validación por el Coordinador: ≤45 días hábiles desde recepción | 3 meses para definir cronograma | ~3-may-2026 |
| 7-5 | Titulares de IBR GFL conectadas al SEN (y las declaradas en construcción a la fecha de publicación) deben presentar al Coordinador un **plan de adecuaciones**. En el mismo plazo, los titulares de SAE / componente de almacenamiento de CRCA deben **informar la factibilidad de actualizar sus sistemas para operar como IBR GFM** | 9 meses | ~3-nov-2026 (**vigente — acción pendiente**) |
| 7-5 | Coordinador publica cronograma de adecuaciones dentro de los 6 meses siguientes al vencimiento del plazo anterior; ejecución máxima 24 meses desde publicación del cronograma | — | — |
| 7-6 | Mientras el Anexo Técnico "Información Técnica de Instalaciones y Equipamiento" no incorpore los antecedentes exigibles a IBR GFM, se debe entregar al Coordinador, **previo a entrada en operación**, un paquete de 19 ítems: diagrama de impedancia vs. frecuencia, diagrama de Nichols, arquitectura y diagrama de bloques en Laplace, documentación del modelo EMT, tipo de IBR GFM (UGBC, SAE, compensación dinámica reactiva, CRCA), límites y potencia por salto de fase, potencia de amortiguamiento activa, constante de inercia H y constante de inercia efectiva He, capacidad de sobrecorriente, aportes de cortocircuito trifásico/monofásico, corriente de secuencia negativa, Factor Equivalente de Amortiguamiento (z), entre otros | previo a EO | — |

#### Guía de verificación GFM del Coordinador (mayo 2026) — **(a)**
El CEN publicó en **mayo de 2026** la *Guía para la Verificación de Instalaciones Grid-Forming (IBR GFM)*, en el marco del AT-IBR y conforme al **Oficio ORD CNE N°337/2026**. Estructura la verificación en **tres etapas**: (1) validación de modelos y ensayos Hardware-in-the-Loop (HIL); (2) verificación en terreno durante la puesta en servicio; (3) monitoreo continuo durante la operación.

**(b)** Para un proyecto BESS esto define la ruta de cumplimiento completa: no basta la declaración del OEM — hay que producir modelos EMT validados, pasar HIL, verificación en terreno y quedar sujeto a monitoreo permanente. Es un requisito que debe estar en el alcance del suministrador desde la etapa de oferta.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Clasif. |
|---|---|---|---|---|
| Ley General de Servicios Eléctricos (LGSE) | Regulación de mercado | Marco original de generación/transmisión/distribución, sin almacenamiento contemplado originalmente. | Norma base; toda regulación de storage posterior es una modificación de esta ley. | seed |
| Ley N°20.936 | Regulación de mercado | Primera ley en reconocer formalmente la existencia de sistemas de almacenamiento. Define SAE (Sistema de Almacenamiento de Energía) y CRCA. | Introduce categorías legales SAE/CRCA; storage reconocido pero sin mecanismo de pago definido. | seed |
| Ley N°21.505 | Regulación de mercado | Permite a sistemas de batería stand-alone (SAE) vender energía y recibir pagos por potencia de suficiencia en el mercado mayorista. | SAE stand-alone puede vender en el mercado spot y acceder a potencia de suficiencia. | seed |
| DS N°62 | Regulación de mercado | Rige pagos por potencia (suficiencia) para todos los generadores. | Pagos basados en contribución de confiabilidad en punta; tecnología de referencia: diésel. | seed |
| DS N°70 | Regulación de mercado | Modifica DS 62 y DS 125 para que baterías stand-alone reciban pagos por potencia — fórmula: a mayor duración de descarga, mayor crédito de capacidad (vigente 10 años). | Tabla de reconocimiento por duración, aplica a SAE y CRCA. | seed |
| Ley N°21.721 | Transmisión | Ataca cuellos de botella de transmisión que bloquean renovables. Beneficia indirectamente al almacenamiento. | Acelera permisos de nuevas líneas; complemento estratégico de la Ley 21.505. | seed |
| DS N°125 | Regulación de mercado | SAE puede proveer Servicios Complementarios; actualiza reglas de despacho económico para incluir BESS explícitamente en coordinación en tiempo real y formación de precios. | Habilita pago formal por servicios complementarios. | seed |
| DS N°37 | Transmisión | Regula planificación, construcción y operación del sistema de transmisión; conecta SAE a la planificación de transmisión. | CEN puede co-optimizar formalmente storage y transmisión. | seed |
| MINVU 522 | Planificación urbana | Regulación urbana aplicable a sistemas de almacenamiento. | Clasifica BESS stand-alone como "Infraestructura Energética" (Art. 2.1.29 OGUC); requiere permiso de edificación, no concesión. | seed |
| Ley N°20.920 (REP) | Responsabilidad extendida del productor | Responsabiliza a productores/importadores por recolección y reciclaje de productos prioritarios, incluidas baterías. | Baterías industriales BESS ≥5 kg listadas como producto prioritario; fiscalizada por SMA. | seed |
| DS 88 | Regulación de mercado | Actualiza régimen PMGD para permitir que BESS bajo 9 MW use margen de capacidad de red disponible para carga. | Nueva vía de ingreso para BESS comercial/industrial distribuido hasta 9 MW. | seed |
| **NTSyCS** (modificada por REx CNE N°45, 28-ene-2026) | Seguridad / código de red | Requisitos de seguridad y calidad para instalaciones del SEN, incluyendo BESS. **Norma primaria** de la que cuelga el AT-IBR. | Norma de referencia jerárquicamente superior en materia IBR/GFM. | **(a)** |
| **AT-IBR — Anexo Técnico de Exigencias Mínimas de Instalaciones Basadas en Convertidores** (aprobado por REx CNE N°45, 28-ene-2026; DO 3-feb-2026) | Código de red — anexo de la NTSyCS | Exigencias mínimas **complementarias** a la NTSyCS para IBR GFM y GFL. Aplica a IBR interconectadas o a interconectarse al **Sistema de Transmisión** del SEN. | **Art. 3-12: GFM obligatorio para todo SAE y para la componente de almacenamiento de CRCA que se interconecte al SEN.** Régimen transitorio en Título 7. | **(a)** |
| REx CNE N°41-2025 | Seguridad | Primera regulación con requisitos sísmicos específicos para BESS e instalaciones eléctricas de alta tensión. | Referencia NCh 2369:2023 e IEEE 693:2018; obligatorio para permisos e ingeniería de proyectos BESS nuevos. | seed |
| DS N°148 | Seguridad | Manejo, transporte y disposición de residuos peligrosos, incluidos componentes de baterías de litio. | Baterías de litio clasificadas como residuo peligroso en operación y desmantelamiento. | seed |
| DS N°8 | Seguridad | Diseño, construcción y operación de instalaciones eléctricas de consumo. | Fichas técnicas RIC. | seed |

### Licitación de Suministro 2026/01 — **(a)**, actualizado 2026-08-13
- Bases preliminares aprobadas por **REx CNE N°292** (junio 2026); **bases definitivas publicadas el 20 de julio de 2026**, con inicio formal del proceso.
- Volumen: **2.835 GWh** en dos bloques, distribuidos en **4 zonas** y **3 bandas horarias**. Bloque 1: 1-ene-2029 a 31-dic-2043. Bloque 2: 1-ene-2030 a 31-dic-2044.
- **Sin carbón ni diésel** como tecnologías de respaldo admisibles.
- **Reconocimiento explícito del almacenamiento**: las bases reconocen los sistemas de almacenamiento como activos válidos para respaldar obligaciones de suministro, permitiendo al oferente acreditar sistemas existentes o proyectados, siempre que estén interconectados al SEN y su capacidad de inyección anual sea suficiente para cubrir el volumen comprometido.
- Cronograma: cierre del período de consultas **28-ago-2026**; publicación de respuestas y modificaciones finales **2-oct-2026**; recepción de ofertas **4-dic-2026**; **adjudicación prevista enero 2027**.

### Políticas públicas relevantes
- **Plan Nacional de Almacenamiento — Terrenos Fiscales** (seed): arriendo directo en terrenos fiscales del Norte Grande (Tarapacá, Antofagasta, Atacama). Concesión directa, sin licitación pública.
- **Segunda Fase de la Agenda de Transición Energética** (seed): storage como pilar explícito.
- **Estudio de Almacenamiento CEN (2023)** (seed): capacidad óptima 1.000–4.000 MW (2026–2032), duración óptima 6–8 h, almacenamiento diario óptimo 13,2 GWh.
- **Propuesta de nuevos Servicios Complementarios** — Minuta Técnica CEN SSE-26002 (mayo 2026). **(c)** propuesta del Coordinador, no norma vigente. A monitorear.

### Nota de estructura — **actualizada 2026-08-13**
Las licitaciones de suministro chilenas siguen contratando **energía** (GWh/año), no capacidad de almacenamiento. El BESS entra por lógica de mercado e incentivos, no por mandato de contratación. **Matiz nuevo (b):** la Licitación 2026/01 sí reconoce formalmente al almacenamiento como activo acreditable de respaldo de la obligación de suministro — sigue sin ser un mandato de storage, pero ya no es sólo lógica de mercado indirecta. En paralelo, por la vía **técnica** (AT-IBR Art. 3-12) Chile sí impone un mandato: GFM obligatorio para todo BESS que se conecte.

---

## Argentina

### Reguladores / instituciones
- **Secretaría de Energía (SE)** — autoridad de política principal, emite resoluciones que rigen el MEM; convocó AlmaGBA y AlmaSADI.
- **CFEE — Consejo Federal de la Energía Eléctrica** — consejo asesor a gobiernos nacional y provinciales; administra el FNEE.
- **CAMMESA** — nodo operativo central del mercado: despacho técnico-económico del SADI, cálculo de precios spot, administración del mercado a término. En AlmaSADI actúa como **offtaker directo**.
- **Ente Nacional Regulador del Gas y la Electricidad** (fusión 2025 de ENRE + ENARGAS, Decreto 452/2025) — regula generación, transmisión y distribución federal; autoriza el punto de acceso a la red de cada proyecto de storage nuevo.
- **EDENOR / EDESUR** — distribuidoras federales, compradoras directas de capacidad BESS vía AlmaGBA.
- **Transener** — principal transportista de alta tensión (troncal 500 kV).

### **AlmaSADI adjudicada — Res. SE N°155/2026 — (a), novedad 2026-08-13**

| Ítem | Dato |
|---|---|
| Norma de adjudicación | **Resolución SE N°155/2026** (Resol-2026-155-APN-SE#MEC), Boletín Oficial **7-jul-2026** |
| Convocatoria original | Res. SE N°50/2026, Boletín Oficial 2-mar-2026 |
| Meta convocada | hasta 700 MW |
| **Adjudicado** | **700,5 MW en 20 proyectos** |
| Ofertas recibidas | 235 ofertas técnicas por **8.338 MW** (27-may-2026) — sobresuscripción ~11,9x |
| Adjudicatarios | Genneia (7 proyectos), DQD Energy (8), 360 Energy Solar (3), Aluar (1), Intermepro (1) |
| Inversión estimada | ~USD 700 millones |
| **Precio promedio de adjudicación** | **USD 8.427 /MW-mes** |
| Plazo de los Acuerdos de Almacenamiento | **15 años** ⚠️ ver ambigüedad abajo |
| Offtaker | CAMMESA (compra directa, no sólo garante) |
| Remuneración | centrada en **disponibilidad de potencia** |

**Distribución regional adjudicada (a):** Buenos Aires 185 MW · NOA 150 MW · NEA Chaco-Formosa 161,5 MW · NEA Misiones-Corrientes 50 MW · Litoral Entre Ríos 50 MW · Litoral Santa Fe 36 MW · Pampa 68 MW.

> ⚠️ **Correcciones respecto del seed:**
> - Fecha de adjudicación: **7-jul-2026** (no 19-jun-2026, que era la fecha *prevista* en el cronograma original).
> - Plazo de contrato: las fuentes de prensa especializada convergen en **15 años**, no 10 como registraba el seed.
> - Cupos regionales adjudicados difieren de la lista de zonas convocadas del seed (que incluía "Centro" y "Cuyo" y no desagregaba NEA ni Litoral).

> ⚠️ **Pendiente de verificación (c):** no se pudo acceder al texto íntegro de la Res. 155/2026 en el Boletín Oficial (servidor devolvió HTTP 503) ni al pliego de la Res. 50/2026. El plazo contractual de 15 años, el precio promedio USD 8.427/MW-mes y la duración mínima de descarga exigida (HAC) provienen de prensa especializada, no del texto oficial. **Confirmar contra el texto de la resolución antes de usar como dato firme en oferta.**

**(b)** Referencia comparativa: el techo de AlmaGBA fue USD 12.500/MW-mes. El promedio de AlmaSADI (USD 8.427/MW-mes) implica una caída del orden del 33% en el precio de capacidad entre la primera y la segunda generación de licitaciones argentinas de storage. Con 11,9x de sobresuscripción, la presión competitiva sobre el CAPEX de BESS en Argentina es alta y previsiblemente seguirá.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Clasif. |
|---|---|---|---|---|
| Ley N°15.336 | Marco general | Ley fundacional del sector eléctrico argentino; jurisdicción federal sobre electricidad interprovincial vía SADI. | Autoriza a la SE a regular el MEM y emitir resoluciones como AlmaGBA/AlmaSADI. | seed |
| Ley N°24.065 | Mercado mayorista | Crea el mercado mayorista competitivo. Decreto 450/2025 restauró principios marginalistas. | Toda resolución BESS cita esta ley como base legal. | seed |
| Ley N°27.742 (Ley Bases) | Inversión privada | Delegó al Ejecutivo la actualización del marco regulatorio eléctrico por decreto. | Habilitó el Decreto 450/2025 y la Res. 400/2025. | seed |
| Ley N°26.190 y N°27.191 | Renovables / grandes usuarios | Meta obligatoria de 20% renovables al 31-dic-2025 para consumidores ≥300 kW. | Demanda cautiva MATER; proyectos híbridos BESS acceden a estos beneficios. | seed |
| SE Res. N°36/2023 y N°906/2023 (RenMDI / ALMA MDI) | Renovables / BESS híbrido | Primera apertura formal a proyectos renovables con storage. 633,7 MW adjudicados en 98 proyectos. | Primer marco contractual que exige datos técnicos de BESS. | seed |
| **SE Res. N°67/2025 — AlmaGBA** | Storage stand-alone | Primera licitación exclusiva para storage stand-alone a gran escala. 713 MW adjudicados en agosto 2025. | Define el modelo "Storage Generation Contract". Duración mínima de descarga: 4 h (HAC). Compradores: EDENOR/EDESUR. | seed |
| SE Res. N°344, 361, 384/2025 | Storage stand-alone | Formalizan adjudicación de los 713 MW de AlmaGBA. | Pago por capacidad hasta USD 12.500/MW/mes; energía USD 10/MWh fijo hasta 2037. | seed |
| **SE Res. N°50/2026 — AlmaSADI (convocatoria)** | Storage stand-alone | Convocatoria nacional e internacional abierta para abastecimiento por centrales de almacenamiento para reserva y confiabilidad en el MEM. BO 2-mar-2026. | Segunda generación de licitaciones BESS, escala nacional (todo el SADI). CAMMESA compra directo. | **(a)** |
| **SE Res. N°155/2026 — AlmaSADI (adjudicación)** | Storage stand-alone | **Adjudica 700,5 MW en 20 proyectos.** BO 7-jul-2026. Instruye a CAMMESA notificar adjudicatarios y firmar los Acuerdos de Almacenamiento. | Cierra el ciclo AlmaSADI. Precio promedio USD 8.427/MW-mes. | **(a)** |
| SE Res. N°400/2025 — Normalización MEM | Reforma MEM | Vigente desde 1-nov-2025. Redefine categorías de generador; crea Mercado a Término de Energía y Capacidad. | BESS de AlmaGBA/AlmaSADI califican como "Nueva Generación". | seed |
| Decreto N°450/2025 | Reforma estructural | Actualiza texto de Ley 24.065; restaura principios marginalistas; período de transición de 24 meses (hasta jul-2027). | Nuevo Art. 9°: distribuidoras deben contratar ≥75% de su demanda vía contratos de largo plazo. | seed |
| Decreto 513/2025 | Incentivo fiscal | Reduce arancel de importación de sistemas de batería de litio a 12,6%. | Reduce costo de importación de BESS. | seed |
| RIGI — Ley 27.742, Título VII | Incentivo de inversión | Régimen para proyectos >USD 200M en sectores estratégicos incluida energía; estabilidad fiscal y regulatoria de 30 años. | Clusters BESS grandes o renovable+storage >USD 200M pueden calificar. | seed |

### Políticas públicas relevantes
- **RENPALMA** (seed) — Registro Nacional de Proyectos de Almacenamiento.
- **Plan de Contingencia de la Secretaría de Energía** **(a)** — AlmaSADI se enmarca formalmente en este plan, orientado a reducir cortes en períodos de mayor consumo mediante reserva y confiabilidad de corto plazo.

### Nota de estructura
AlmaSADI contrata directamente **capacidad de almacenamiento (MW/MWh) stand-alone**, a diferencia de Chile. Con AlmaSADI adjudicada, Argentina acumula ~1.413,5 MW de storage stand-alone contratado (713 MW AlmaGBA + 700,5 MW AlmaSADI). **(b)** El próximo hito a vigilar es si aparece una tercera convocatoria o si el mecanismo migra al Mercado a Término de Energía y Capacidad creado por la Res. 400/2025.

---

## Colombia

### Reguladores / instituciones
- **MinMinas y Energía** — define política energética nacional, metas estratégicas, convoca subastas de largo plazo (Res. 40208/2026).
- **CREG** — regula el MEM: precios de bolsa, OEF, SSCC, acceso a la red. Emisora de la Res. CREG 101 113/2026 sobre SAEB.
- **UPME** — planificación energética nacional (PEN 2024–2054); aprueba conexiones de proyectos FNCER y BESS.
- **XM (ISA)** — operador del SIN (CND, despacho en tiempo real) y administrador del mercado (ASIC, liquidación).
- **ANLA / SSPD** — ANLA: licenciamiento ambiental (cuello de botella clave). SSPD: supervisa utilities.
- **BMC — Bolsa Mercantil de Colombia** — operador designado de la subasta de largo plazo 2026; publica el informe oficial de cierre.

### **Res. CREG 101 113 de 2026 — marco definitivo de SAEB — (a), novedad 2026-08-13**

**Título oficial:** *"Por la cual se definen los mecanismos para incorporar sistemas de almacenamiento de energía eléctrica con baterías -SAEB- en el Sistema Interconectado Nacional"*.
**Aprobada en Sesión CREG N°1473 del 19 de junio de 2026.** Publicada en **Diario Oficial N°53.530, lunes 22 de junio de 2026**.

> ⚠️ **Esta resolución es la versión definitiva del Proyecto de Resolución CREG 701-103 de 2025**, que el seed registraba como "en consulta pública". La CREG la expidió tras analizar los comentarios recibidos en la consulta. **Al citar el marco técnico-comercial de BESS en Colombia, la referencia correcta ya no es el proyecto 701-103/2025 sino la Res. CREG 101 113 de 2026.**

**Modalidades de participación (a):**
1. **SAEB como activos de red (Título I)** — conectados al STN, STR o SDL para atender necesidades específicas del sistema. La resolución define cuándo son necesarios, cómo se desarrollan los proyectos, cómo se remuneran, obligaciones de calidad del servicio y manejo de la energía almacenada y entregada.
2. **SAEB independientes (Título II)** — instalaciones de **≥5 MW**, con **dos fronteras comerciales separadas** para carga y descarga.
3. **SAEB como parte de recursos de generación híbridos** — de cualquier capacidad.

**Remuneración (a):**
- STN y STR por procesos de selección → **Ingreso Anual Esperado (IAE)** en pesos constantes.
- STR ejecutado por el OR → metodología de distribución vigente.
- SDL → conforme a la regulación de distribución.

**Servicios comercializables por un SAEB independiente (a):** participación en la bolsa de energía con ofertas de descarga, y **Regulación Secundaria de Frecuencia (AGC)**. Adicionalmente puede entregar energía por condiciones de seguridad.

### **Resultados de la Subasta CLPE-MME 2026 — (a)/(c), novedad 2026-08-13**

Jornadas de subasta: **28 y 29 de julio de 2026**. Informe oficial de cierre publicado por la BMC. Contratos a **15 años**, con obligaciones desde el **1 de enero de 2030**.

| Producto | Resultado | Precio promedio | Adjudicatarios |
|---|---|---|---|
| **Producto 1** | **Cancelado** antes de ejecutarse por competidores insuficientes (mínimo 3 requeridos) | — | — |
| **Producto 2** — solar fotovoltaica | **995 MW / 4.174 MWh-día** | COP 246,13 /kWh | 4 proyectos: Enel Colombia (2), EPM (2), Bosques Solares |
| **Producto 3** — híbrido solar + almacenamiento | **390 MWh-día** ⚠️ | COP 315,87 /kWh | 2 proyectos: Bosques Solares de los Llanos 8 y Parque Solar Andrómeda (Celsia) |
| **Producto 4** — suministro nocturno (18:00–22:00) respaldado por almacenamiento | **Desierto — sin adjudicaciones** | — | — |

**Agregados:** ofertas totales 6.352 MWh-día · demanda agregada de compradores 23.685 MWh-día · adjudicado 4.564 MWh-día. Cuatro vendedores y seis compradores obtuvieron contratos. **Primera incorporación de sistemas de almacenamiento con baterías en las subastas de energía limpia de Colombia.**

> ⚠️ **Conflicto de fuentes señalizado (c).** Existen reportes de prensa contradictorios sobre el Producto 3: una fuente lo reporta como **desierto sin precio de cierre** (ofertas por 558 MWh-día contra demanda de 5.990 MWh-día, adjudicado cero); otra reporta **390 MWh-día adjudicados** a dos proyectos nombrados con precio de cierre. Se adopta la segunda por ser la más detallada y consistente con el agregado de 4.564 MWh-día, pero **el dato debe confirmarse contra el informe de cierre oficial de la BMC antes de usarse como firme**. Algunas fuentes también fechan las jornadas el 23-24 de julio en lugar del 28-29.

> ⚠️ **Corrección respecto del seed:** el seed describía el "Producto 3" como el que "mandata almacenamiento explícitamente". En la estructura real de la subasta, el Producto 3 es **híbrido solar+BESS** y el Producto 4 es **suministro en franja nocturna respaldado por almacenamiento** — y fue el Producto 4, no el 3, el que quedó desierto. La franja horaria del Producto 4 es **18:00–22:00**, no "17–21 h" como registraba el seed.

**(b)** Lectura de mercado: el almacenamiento entró a la subasta pero con una tracción muy por debajo de la demanda declarada (Producto 3 adjudicó 390 de ~5.990 MWh-día demandados; Producto 4 quedó desierto). La señal es que **el precio de cierre disponible no cubrió el costo de un BESS colombiano en las condiciones actuales**. Para un proveedor de BESS esto es relevante en dos direcciones: hay demanda regulatoria insatisfecha, y hay presión estructural sobre el CAPEX para la próxima ronda.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Clasif. |
|---|---|---|---|---|
| Ley 143/1994 | Marco legal sectorial | Crea la CREG; modelo de pool competitivo. | Fundación del modelo de mercado. | seed |
| Ley 1715/2014 | Marco FNCER | Incentivos fiscales para FNCER. Modificada por Ley 2099/2021. | Aplica a BESS acoplado a FNCER. | seed |
| Ley 2099/2021 (Transición Energética) | Marco FNCER | Extiende incentivos a todos los proyectos de energía. Primer reconocimiento legal explícito del almacenamiento en planificación del SIN. | Base legal para storage en la planificación nacional. | seed |
| Res. CREG 071/2006 | Cargo por confiabilidad | Regula OEF, precio de escasez, gatillo de condición crítica. Última modificación: Res. 101 066/2024. | Marco de adecuación de capacidad — vía potencial para BESS. | seed |
| Res. CREG 098/2019 | Storage | Primer reconocimiento regulatorio formal del almacenamiento en el SIN. Habilitó proyectos piloto BESS. | Origen de la regulación colombiana de BESS. ⚠️ ver ambigüedad estructural. | seed |
| Res. CREG 101 066/2024 | Precios de escasez | Diferencia precios de escasez por tipo de planta. | Afecta competitividad de BESS para la Obligación de Confiabilidad. | seed |
| **Decreto 1091/2025** | Contratación de largo plazo | Directrices de política para contratación de largo plazo de generación y storage. | Habilita BESS standalone en subastas de largo plazo. Da 12 meses a la CREG para definir metodología de remuneración BESS. | seed |
| **Res. CREG 101 113 de 2026** | Marco técnico-comercial BESS | **Norma definitiva** que define los mecanismos para incorporar SAEB al SIN. Sesión CREG 1473 del 19-jun-2026; DO 53.530 del 22-jun-2026. Reemplaza operativamente al Proyecto 701-103/2025. | **Marco técnico, comercial y operacional vigente de BESS en Colombia.** Tres modalidades; SAEB independiente ≥5 MW con dos fronteras comerciales; servicios: bolsa de energía y AGC. | **(a)** |
| Res. MinMinas 40178/2026 | Contratación de largo plazo | Reglas generales para contratación de largo plazo de energía limpia. | Marco habilitante previo a la subasta LP. | seed |
| **Res. MinMinas 40208/2026** (21-abr-2026) | Subasta de largo plazo | Convoca y define el mecanismo de contratación de largo plazo de electricidad, en línea con el Decreto 1091/2025. | Primera subasta de largo plazo de Colombia con BESS como producto explícito. **Ejecutada 28-29 jul 2026 — ver resultados arriba.** | **(a)** |

### Políticas públicas relevantes
- **Incentivos activos (proyectos FNCER certificados)** (seed): deducción de renta 50%, exclusión de IVA, arancel cero, depreciación acelerada hasta 33,3%/año — trámite vía UPME + certificación ANLA.

### Nota de estructura
El caso de storage colombiano está enraizado en **riesgo hidrológico** (dependencia de El Niño), a diferencia del vertimiento solar en Chile o del deterioro de transmisión en Argentina. **Actualizada (b):** Colombia ya no depende sólo de la subasta para incorporar BESS — con la Res. CREG 101 113/2026 existe una vía permanente y reglada (SAEB como activo de red, híbrido o independiente) que no requiere ganar una subasta. Esa vía, y no el Producto 3/4, es probablemente el canal más sólido de entrada de BESS en Colombia en el corto plazo.

---

## Perú

### Reguladores / instituciones
- **MINEM — Ministerio de Energía y Minas** — máxima autoridad ejecutiva: políticas energéticas, planificación estratégica, concesiones.
- **OSINERGMIN** — brazo regulatorio bajo MINEM: normas técnicas, revisión de planes de expansión de red, permisos administrativos de conexión. Aprueba los procedimientos técnicos del COES.
- **ProInversión** — administra el Plan Nacional de Electrificación Rural (PNER).
- **COES** — operador independiente del SEIN y cámara de compensación financiera; establece procedimientos técnicos de conexión y penaliza desviaciones de red.

### **Reglamento de Servicios Complementarios — (a)/(c), novedad 2026-08-13**

**Confirmado (a):** el **19 de abril de 2026**, mediante **Resolución Ministerial N°171-2026-MINEM/DM**, el MINEM dispuso la publicación del **proyecto de decreto supremo** que aprueba el **Reglamento de los Servicios Complementarios** y modifica el Reglamento de la Ley de Concesiones Eléctricas, el Reglamento del Mercado Mayorista de Electricidad y el Reglamento del COES. Plazo de comentarios: **25 días calendario**. El MINEM realizó además un taller sobre el proyecto en mayo de 2026.

**Contenido reportado (c) — 7 títulos y 44 artículos.** Disposiciones relevantes para BESS:
- Define los servicios complementarios como *"aquellos necesarios para asegurar el transporte y suministro de electricidad desde la generación hasta la demanda"*.
- Incorpora definiciones de **desempeño, disponibilidad, medición y esquemas de verificación**.
- **Exime a los proveedores de almacenamiento del pago de peajes de transmisión y distribución** por los retiros de energía destinados a servicios complementarios.
- **Excluye al almacenamiento de las obligaciones de pago por potencia**, incluso en horas de máxima demanda.
- Plazos de implementación: **MINEM 120 días** para adecuar las normas técnicas de operación en tiempo real; **COES 180 días** para presentar los procedimientos técnicos a OSINERGMIN.

> ⚠️ **AMBIGÜEDAD — REQUIERE DECISIÓN HUMANA.** Las fuentes están en conflicto sobre el **estatus** de este reglamento:
> - Fuentes que reportan la **publicación del proyecto** para comentarios (RM 171-2026-MINEM/DM, 19-abr-2026) — consistente entre sí y con la práctica normativa peruana.
> - Prensa especializada (jul-2026) titula que *"Perú publica uno de los reglamentos de la Ley 32249 tras más de un año de espera"*, describiendo su contenido en términos de norma vigente y con plazos de implementación corriendo.
> - **Infobae, 16-jul-2026**: reporta que la falta de reglamento de la Ley 32249 **mantiene frenada su aplicación** y que el reglamento **sigue pendiente**.
>
> **No se pudo confirmar la publicación de un Decreto Supremo aprobatorio en El Peruano.** Hasta que se confirme, el estatus operativo es: **proyecto publicado, aprobación no confirmada.** El business case de BESS standalone en Perú sigue dependiendo de esta pieza.

### **Inercia sintética: parámetros técnicos aprobados — (a), novedad 2026-08-13**
**OSINERGMIN, Resolución de Consejo Directivo N°176-2025-OS/CD, del 18 de diciembre de 2025**, aprueba los **parámetros técnicos para el aporte de inercia sintética en la generación eléctrica**.

**(b)** Esto cierra parcialmente la brecha del mandato técnico peruano: hasta ahora existía la obligación (inercia sintética desde el 1-ene-2028) pero sin parámetros verificables. Ya hay parámetros. **La remuneración sigue sin definirse** y depende del Reglamento de Servicios Complementarios — la brecha central del mercado peruano se mantiene, pero se estrechó.

### **Corrección de nomenclatura: el "PR-20" fue desagregado — (a)**
El antiguo **PR-20** ("Ingreso, Modificación y Retiro de Instalaciones en el SEIN", aprobado por Res. OSINERGMIN N°173-2024-OS/CD del 8-oct-2024, con antecedente en la Res. N°035-2013-OS/CD) fue **reestructurado por el COES en procedimientos separados**:
- Estudios de Pre Operatividad
- Estudios de Operatividad
- Integración de Instalaciones al SEIN
- Operación Comercial de unidades o centrales de generación
- Conclusión de Operación Comercial y Retiro

Régimen transitorio: los procesos iniciados antes de la modificación se rigen hasta su conclusión por el PR-20 aprobado por Res. N°035-2013-OS/CD (Res. OSINERGMIN N°083-2021-OS/CD, 30-abr-2021).

> ⚠️ **Citar "PR20" a secas ya no es preciso.** Para requisitos de conexión de un BESS en Perú hay que identificar el procedimiento específico aplicable según la etapa (pre-operatividad, operatividad, integración, operación comercial).

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Clasif. |
|---|---|---|---|---|
| D.Leg. 25844 — Ley de Concesiones Eléctricas | Marco legal | Fundamento del modelo mixto peruano. | Base legal del SEIN. No contempla almacenamiento. | seed |
| D.S. 009-93-EM — Reglamento LCE | Regulación de mercado | Reglas operativas del mercado: despacho por mérito, tarifas, obligaciones de agentes. | Sin mención de almacenamiento. Sería modificado por el proyecto de Reglamento de SSCC. | seed |
| Ley 28832 — Desarrollo Eficiente de la Generación | Regulación de mercado | Introduce licitaciones de energía, mecanismo OEF. | Marco de licitaciones que la Ley 32249 modifica para habilitar BESS. | seed |
| Res. OS 224-2021 (OSINERGMIN) | Regulación de mercado | Modifica el procedimiento del COES para cálculo de costos variables. | Mejoró la señal de precio spot → mayor spread potencial para arbitraje en estiaje. | seed |
| RM 278-2023-MINEM — Hoja de Ruta Smart Grids | Política pública | Estrategia nacional de redes inteligentes 2023–2030. | Primera mención explícita de BESS en política pública. | seed |
| **Ley 32249** — Modificación Ley 28832 | Regulación de mercado | Publicada enero 2025. Crea la figura del Proveedor de Servicios Complementarios (PSC). Habilita PPAs sin respaldo de potencia. Vigente desde 1-ene-2026. | Marco legal que reconoce BESS standalone como PSC. **Su aplicación efectiva está frenada por la falta de reglamento.** | **(a)** |
| **Res. OSINERGMIN N°176-2025-OS/CD** (18-dic-2025) | Requisito técnico | Aprueba los parámetros técnicos para el aporte de inercia sintética en la generación eléctrica. | Hace verificable la obligación de inercia sintética. Tecnologías habilitadas: inversores grid-forming con BESS, supercapacitores u otros. | **(a)** |
| **Obligación de inercia sintética** (ex-PR20, hoy procedimientos COES desagregados) | Requisito técnico | Toda central que inicie operación comercial **desde el 1-ene-2028** debe aportar inercia sintética al SEIN. | Mandato técnico que empuja BESS/GFM en toda generadora nueva. **Sin remuneración definida.** | **(a)** |
| **Proyecto de Reglamento de Servicios Complementarios** (RM N°171-2026-MINEM/DM, 19-abr-2026) | Pendiente / en trámite | Proyecto de DS que aprueba el Reglamento de SSCC y modifica los reglamentos de la LCE, del Mercado Mayorista y del COES. 7 títulos, 44 artículos. | **Pieza regulatoria más crítica pendiente.** Exención de peajes y exclusión de pago por potencia para almacenamiento. ⚠️ Estatus de aprobación no confirmado. | **(a)** proyecto / **(c)** estatus |
| Reglamentación de generación distribuida | Pendiente | Marco para generación descentralizada, prosumidores y BESS behind-the-meter a escala comercial. | Su ausencia bloquea desarrollo C&I y electrificación rural con almacenamiento. | seed |

### Nota de estructura — actualizada 2026-08-13
El **mandato técnico va por delante de la remuneración** — sigue siendo la brecha regulatoria más relevante de este mercado. **Matiz nuevo (b):** en 2026 la brecha se estrechó por el lado técnico (parámetros de inercia sintética aprobados, Res. 176-2025-OS/CD) pero **no** por el lado económico (Reglamento de SSCC sin aprobación confirmada). Un proyecto BESS standalone en Perú sigue sin flujo de ingresos reglado.

---

## Uruguay

### Reguladores / instituciones
- **MIEM — Ministerio de Industria, Energía y Minería** — autoridad de política energética nacional. Dirección Nacional de Energía impulsa la revisión de la normativa de almacenamiento.
- **URSEA — Unidad Reguladora de Servicios de Energía y Agua** — regulación técnica y tarifaria; dicta reglamentos de seguridad de productos eléctricos de baja tensión, incluidas especificaciones para sistemas de almacenamiento con baterías asociados a instalaciones de autoconsumo.
- **UTE — Administración Nacional de Usinas y Trasmisiones Eléctricas** — utility estatal; aprueba instalaciones de storage de sus clientes. Reglamento de Baja Tensión, Capítulo XXIX (instalaciones para autoconsumo).
- **ADME — Administración del Mercado Eléctrico** — administrador/despachador del mercado eléctrico mayorista.
- **Ministerio de Ambiente** — competente en gestión de residuos de baterías (Decreto 227/025).

### **Corrección de nomenclatura: el decreto es el N° 27/020 — (a), 2026-08-13**

> ⚠️ El instrumento que el seed llamaba genéricamente **"Decreto 2020"** es el **Decreto N° 27/020** (Decreto 27 del año 2020). Habilita a usuarios conectados a **redes de distribución de baja tensión** a generar energía eléctrica mediante instalaciones de baterías operando **en paralelo, sin inyectar energía a la red del distribuidor** (régimen de inyección cero). Enfoque detrás del medidor / autoconsumo.

### **Revisión anunciada del Decreto N° 27/020 — (c)**
El MIEM (Dirección Nacional de Energía) ha anunciado que **modificará el Decreto N° 27/020 para permitir la inyección de las baterías a la red**, bajo el criterio de que la inyección **nunca supere el consumo del usuario final**. La motivación declarada es que el requisito de inyección cero impone obstáculos técnicos: obliga al consumidor a instalar equipamiento sofisticado para impedir la inyección y al distribuidor a instalar equipamiento para detectarla.

> ⚠️ **Clasificación (c) — anuncio, no norma.** No hay texto oficial publicado ni proceso de consulta pública confirmado a la fecha de esta corrida. **No usar como dato firme.** Es la novedad de mayor potencial estructural en Uruguay y debe seguirse en cada corrida.

### **Decreto N° 227/025 — gestión de baterías al final de su vida útil — (a), novedad 2026-08-13**

Nuevo marco regulatorio integral para la gestión, reciclaje y disposición de baterías usadas o a ser desechadas y sus componentes. Emitido por el **Ministerio de Ambiente** junto con otros ministerios; publicado en **noviembre de 2025** (fuentes discrepan en el día exacto — dato a confirmar).

**Alcance — incluye explícitamente BESS estacionario:** baterías de todo tipo y tamaño utilizadas en vehículos terrestres, marítimos y aéreos y maquinaria agrícola **de más de 1 kW**, así como **baterías utilizadas en sistemas de almacenamiento estacionario de energía cuya capacidad supere los 2 kWh**.

**Obligaciones para productores e importadores (a):**
1. Contar con **planes maestros** aprobados por el Ministerio de Ambiente.
2. Inscribirse en el **registro nacional** con información actualizada.
3. Implementar un **sistema de etiquetado e información digital** que garantice la **trazabilidad durante todo el ciclo de vida**.
4. Cumplir **metas anuales de recuperación y valorización**.
5. Presentar **informes anuales auditados**.

**Plazos:** 9 meses para presentar planes maestros; 2 años para la adecuación total.

**(b)** Este decreto es el análogo funcional uruguayo de la Ley REP chilena (Ley 20.920) y **aplica a cualquier BESS estacionario superior a 2 kWh** — es decir, a la totalidad de un portafolio BESS utility-scale o C&I. Es la primera obligación regulatoria uruguaya concreta y verificable que recae sobre el proveedor/importador de baterías, y afecta la estructura de costos EOL y los requisitos de trazabilidad documental exigibles al fabricante.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS | Clasif. |
|---|---|---|---|---|
| **Decreto N° 27/020** | Regulación de mercado | Habilita a usuarios de baja tensión (clientes de UTE) a instalar baterías en paralelo **sin inyección** a la red del distribuidor. | Enfoque detrás del medidor / autoconsumo. Sin licitación ni mandato de storage stand-alone. | **(a)** |
| **Modificación anunciada del Decreto N° 27/020** | Anuncio | Permitiría inyección a la red sin superar el consumo del usuario final. | Ampliaría el modelo de negocio BTM. **Sin texto oficial.** | **(c)** |
| **Decreto N° 227/025** | Ambiental / EOL | Marco de gestión de baterías usadas. Alcance: almacenamiento estacionario **>2 kWh**. | Obligaciones de plan maestro, registro, etiquetado y trazabilidad, metas de valorización e informes auditados para productores/importadores. | **(a)** |
| Reglamento de Baja Tensión UTE, Cap. XXIX | Técnico | Instalaciones para autoconsumo. | Requisitos técnicos de conexión BTM. | **(a)** referencia |
| Reglamentos URSEA de seguridad de productos eléctricos BT | Técnico | Incluyen especificaciones para sistemas de almacenamiento con baterías asociados a autoconsumo. | Requisitos de producto para BESS de baja tensión. | **(a)** referencia |

### Nota de estructura — actualizada 2026-08-13
**Se mantiene la conclusión del seed:** el marco de storage uruguayo sigue **marcadamente menos desarrollado** que los otros cuatro mercados. **A la fecha de esta corrida no existe licitación, mandato ni esquema de contratación de storage stand-alone equivalente a AlmaSADI (Argentina), a los Productos 3/4 de la CLPE (Colombia) ni al mandato GFM del AT-IBR (Chile).** El movimiento regulatorio de 2025-2026 fue por dos vías **ninguna de las cuales abre mercado utility-scale**: (i) ambiental/EOL (Decreto 227/025, ya vigente y con obligaciones reales), y (ii) autoconsumo BTM (revisión anunciada del Decreto 27/020, aún sin texto).

**Prioridad de vigilancia (sin cambios):** detectar si surge un marco más estructurado — en particular cualquier señal desde ADME o UTE hacia contratación de capacidad de almacenamiento en el mercado mayorista.
