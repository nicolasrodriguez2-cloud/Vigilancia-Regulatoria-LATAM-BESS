# Panorama Regulatorio BESS — LATAM

> **Origen de este seed:** este archivo se generó a partir de la sección "REGULATION INVOLVED" / "GOVERMENT INSTITUTIONS" / "PUBLIC POLICIES" de `BESS_POTENTIAL_CLIENTS_v2.xlsx` (corte de datos: 2026-08-12), no de una corrida real del agente de Vigilancia Regulatoria. Es un punto de partida, no una revisión confirmada. **La primera corrida de la Routine debe validar cada ítem contra la fuente oficial antes de dar cualquiera de estos datos por vigente**, siguiendo el principio no negociable de no confiar en conocimiento previo para el estado regulatorio.
>
> Clasificación de fuente por defecto de este seed: **(b) extraído de archivo de mercado interno**, no (a) texto oficial confirmado directamente por esta vigilancia — salvo que se indique lo contrario.

---

## Chile

### Reguladores / instituciones
- **Ministerio de Energía** — máxima autoridad ejecutiva: política energética nacional, planificación estratégica, decretos que regulan generación, transmisión, distribución y almacenamiento.
- **CNE — Comisión Nacional de Energía** — cuerpo técnico asesor: normas regulatorias, precios regulados (precio nudo, semestral), metodologías de servicios complementarios y almacenamiento.
- **CEN — Coordinador Eléctrico Nacional** — operador del sistema: despacho en tiempo real, costo marginal, liquidaciones económicas, aprobación de acceso a la red para proyectos nuevos incluyendo BESS.
- **SEC — Superintendencia de Electricidad y Combustibles** — fiscaliza cumplimiento de la ley eléctrica, otorga concesiones, autoriza conexión física de instalaciones de generación y almacenamiento.
- **Panel de Expertos** — cuerpo colegiado independiente, resuelve disputas técnicas y tarifarias vinculantes (peajes de transmisión, costos de servicios complementarios).
- **Ministerio del Medio Ambiente / SEA** — administra el SEIA; todo proyecto de generación o almacenamiento sobre umbral definido requiere Resolución de Calificación Ambiental (RCA).

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS |
|---|---|---|---|
| Ley General de Servicios Eléctricos (LGSE) | Regulación de mercado | Marco original de generación/transmisión/distribución, sin almacenamiento contemplado originalmente. | Norma base; toda regulación de storage posterior es una modificación de esta ley. |
| Ley N°20.936 | Regulación de mercado | Primera ley en reconocer formalmente la existencia de sistemas de almacenamiento. Define SAE (Sistema de Almacenamiento de Energía) y CRCA. | Introduce categorías legales SAE/CRCA; storage reconocido pero sin mecanismo de pago definido. |
| Ley N°21.505 | Regulación de mercado | Permite a sistemas de batería stand-alone (SAE) vender energía y recibir pagos por potencia de suficiencia en el mercado mayorista. | SAE stand-alone puede vender en el mercado spot y acceder a potencia de suficiencia. |
| DS N°62 | Regulación de mercado | Rige pagos por potencia (suficiencia) para todos los generadores. | Pagos basados en contribución de confiabilidad en punta; tecnología de referencia: diésel. |
| DS N°70 | Regulación de mercado | Modifica DS 62 y DS 125 para que baterías stand-alone reciban pagos por potencia — fórmula: a mayor duración de descarga, mayor crédito de capacidad (vigente 10 años). | Tabla de reconocimiento por duración, aplica a SAE y CRCA. |
| Ley N°21.721 | Transmisión | Ataca cuellos de botella de transmisión que bloquean renovables. Beneficia indirectamente al almacenamiento. | Acelera permisos de nuevas líneas; complemento estratégico de la Ley 21.505. |
| DS N°125 | Regulación de mercado | SAE puede proveer Servicios Complementarios; actualiza reglas de despacho económico para incluir BESS explícitamente en coordinación en tiempo real y formación de precios. | Habilita pago formal por servicios complementarios — actualización más crítica para rentabilidad de BESS en el corto plazo. |
| DS N°37 | Transmisión | Regula planificación, construcción y operación del sistema de transmisión; conecta SAE a la planificación de transmisión. | CEN puede co-optimizar formalmente storage y transmisión; BESS puede sustituir expansión de transmisión si es económicamente equivalente. |
| MINVU 522 | Planificación urbana | Regulación urbana aplicable a sistemas de almacenamiento (BESS en particular). | Clasifica BESS stand-alone como "Infraestructura Energética" (Art. 2.1.29 OGUC); requiere permiso de edificación, no concesión. |
| Ley N°20.920 (REP) | Responsabilidad extendida del productor | Responsabiliza a productores/importadores por recolección y reciclaje de productos prioritarios, incluidas baterías. | Baterías industriales BESS ≥5 kg listadas como producto prioritario; fiscalizada por SMA. |
| DS 88 | Regulación de mercado | Actualiza régimen PMGD para permitir que BESS bajo 9 MW use margen de capacidad de red disponible para carga. | Nueva vía de ingreso para BESS comercial/industrial distribuido hasta 9 MW. |
| NTSyCS | Seguridad | Requisitos de seguridad y calidad para instalaciones del SEN, incluyendo BESS. | Cubre esquemas de protección, desconexión y comunicaciones para SAE. |
| REx CNE N°41-2025 | Seguridad | Primera regulación con requisitos sísmicos específicos para BESS e instalaciones eléctricas de alta tensión. | Aplica a BESS, sistemas de transmisión y equipos de compensación; referencia NCh 2369:2023 e IEEE 693:2018; obligatorio para permisos e ingeniería de proyectos BESS nuevos. |
| DS N°148 | Seguridad | Manejo, transporte y disposición de residuos peligrosos, incluidos componentes de baterías de litio. | Baterías de litio clasificadas como residuo peligroso en operación y desmantelamiento. |
| DS N°8 | Seguridad | Diseño, construcción y operación de instalaciones eléctricas de consumo. | Fichas técnicas RIC. |
| **AT-IBR (REx CNE N°45-2026, marzo 2026)** | Código de red | GFM no obligatorio aún, pero referenciado explícitamente. Actualización del código de red chileno para incorporar requisitos GFM está en curso — basada en estudio NREL G-PST. | **Norma primaria para requisitos IBR/GFM** — no está en la NTSyCS. Fabricantes con capacidad GFM certificada tendrán estatus preferente en futuras licitaciones SSCC. |

