# Regulación de baterías e inversores residenciales — Chile

**Fecha de la investigación:** 2026-09-30 · **Alcance:** baterías (BS/BESS) e inversores/PCE para instalaciones residenciales conectadas a la red de distribución (Ley 21.118 / DS 57/2019). Solo Chile.
**Complemento:** `regulacion_residencial_chile.xlsx` (registro de normas, estándares, paso a paso, checklist, pendientes y fuentes).

Convención de fuente (principio #2 de CLAUDE.md): **(A)** texto oficial leído en esta corrida · **(B)** interpretación mía o fuente secundaria · **(C)** borrador o trámite no vigente.

---

## 1. Resumen ejecutivo

1. **En Chile no existe una "certificación" única de batería o inversor residencial.** Hay tres capas distintas (A/B):
   - **Inversor/PCE:** *autorización de producto* de la SEC, pedida por el importador o comercializador en la Plataforma de Autorización de Productos. Se apoya en certificados IEC 62109-1/-2 y IEC 62116, detección de arco (AFCI) y un anexo con el "Perfil de Red Chile".
   - **Batería:** conformidad con **IEC 62619, UL 1973 o UL 9540** (Li-ion) o IEC 60896-21/-22 (VRLA), acreditada con documentos que el instalador adjunta al TE-4. No encontré una autorización SEC de producto específica para baterías (mi lectura, B; ver P-01).
   - **Instalación:** solicitud de conexión (SCR) a la distribuidora y declaración **TE-4** por un instalador clase A o B.
2. **Norma primaria para el BESS residencial: RGR N°06/2024 de la SEC**, modificada por la Res. Ex. SEC 33.038 (8-jul-2025). Se lee junto con RGR 01/2024 (trámite TE-4), RGR 02/2024 (inversor FV), DS 57/2019 y NT Netbilling (CNE).
3. **Cambio más reciente con impacto directo:** las autorizaciones de inversores sin detección e interrupción de arco (AFCI, IEC 63027 / UL 1699B) perdieron validez el **31-dic-2025** (A: Res. 33.038, punto 4°). Un aviso de la SEC, reproducido por una consultora, confirma que desde el 1-ene-2026 solo se declaran inversores con AFCI (B).
4. **Tensión DC del BESS:** el texto original topaba en 60 V. Res. 33.038 lo reemplaza: sobre **120 V CC** se exigen medidas adicionales contra choque y arco; ≤60 V sin riesgo de arco sostenido queda exceptuado (A).
5. **Dentro de la vivienda** solo se permite Li-ion o BESS integrado, **≤20 kWh**, y no en dormitorios, baños, cocinas ni entretechos. En exterior o anexos no hay límite de capacidad, pero el BS debe ir confinado (A).
6. **Normativa en evolución:** modificación del DS 57 (en proceso a dic-2024, estado actual no encontrado), decreto REP de baterías (anteproyecto, plazo hasta 29-ene-2027) y Decreto 32/2025 (reportado por estudio jurídico).
7. **Advertencia de calidad de datos:** varios blogs comerciales citan "D.S. 24T/2025", "D.S. 5T/2024" y "D.S. 780/2025". No los encontré en fuentes oficiales y no los uso.

---

## 2. Jerarquía documental

| Nivel | Documento | Rol para baterías/inversores residenciales |
|---|---|---|
| Ley | LGSE art. 149 bis; Ley 20.571; Ley 21.118 (límite 300 kW) | Derecho a generar, inyectar y acogerse al régimen |
| Reglamento | **DS 57/2019** (Min. Energía) | SCR (art. 15), instalador (art. 25), comunicación de energización (art. 26) |
| Reglamento | DS 8/2019 (RIC) y pliegos RIC | Seguridad del lado CA |
| Norma técnica | **NT Netbilling** (CNE, Res. Ex. 338/2019) | Conexión, protección RI, parámetros de desconexión |
| Instrucción SEC | **RGR 06/2024** (BESS) — *norma primaria para baterías y PCE del BESS* | Requisitos de producto, ubicación, protecciones, puesta en marcha |
| Instrucción SEC | RGR 01/2024 | Procedimiento TE-4 y documentos |
| Instrucción SEC | RGR 02/2024 | Inversor FV (§12), RCD, canalizaciones |
| Resoluciones SEC | 29.787/2024, 31.661/2025, 33.038/2025 y autorizaciones de producto | Aprobación, AFCI, modificaciones |

**Ambigüedad de jerarquía (no resuelta por mí):** un inversor híbrido con FV debe cumplir RGR 02 §12 y RGR 06 §11 a la vez. RGR 06 remite a los puntos 12.3 y 12.4 de RGR 02 "o los que los reemplacen" (A), así que ambos aplican; conviene confirmar la numeración vigente en el texto refundido.

---

## 3. Inversor / PCE — qué se exige

**Base:** RGR 02/2024 §12, RGR 06/2024 §11, NT Netbilling, Res. 31.661/2025 y 33.038/2025 (A).

- **Seguridad:** IEC 62109-1 e IEC 62109-2, o UL 1741 o UL 9540.
- **Anti-isla:** IEC 62116, siempre activada. Se exceptúa solo la isla autorizada por la distribuidora mediante proyecto especial.
- **AFCI:** detección e interrupción de arco conforme IEC 63027 y/o UL 1699B. Distancia máxima de 80 m de conductor CC entre el AFCI y el último módulo, salvo acreditación del fabricante. Sin AFCI integrado solo procede un proyecto especial con AFCI externo.
- **Comunicación:** Modbus (RTU/TCP/RS485) o IEC 61850 si el inversor supera 5 kW o el conjunto supera 20 kW.
- **Perfil de Red Chile (NT Netbilling, Tabla 2):** V< 0,80 Vn; V> 1,10 Vn (media 10 min); V>> 1,15 Vn; f< 47,5 Hz; f> 51,5 Hz; cada función <100 ms y desconexión total ≤200 ms. Los ajustes son inalterables salvo V>.
- **PCE de BESS:** debe seleccionarse según química y tensión de la batería; para Li-ion la compatibilidad marca/modelo debe estar validada por el fabricante del PCE y de la batería. Configuración protegida por contraseña o hardware. IP55 a la intemperie; IP20 en sala o gabinete.
- **PCE sin puertos para otras fuentes:** IEC 62477-1 o IEC 62040-1 y autorización SEC.
- **Puerto para carga de VE:** IEC 62909-2 o IEC 61851-23 (CC); IEC 61851-1 (CA).
- **RCD en instalaciones FV (Res. 33.038):** IΔn ≤30 mA hasta 5 kW, ≤100 mA hasta 10 kW, ≤300 mA hasta 300 kW.

## 4. Batería — qué se exige

**Base:** RGR 06/2024 §§5–9, 12–16 (A).

- **Químicas admitidas:** Li-ion y VRLA. Otras químicas se presentan como proyecto especial ante la SEC.
- **Li-ion (celdas, sistemas de baterías y BMS):** IEC 62619 **o** UL 1973 **o** UL 9540. Los documentos se adjuntan al TE-4.
- **VRLA:** IEC 60896-21 e IEC 60896-22.
- **BMS obligatorio** en Li-ion, compatible con el protocolo del PCE.
- **Tensión CC (Res. 33.038):** >120 V exige medidas adicionales; ≤60 V sin riesgo de arco sostenido queda exceptuado.
- **Ubicación:**
  - Dentro de la vivienda: Li-ion o BESS integrado, ≤20 kWh, fuera de dormitorios, baños, cocinas y entretechos. Tabique RF60 si se monta en pared; pasillo de 1 m hacia salidas.
  - Exterior/anexos: cualquier capacidad, BS confinado y con llave. IP55 mínimo a la intemperie. RF60 si hay zona habitable al otro lado.
  - Distancias de 600 mm a salidas de gases, ventanas y equipos de clima; altura máxima de 2,2 m.
- **Sobre 20 kWh (Li-ion) o 40 kWh (Pb-ácido):** evaluación y gestión de peligros (Anexos A y B), acceso restringido, ventilación calculada, detección de humo, alarma, extintor e iluminación de emergencia.
- **Señalización, manual O&M, inducción al propietario y Anexo 11** firmados (RGR 06 §16).

---

## 5. Paso a paso

### 5.1 Habilitar un inversor (fabricante/importador)

1. Clasificar el equipo (on-grid, híbrido bidireccional, off-grid; puertos).
2. Obtener certificados IEC 62109-1/-2 e IEC 62116 de un organismo de certificación acreditado. Las dos autorizaciones de inversores que leí usan TÜV SÜD (CB Scheme) y KIWA (DAkkS/ENAC); otros resultados de búsqueda mencionan Intertek y CCIC (no leídos).
3. Acreditar AFCI (IEC 63027 / UL 1699B).
4. Preparar anexo técnico con el Perfil de Red Chile e imágenes de la configuración.
5. El importador o comercializador ingresa la solicitud en la **Plataforma de Autorización de Productos** de la SEC.
6. La SEC emite una **Resolución Exenta** con la tabla de modelos autorizados. Vigencia observada de **5 o 6 años**; pierde validez si cambia el modelo certificado.
7. Verificar el modelo en el buscador de Equipamiento Autorizado.

*Plazos observados (B, solo dos casos):* Victron, solicitud 8-feb-2024 → resolución 14-mar-2024 (35 días); Solis, solicitud 14-oct-2024 → resolución 13-nov-2024 (30 días). No hay plazo oficial.

### 5.2 Habilitar una batería

1. Clasificar (BESS integrado, BS ensamblado o no ensamblado) y química.
2. Obtener IEC 62619 / UL 1973 / UL 9540 (Li-ion) o IEC 60896-21/-22 (VRLA).
3. Validar compatibilidad con los inversores objetivo junto al fabricante del PCE.
4. Preparar dossier: manual de instalación, SDS, parámetros de carga/descarga, placa indeleble, garantías.
5. Logística: UN 38.3 y clase 9 (B; no verifiqué la norma chilena de transporte, ver P-08).
6. Si el equipo incluye WiFi/Bluetooth: declaración SUBTEL con QR (B).

### 5.3 Instalar y declarar (instalador A o B con el usuario)

1. Presentar SCR a la distribuidora. Agregar batería a un EG existente implica un proyecto nuevo con EG + almacenamiento (A: NT Netbilling). El usuario tiene 20 días hábiles para manifestar conformidad.
2. Diseñar y ejecutar según RGR 06, RGR 02 (si hay FV) y RIC.
3. Probar y poner en marcha: polaridad, tierras, desconexiones, ajustes del PCE, carga/descarga a corriente máxima configurada, procedimiento de apagado. Instrumentos IEC 61557 con calibración ≤36 meses de laboratorio acreditado ISO/IEC 17025.
4. Declarar **TE-4** digital con proyecto definitivo, SCR, ajustes del PCE con número de serie, evidencia de la batería y manual O&M.
5. Inducción al propietario y firma del Anexo 11. Entrega del comprobante TE-4 y del protocolo de conexión de la distribuidora.
6. La SEC puede fiscalizar aun con TE-4 inscrito.

---

## 6. Hallazgos recientes (formato CLAUDE.md)

| País | Qué cambió | Fuente | Tipo de proyecto afectado | Relevancia |
|---|---|---|---|---|
| Chile | Autorizaciones de inversores sin AFCI perdieron validez el 31-dic-2025 (A); desde 1-ene-2026 solo se declaran inversores con AFCI (B, aviso SEC vía consultora) | Res. Ex. SEC 33.038/2025 y 31.661/2025 | Inversores on-grid e híbridos residenciales | **Alto** |
| Chile | Tope de 60 V CC reemplazado: >120 V exige protecciones adicionales; ≤60 V exceptuado (A) | Res. Ex. SEC 33.038/2025 | BESS residencial de alta tensión | **Alto** |
| Chile | RGR 01/02/06-2024 reemplazan a los de 2020/2021 (A) | Res. Ex. SEC 29.787/2024 | Todo BESS/FV residencial | **Alto** |
| Chile | RCD por potencia del EG: 30/100/300 mA (A) | Res. Ex. SEC 33.038/2025 | FV + BESS residencial | Medio |
| Chile | SUBTEL pasa a autodeclaración con QR para equipos de alcance reducido desde feb-2026 (B) | Res. SUBTEL 737/2025 | Equipos con WiFi/Bluetooth | Medio |
| Chile | Decreto REP de baterías: plazo ampliado al 29-ene-2027 (A; contenido C) | MMA, RE 4.225/2026 | Baterías de almacenamiento (fin de vida) | Medio |
| Chile | Decreto 32/2025 publicado el 17-jun-2026 según estudio jurídico (B) | Garrigues | Generación distribuida y SAE (alcance residencial incierto) | Bajo |

---

## 7. Ambigüedades señalizadas para tu decisión

1. **¿La batería necesita autorización SEC de producto?** RGR 06 pide autorización para el PCE, pero para la batería solo "documentos que acrediten" IEC 62619/UL 1973/UL 9540. No encontré listados ni resoluciones de autorización de baterías. Recomiendo consultar por escrito a SEC-UERNC (P-01).
2. **Cuál es el documento primario de requisitos de autorización de inversores.** Las autorizaciones citan Res. 32.427/2020 y 26.493/2024; la 31.661/2025 agrega AFCI. No leí esos textos (P-02).
3. **Texto local desactualizado.** La copia `chile/contentRGR-N-06-2024_v4-destacada.md` no incluye Res. 33.038 y aún dice 60 V (P-03).
4. **Modificación del DS 57.** CNE dijo en dic-2024 que el Ministerio lo está modificando y por eso posterga la NT Netbilling. No encontré el estado actual (P-04).
5. **Afirmaciones de blogs no verificadas** (P-10).

La lista completa (11 ítems) está en la hoja `Pendientes` del Excel.

---

## 8. Límites de esta corrida

- No pude recalcular el Excel con LibreOffice en este entorno (no cargó archivos). Las celdas de la hoja `Resumen` tienen fórmulas y llevan los valores ya calculados; se verificaron leyendo el archivo con openpyxl.
- Varias páginas se verificaron por resumen, no por texto completo (ver hoja `Fuentes`).
- No cubrí Aduanas, transporte terrestre, consumidor/garantías, tributación ni incentivos.
- No actualicé `regulacion_LATAM.md` ni `ultima_revision_regulatoria.md`: esta investigación es un segmento nuevo (residencial) y no es una corrida semanal de vigilancia. Dime si quieres integrarlo.
