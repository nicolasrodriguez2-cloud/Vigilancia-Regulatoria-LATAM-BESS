# Vigilancia-Regulatoria-LATAM-BESS

Repo de vigilancia regulatoria de BESS en los mercados donde opera Nicolás como PM en BYD Chile: Chile, Argentina, Colombia, Perú y Uruguay.

Este repo es la fuente de verdad del panorama regulatorio vigente por país. Se mantiene mediante una arquitectura de tres herramientas coordinadas (Claude Code Routines + Chat Project + Cowork), documentada en el Project "Diseño de Agentes".

Qué hay en este repo
Archivo / carpeta	Qué es	Quién lo edita
CLAUDE.md	Instrucciones que sigue la Routine en cada corrida: rol, principios, mercados/fuentes oficiales, checklist, formato de PR.	Nicolás (vía Chat Project, revisión humana)
regulacion_LATAM.md	Panorama regulatorio vigente por país. Archivo oficial único — sin fecha en el nombre.	Routine (directo, en su rama)
ultima_revision_regulatoria.md	Tabla de seguimiento: última fecha de revisión y última novedad detectada por país.	Routine (directo, en su rama)
/historial/	Copias fechadas (YYYYMMDD_regulacion_LATAM.md) de regulacion_LATAM.md, una por cada corrida que detectó cambios.	Routine (solo agrega, nunca reemplaza)
Cómo se actualiza
Una Claude Code Routine corre semanalmente en la nube (sin depender de que haya una compu prendida).
Clona este repo, lee CLAUDE.md, y revisa fuentes oficiales de los 5 mercados.
Si hay novedades: edita regulacion_LATAM.md y ultima_revision_regulatoria.md directo, en su propia rama (claude/vigilancia-regulatoria-YYYYMMDD), y guarda copia fechada en /historial/.
Si no hay novedades: solo actualiza la fecha en ultima_revision_regulatoria.md.
Abre un único Pull Request con el changelog de la semana (resumen ejecutivo, hallazgo por país con fuente y tipo de proyecto BESS afectado, y cualquier ambigüedad estructural señalizada para revisión humana).
Nicolás revisa el diff y mergea manualmente — la Routine nunca mergea su propio PR ni decide sola sobre ambigüedades estructurales (ej. si una norma nueva reemplaza o complementa a la vigente).
Cómo se consulta
Preguntas puntuales ("¿qué dice la última resolución sobre GFM en Perú?", "¿sigue vigente tal requisito?") → Chat Project "Vigilancia Regulatoria LATAM" en claude.ai, conectado a este repo vía conector de GitHub. Lee y responde directo desde acá, sin necesidad de tener el archivo subido a mano en otro lado.
Sesión de investigación en profundidad (nivelación puntual, revisar un tema regulatorio a fondo) → Cowork, de forma interactiva.
Revisión y merge de PRs → directo en GitHub.
Principios no negociables (resumen — el detalle completo está en CLAUDE.md)
Un solo archivo oficial por tipo de dato, sin fecha en el nombre; el historial vive en /historial/.
Nunca mezclar sin aclarar: (a) texto oficial confirmado, (b) interpretación propia, (c) rumor o borrador no oficial.
Diff-first siempre — ningún cambio se aplica sin pasar por PR y revisión.
Ninguna corrida automática decide sola sobre ambigüedades estructurales (si una norma reemplaza o complementa a otra, por ejemplo) — quedan señalizadas en el PR.
Alcance por país en general, no por proyecto de cliente específico — la conexión con proyectos activos la hace Nicolás por su cuenta en otro espacio (Intake BESS / Inteligencia de Mercado).
Mercados cubiertos

Chile (CNE, CEN, Ministerio de Energía) · Argentina (CAMMESA, Secretaría de Energía) · Colombia (CREG, XM, UPME) · Perú (OSINERGMIN, COES) · Uruguay (MIEM, URSEA, UTE, ADME)

Detalle de documentos clave y notas de estructura de cada mercado: ver CLAUDE.md.