### Políticas públicas relevantes
- **Plan Nacional de Almacenamiento — Terrenos Fiscales**: permite a desarrolladores de storage solicitar arriendo directo en terrenos fiscales del norte de Chile (Norte Grande: Tarapacá, Antofagasta, Atacama). Concesión directa, sin licitación pública; abierto a cualquier desarrollador.
- **Segunda Fase de la Agenda de Transición Energética**: hoja de ruta gubernamental de descarbonización; storage es pilar explícito.
- **Estudio de Almacenamiento CEN (2023)**: capacidad óptima de BESS estimada en 1.000–4.000 MW (2026–2032), duración óptima de descarga 6–8h, almacenamiento diario óptimo de energía 13,2 GWh.

### Nota de estructura
Las licitaciones chilenas contratan energía (GWh/año); el BESS entra por lógica de mercado e incentivos, no por mandato regulatorio directo.

---

## Argentina

### Reguladores / instituciones
- **Secretaría de Energía (SE)** — autoridad de política principal, emite resoluciones que rigen el MEM, convocó directamente AlmaGBA y AlmaSADI.
- **CFEE — Consejo Federal de la Energía Eléctrica** — consejo asesor a gobiernos nacional y provinciales; administra el FNEE.
- **CAMMESA** — nodo operativo central del mercado: despacho técnico-económico del SADI, cálculo de precios spot, administración del mercado a término.
- **Ente Nacional Regulador del Gas y la Electricidad** (fusión 2025 de ENRE + ENARGAS, Decreto 452/2025) — regula y supervisa generación, transmisión y distribución federal (EDENOR, EDESUR); autoriza el punto de acceso a la red de cada proyecto de storage nuevo.
- **EDENOR / EDESUR** — distribuidoras federales, compradoras directas de capacidad BESS vía AlmaGBA.
- **Transener** — principal transportista de alta tensión (troncal 500 kV).

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS |
|---|---|---|---|
| Ley N°15.336 | Marco general | Ley fundacional del sector eléctrico argentino; jurisdicción federal sobre electricidad interprovincial vía SADI. | Autoriza a la Secretaría de Energía a regular el MEM y emitir resoluciones como AlmaGBA/AlmaSADI. |
| Ley N°24.065 | Mercado mayorista | Crea el mercado mayorista competitivo. Decreto 450/2025 restauró principios marginalistas. | Toda resolución BESS cita esta ley como base legal. |
| Ley N°27.742 (Ley Bases) | Inversión privada | Delegó al Ejecutivo la actualización del marco regulatorio eléctrico por decreto. | Habilitó el proceso de reforma del MEM que derivó en el Decreto 450/2025 y la Res. 400/2025. |
| Ley N°26.190 y N°27.191 | Renovables / grandes usuarios | Meta obligatoria de 20% renovables al 31-dic-2025 para consumidores ≥300 kW. | Demanda cautiva para contratación MATER; proyectos híbridos BESS acceden a estos beneficios. |
| SE Res. N°36/2023 y N°906/2023 (RenMDI / ALMA MDI) | Renovables / BESS híbrido | Primera apertura formal a proyectos renovables con storage. 633,7 MW adjudicados en 98 proyectos. | Primer marco contractual que exige datos técnicos de BESS. |
| **SE Res. N°67/2025 — AlmaGBA** | Storage stand-alone | Primera licitación exclusiva para storage stand-alone a gran escala. 713 MW adjudicados en agosto 2025. | Define el modelo "Storage Generation Contract" — estándar de mercado. Duración mínima de descarga: 4h (HAC). Compradores: EDENOR/EDESUR. |
| SE Res. N°344, 361, 384/2025 | Storage stand-alone | Formalizan adjudicación de los 713 MW de AlmaGBA. | Pago por capacidad hasta USD 12.500/MW/mes; energía USD 10/MWh fijo hasta 2037. |
| **SE Res. N°50/2026 — AlmaSADI** | Storage stand-alone | Segunda generación de licitaciones BESS, ahora a escala nacional (todo el SADI). CAMMESA compra directo (no solo garante). Adjudicación: 19-jun-2026. | Meta: hasta 700 MW. Cupos regionales por zona (NEA, Litoral, Buenos Aires, NOA, Centro, Cuyo, La Pampa). Contratos a 10 años. |
| SE Res. N°400/2025 — Normalización MEM | Reforma MEM | Vigente desde 1-nov-2025. Redefine categorías de generador; crea Mercado a Término de Energía y Capacidad. | BESS de AlmaGBA/AlmaSADI califican como "Nueva Generación". |
| Decreto N°450/2025 | Reforma estructural | Actualiza texto de Ley 24.065; restaura principios marginalistas; período de transición de 24 meses (hasta jul-2027). | Nuevo Art. 9°: distribuidoras deben contratar ≥75% de su demanda vía contratos de largo plazo. |
| Decreto 513/2025 | Incentivo fiscal | Reduce arancel de importación de sistemas de batería de litio a 12,6%. | Reduce costo de importación de BESS. |
| RIGI — Ley 27.742, Título VII | Incentivo de inversión | Régimen para proyectos >USD 200M en sectores estratégicos incluida energía; estabilidad fiscal y regulatoria de 30 años. | Clusters BESS grandes o proyectos renovable+storage integrados >USD 200M pueden calificar. |

### Políticas públicas relevantes
- **RENPALMA** — Registro Nacional de Proyectos de Almacenamiento; primer instrumento sistemático de seguimiento de la flota de storage argentina.

### Nota de estructura
AlmaSADI contrata directamente capacidad de almacenamiento (MW/MWh) stand-alone, a diferencia de Chile.

---

## Colombia

### Reguladores / instituciones
- **MinMinas y Energía** — define política energética nacional, metas estratégicas (Plan 6GW+), convoca subastas de largo plazo (Res. 40208/2026).
- **CREG** — regula el MEM: precios de bolsa, OEF, SSCC, acceso a la red; plazo de 12 meses (Decreto 1091/2025) para definir metodología de remuneración BESS.
- **UPME** — planificación energética nacional (PEN 2024–2054); aprueba conexiones de proyectos FNCER y BESS.
- **XM (ISA)** — operador del SIN (CND, despacho en tiempo real) y administrador del mercado (ASIC, liquidación).
- **ANLA / SSPD** — ANLA: licenciamiento ambiental (cuello de botella clave en la ejecución del pipeline). SSPD: supervisa utilities, puede intervenir operadores.
- **BMC — Bolsa Mercantil de Colombia** — operador designado de la subasta de largo plazo 2026.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS |
|---|---|---|---|
| Ley 143/1994 | Marco legal sectorial | Crea la CREG; establece generación, transmisión, distribución y comercialización como actividades reguladas; modelo de pool competitivo. | Fundación del modelo de mercado. |
| Ley 1715/2014 | Marco FNCER | Incentivos fiscales para solar, eólica, biomasa, pequeña hidro (deducción 50% renta, exención IVA, arancel cero, depreciación acelerada 33%/año). Modificada por Ley 2099/2021. | Aplica a BESS acoplado a FNCER; BESS standalone en revisión. |
| Ley 2099/2021 (Ley de Transición Energética) | Marco FNCER | Extiende incentivos de Ley 1715 a todos los proyectos de energía. Primer reconocimiento legal explícito del almacenamiento en planificación del SIN. | Base legal para storage en la planificación nacional. |
| Res. CREG 071/2006 | Cargo por confiabilidad | Regula la Obligación de Energía Firme (OEF), precio de escasez, gatillo de condición crítica. Última modificación: Res. 101 066/2024. | Marco de adecuación de capacidad — vía potencial para BESS. |
| Res. CREG 098/2019 | Storage | Primer reconocimiento regulatorio formal del almacenamiento en el SIN. Habilitó proyectos piloto BESS. | Origen de la regulación colombiana de BESS. |
| Res. CREG 101 066/2024 | Precios de escasez | Diferencia precios de escasez por tipo de planta: alto para térmica gas/ACPM, bajo para solar/renovables. | Afecta competitividad de BESS para la Obligación de Confiabilidad. |
| **Decreto 1091/2025** | Contratación de largo plazo | Directrices de política para contratación de largo plazo de generación y storage; backstop si CREG se demora. | Habilita BESS standalone en subastas de largo plazo. CREG tiene 12 meses para definir metodología de remuneración BESS. |
| **Res. CREG 701-103/2025** | Marco técnico BESS | Marco técnico, comercial y operacional completo para SAEB en el SIN. En consulta pública. Servicios: arbitraje de energía, AGC, black start. | Regulación específica de BESS — hito clave. |
| Res. MinMinas 40178/2026 | Contratación de largo plazo | Reglas generales para contratación de largo plazo de energía limpia; introduce storage en esquemas de subasta competitiva. | Marco habilitante previo a la subasta LP. |
| **Res. MinMinas 40208/2026** | Subasta de largo plazo | Convoca la primera subasta de largo plazo de Colombia con BESS como producto explícito. Productos: solar, eólico, híbrido solar+BESS (franja 17-21h), BESS standalone. Contratos a 15 años. Obligaciones desde 1-ene-2030. Adjudicación antes del 31-jul-2026. | Primera subasta de largo plazo que incluye BESS como producto. Hito regulatorio central. |

### Políticas públicas relevantes
- **Incentivos activos (proyectos FNCER certificados)**: deducción de renta 50%, exclusión de IVA, arancel cero, depreciación acelerada hasta 33,3%/año — trámite vía UPME + certificación ANLA.
- **Subasta LP 2026**: lanzada abril 2026; adjudicación antes del 31-jul-2026; inicio de obligaciones 1-ene-2030; composición: solar, eólico, híbridos solar+BESS (franja 17-21h), BESS autónomo; contratos a 15 años (Res. 40208/2026 + Res. 40178/2026).

### Nota de estructura
El caso de storage colombiano está enraizado en riesgo hidrológico (dependencia de El Niño), a diferencia de la curtailment solar en Chile o el deterioro de transmisión en Argentina. Producto 3 mandata almacenamiento explícitamente.

---

## Perú

### Reguladores / instituciones
- **MINEM — Ministerio de Energía y Minas** — máxima autoridad ejecutiva: políticas energéticas nacionales, planificación estratégica, concesiones de generación/transmisión/distribución.
- **OSINERGMIN** — brazo regulatorio bajo MINEM: normas técnicas, revisión de planes de expansión de red, permisos administrativos de conexión.
- **ProInversión** — administra el Plan Nacional de Electrificación Rural (PNER); ejecuta microrredes solar-storage autónomas en zonas rurales fuera de red.
- **COES** — operador independiente del sistema (SEIN) y cámara de compensación financiera; establece procedimientos técnicos de conexión (ej. PR20) y penaliza desviaciones de red.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS |
|---|---|---|---|
| D.Leg. 25844 — Ley de Concesiones Eléctricas | Marco legal | Fundamento del modelo mixto peruano: separa generación, transmisión y distribución; introduce participación privada. | Base legal del SEIN. No contempla almacenamiento. |
| D.S. 009-93-EM — Reglamento LCE | Regulación de mercado | Reglas operativas del mercado: despacho por mérito, tarifas, obligaciones de agentes. | Sin mención de almacenamiento. |
| Ley 28832 — Desarrollo Eficiente de la Generación | Regulación de mercado | Introduce licitaciones de energía, mecanismo OEF, refuerza competencia en generación. | Marco de licitaciones que la Ley 32249 modifica para habilitar BESS. |
| Res. OS 224-2021 (OSINERGMIN) | Regulación de mercado | Modifica el procedimiento del COES para cálculo de costos variables. | Mejoró la señal de precio spot → mayor spread potencial para arbitraje en estiaje. |
| RM 278-2023-MINEM — Hoja de Ruta Smart Grids | Política pública | Estrategia nacional de redes inteligentes 2023–2030; reconoce el almacenamiento como componente clave. | Primera mención explícita de BESS en política pública. Sin normativa de desarrollo aún. |
| **Ley 32249 — Modificación Ley 28832** | Regulación de mercado | Crea la figura del Proveedor de Servicios Complementarios (PSC). Habilita PPAs sin respaldo de potencia. Vigente desde 1-ene-2026. | Marco legal que reconoce BESS standalone como PSC. Habilita arbitraje de energía y potencia. |
| **PR20 — Procedimiento técnico COES** ("Ley de Inercia") | Requisito técnico | Obliga a toda central conectada al SEIN a aportar inercia sintética desde 2028. Respuesta <100ms, conexión <20ms, potencia firme <50ms. | Mandato técnico de BESS para toda generadora. **Sin remuneración definida — principal brecha del mercado.** |
| Reglamento de servicios complementarios (MINEM) | Pendiente | Normativa pendiente ordenada por Ley 32249; definirá remuneración, conexión y permisos para PSC/BESS standalone. | **Pieza regulatoria más crítica pendiente** — sin ella el business case standalone es especulativo. |
| Reglamentación de generación distribuida | Pendiente | Marco para generación descentralizada, prosumidores y BESS behind-the-meter a escala comercial. | Su ausencia bloquea desarrollo C&I y electrificación rural con almacenamiento. |

### Nota de estructura
El mandato técnico (PR20) va por delante de la remuneración — es la brecha regulatoria más relevante a monitorear en este mercado.

---

## Uruguay

### Reguladores / instituciones
- **MIEM — Ministerio de Industria, Energía y Minería** — autoridad de política energética nacional.
- **URSEA — Unidad Reguladora de Servicios de Energía y Agua** — regulación técnica y tarifaria.
- **UTE — Administración Nacional de Usinas y Trasmisiones Eléctricas** — utility estatal; aprueba instalaciones de storage para sus clientes bajo el decreto de 2020.
- **ADME — Administración del Mercado Eléctrico** — administrador/despachador del mercado eléctrico.

### Regulación vigente relacionada a BESS

| Norma | Tipo | Descripción | Relevancia BESS |
|---|---|---|---|
| Decreto 2020 (habilitación de storage) | Regulación de mercado | Habilita a clientes de UTE a instalar sistemas de almacenamiento de energía. | Enfoque detrás del medidor / autoconsumo. **Sin licitación o mandato de storage stand-alone identificado a la fecha.** |

> ⚠️ **Marcado explícitamente como no confirmado en la fuente original**: "[Estimación / pendiente de verificación por Vigilancia Regulatoria LATAM — confirmar vigencia y alcance actual antes de usar como dato firme]". Mantener este flag hasta que una corrida real de la Routine lo valide contra fuente oficial.

### Nota de estructura
Marco regulatorio de storage marcadamente menos desarrollado que los otros cuatro mercados — no hay ley o esquema de licitación dedicado equivalente a AlmaSADI (Argentina) o Producto 3 (Colombia). Prioridad de vigilancia: detectar si surge un marco más estructurado.
