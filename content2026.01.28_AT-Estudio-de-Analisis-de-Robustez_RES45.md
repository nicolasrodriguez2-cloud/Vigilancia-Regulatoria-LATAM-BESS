NORMA TÉCNICA DE SEGURIDAD Y
CALIDAD DEL SERVICIO
ANEXO TÉCNICO DE METODOLOGÍA PARA EL
ESTUDIO DE ANÁLISIS DE ROBUSTEZ DEL
SISTEMA ELÉCTRICO NACIONAL
Enero de 2026
Santiago, Chile

—–——–
ÍNDICE
Título 1 Aspectos generales ................................................................................................... 2
Artículo 1-1 Objetivo del Anexo ................................................................................................ 2
Artículo 1-2 Alcance .................................................................................................................. 2
Artículo 1-3 Abreviaturas y definiciones ................................................................................... 2
Artículo 1-4 Objetivo y resultados del Estudio ......................................................................... 2
Artículo 1-5 Alcance del Estudio ............................................................................................... 3
Artículo 1-6 Conjunto de medidas que contribuyen a robustecer el SI .................................... 3
Artículo 1-7 Publicación del Estudio ......................................................................................... 3
Artículo 1-8 Informe preliminar y final del Estudio .................................................................. 4
Artículo 1-9 Actualización del Estudio anual ............................................................................ 4
Título 2 Funciones y obligaciones ........................................................................................... 5
Artículo 2-1 Funciones y obligaciones del Coordinador ........................................................... 5
Artículo 2-2 Obligaciones de los Coordinados .......................................................................... 5
Título 3 Procedimiento para realizar el Estudio ...................................................................... 6
Artículo 3-1 Consideraciones y horizonte de evaluación del Estudio ....................................... 6
Artículo 3-2 Metodología para el desarrollo del Estudio .......................................................... 6
Artículo 3-3 Base de datos ........................................................................................................ 7
Artículo 3-4 Modelo dinámico del SI proyectado ..................................................................... 8
Artículo 3-5 Escenarios de operación ....................................................................................... 8
Artículo 3-6 Indicadores para identificación de áreas .............................................................. 9
Artículo 3-7 Determinación de áreas de frecuencia y tensión ............................................... 10
Artículo 3-8 Determinación de contingencias ........................................................................ 11
Artículo 3-9 Indicadores de desempeño dinámico ................................................................. 13
Artículo 3-10 Cálculo del índice de desempeño dinámico ....................................................... 13
Artículo 3-11 Cálculo de frecuencia mínima y RoCoF ............................................................... 14
Artículo 3-12 Medidas que pueden robustecer el SI ................................................................ 14
Artículo 3-13 Análisis de Fortaleza o Robustez de Tensión ....................................................... 16
Artículo 3-14 Resultados del análisis de Fortaleza ................................................................... 19
Artículo 3-15 Análisis de la Robustez de Frecuencia ................................................................ 20
Título 4 Disposiciones transitorias ....................................................................................... 22
Artículo 4-1 Publicación del primer Estudio ........................................................................... 22
Artículo 4-2 Publicación del primer listado de indicadores SCL y K ........................................ 22
Comisión Nacional de Energía 1 de 22

—–——– Título 1 Aspectos generales
Título 1 Aspectos generales
Artículo 1-1 Objetivo del Anexo
El presente Anexo Técnico tiene por objetivo establecer la metodología que deberá aplicar el
Coordinador para la elaboración del Estudio de Análisis de Robustez del Sistema Eléctrico Nacional
(en adelante, el “Estudio”), de acuerdo con lo señalado en el Título 6-8 de la Norma Técnica de
Calidad y Seguridad de Servicio (en adelante, “NTSyCS”).
Artículo 1-2 Alcance
El Anexo establece los procedimientos, criterios, escenarios, supuestos e indicadores que deberán
ser utilizados por el Coordinador para el desarrollo del Estudio, con el propósito de asegurar
consistencia metodológica, transparencia y trazabilidad en los resultados.
A efectos de la aplicación del presente Anexo Técnico, los plazos establecidos sólo consideran días
hábiles, salvo en los casos que se indique expresamente lo contrario.
Artículo 1-3 Abreviaturas y definiciones
A efectos de la aplicación del presente Anexo Técnico, se aplican las abreviaturas y definiciones
establecidas en el Título 1-2 de la NTSyCS.
Artículo 1-4 Objetivo y resultados del Estudio
El Estudio tiene por objeto evaluar la Robustez del SI en el corto y mediano plazo, con el fin de
determinar su evolución, identificar tendencias y áreas débiles, así como proponer un conjunto de
medidas que permitirían robustecer dichas áreas cuando ello resulte necesario.
La Robustez se evalúa en función del desempeño dinámico del SI durante contingencias,
considerando escenarios de operación creíbles, pero exigentes desde el punto de vista de la
Robustez. La evaluación del desempeño dinámico del sistema se deberá realizar mediante los
indicadores de desempeño establecidos en el Artículo 3-9 del presente Anexo Técnico. El Estudio
deberá contener, al menos:
a) Áreas débiles del SI, tanto desde la perspectiva de la Robustez de Frecuencia como de la
Fortaleza, para cada año del horizonte de evaluación;
b) Resultados de las simulaciones dinámicas realizadas para el análisis de Robustez de Tensión
y Frecuencia, incluyendo el valor de los indicadores de desempeño;
c) Conjunto de medidas, incluyendo instalaciones, servicios o reforzamientos de red, así como
aquellas restricciones operacionales orientadas a robustecer el SI y a garantizar el
cumplimiento de los estándares de seguridad establecidos en la NTSyCS y de los
requerimientos del presente Anexo Técnico, junto con su correspondiente justificación
técnica. Dichas medidas deberán clasificarse según tipo de aporte a la robustez que realizan,
Comisión Nacional de Energía 2 de 22

—–——– Título 1 Aspectos generales
el año a partir del cual la medida podría ser necesaria y el Área de Tensión (“AdT”) o Área de
Frecuencia (“AdF”) en la que impactan, según corresponda; y,
d) Niveles mínimos esperados de cortocircuito ( de acuerdo con sus siglas en inglés “Short
Circuit Level”) y factores agregados de interacción IBR ( definido en el Artículo 4-8 del
𝑆𝑆𝑆𝑆𝑆𝑆
Anexo Técnico de Exigencias Mínimas de Instalaciones Basadas en Convertidores que se
𝐾𝐾
conecten al Sistema Eléctrico Nacional) en las barras del SI con niveles de tensión iguales o
superiores a 66 kV, para cada año considerado dentro del horizonte de evaluación.
Artículo 1-5 Alcance del Estudio
El conjunto de medidas que se deriven de este Estudio no tendrá carácter vinculante y no darán a
lugar, por sí mismas, a procesos de licitación de nueva infraestructura ni a la imposición de
restricciones operacionales a UGBC. El Estudio podrá ser considerado como un insumo técnico para
los procesos de planificación y operación del SI, incluyendo el Estudio de Servicios Complementarios,
el Estudio de Restricciones del Sistema de Transmisión, entre otros.
La calificación de un área como “área débil de frecuencia” o “área débil de tensión” tendrá vigencia
desde la fecha de publicación del Estudio por parte del Coordinador hasta la publicación del
siguiente Estudio.
Artículo 1-6 Conjunto de medidas que contribuyen a robustecer el SI
Para el Estudio el Coordinador deberá considerar un conjunto de medidas orientadas a robustecer
el SI cuando ello resulte necesario. Dicho conjunto podrá incluir tres tipos de medidas, clasificadas
de la siguiente forma:
a) Servicios Complementarios con recursos existentes: Servicios Complementarios prestados
en base a recursos e infraestructura existentes en el SI.
b) Servicios Complementarios con nuevos recursos: Servicios Complementarios basados en
nuevos recursos e infraestructura.
c) Ajustes en la lógica de control de IBR: comprenden ajustes o cambios en la lógica de control
de estas instalaciones, tales como la modificación de parámetros de control (como
ganancias), del modo de operación (de IBR GFL a IBR GFM o viceversa), cambio de prioridad
de inyección de corriente ante fallas (nivel de aporte de potencia activa o reactiva), entre
otros.
Artículo 1-7 Publicación del Estudio
El Coordinador anualmente elaborará y publicará en su sitio web el Estudio, junto con los
antecedentes y bases de datos que sustentan sus resultados, de acuerdo con el calendario señalado
en el Artículo 1-9 de la NTSyCS. Con todo, su publicación deberá ser realizada con anterioridad a la
emisión del Informe de SSCC.
Comisión Nacional de Energía 3 de 22

—–——– Título 1 Aspectos generales
Artículo 1-8 Informe preliminar y final del Estudio
El Coordinador elaborará una versión preliminar del Estudio el cual será publicado en su sitio web,
junto con los antecedentes y bases de datos que sustentan sus resultados, para que los interesados
realicen sus observaciones, en el formato y plazo que establezca el Coordinador. El plazo de
observaciones deberá ser de, al menos, 15 días. Los formatos para realizar las observaciones que
establezca el Coordinador deberán, al menos, asegurar la debida individualización del interesado
que formula las observaciones.
Terminado el periodo de observaciones, el Coordinador deberá analizar las observaciones, y luego
emitir la versión final del Estudio junto con un informe consolidado de respuestas a las observaciones
recibidas.
Artículo 1-9 Actualización del Estudio anual
El Coordinador podrá justificadamente actualizar el Estudio indicado en el Artículo 1-7 del presente
Anexo Técnico en caso de que se produzcan interconexiones, modificaciones o retiros relevantes de
instalaciones que puedan afectar la seguridad y calidad de servicio del SI y que no hayan sido
considerados en el Estudio vigente.
En todo caso, las actualizaciones al Estudio deberán someterse a lo señalado en el Artículo 1-8 del
presente Anexo Técnico.
Comisión Nacional de Energía 4 de 22

—–——– Título 2 Funciones y obligaciones
Título 2 Funciones y obligaciones
Artículo 2-1 Funciones y obligaciones del Coordinador
Para efectos del cumplimiento de lo dispuesto en el presente Anexo Técnico, el Coordinador deberá:
a) Solicitar a los Coordinados la información y antecedentes que se requieran para el desarrollo
del Estudio por medio de los formatos que establecerá y publicará en su sitio web; y,
b) Desarrollar el Estudio conforme a la metodología establecida en el presente Anexo Técnico.
Artículo 2-2 Obligaciones de los Coordinados
Para efectos del cumplimiento de lo dispuesto en el presente Anexo Técnico, los Coordinados
deberán:
a) Proporcionar al Coordinador toda la información técnica y antecedentes que este requiera
para la realización del Estudio;
b) Informar oportunamente sobre cualquier actualización relativa a ajustes, indisponibilidades
o limitaciones operacionales de sus instalaciones; y,
c) Ajustar los parámetros técnicos de sus instalaciones conforme a los requerimientos
instruidos por el Coordinador.
Comisión Nacional de Energía 5 de 22

—–——– Título 3 Procedimiento para realizar el Estudio
Título 3 Procedimiento para realizar el Estudio
Artículo 3-1 Consideraciones y horizonte de evaluación del Estudio
El Estudio deberá contemplar un horizonte de evaluación de, al menos, cinco años, considerando el
análisis detallado de la Robustez del sistema proyectado para los años , y . Si es el año en
que se realiza el Estudio, entonces se tiene que .
𝑇𝑇1 𝑇𝑇3 𝑇𝑇5 𝑇𝑇0
La proyección del SI deberá considerar, al menos𝑇𝑇,1 lo= si1gu+ie𝑇𝑇n0te:
a) Las instalaciones declaradas en construcción, así como aquellas derivadas del plan de
expansión o que hayan sido autorizadas en conformidad con el artículo 91°bis o el artículo
102° de la Ley, y que se espera que su fecha de Entrada en Operación se encuentre dentro
del horizonte de evaluación considerado en el Estudio;
b) La nueva infraestructura para la prestación de Servicios Complementarios a que hace
referencia el artículo 72°-7 de la Ley, y que se espera que su fecha de Entrada en Operación
se encuentre dentro del horizonte de evaluación considerado en el Estudio;
c) El retiro, modificación relevante, desconexión o cese de operaciones de instalaciones que
le hayan sido comunicadas de conformidad con el Artículo 72°-18 de la Ley; y,
d) Los mantenimientos preventivos mayores aprobados por el Coordinador, en conformidad
con el Anexo Técnico “Programa de Mantenimiento Preventivo Mayor” de la NTSyCS.
En caso de que la información técnica disponible de las instalaciones sea insuficiente para su
adecuada modelación dinámica, el Coordinador podrá solicitar a los Coordinados los antecedentes
técnicos que requiera para dichos fines.
Artículo 3-2 Metodología para el desarrollo del Estudio
La Figura 1 muestra la metodología general para el desarrollo del Estudio, la cual se compone de
cuatro etapas principales. Las primeras tres etapas tienen por objetivo establecer las condiciones
base y escenarios a considerar en el análisis. La cuarta etapa corresponde al análisis técnico de la
Robustez, el cual primero contempla la evaluación de Fortaleza y posteriormente, la evaluación de
la Robustez de Frecuencia.
Comisión Nacional de Energía 6 de 22

—–——– Título 3 Procedimiento para realizar el Estudio
Figura 1: diagrama metodológico para el desarrollo del Estudio
La primera etapa de la metodología consiste en definir, para los años , y , los escenarios de
operación a considerar en el análisis. Para ello, el Coordinador deberá seleccionar justificadamente
𝑇𝑇1 𝑇𝑇3 𝑇𝑇5
un conjunto acotado de configuraciones de despacho que sean creíbles, pero exigentes desde el
punto de vista de la Robustez de Frecuencia y de Tensión.
Luego, para cada año del horizonte de evaluación, se determinan las áreas del SI que comparten
características eléctricas y recursos de control similares en términos de Robustez de Frecuencia y de
Tensión, definiéndose AdF y AdT, respectivamente. Esta clasificación tiene por finalidad estructurar
y focalizar el análisis, facilitar la interpretación de los resultados y orientar la identificación y
localización de eventuales medidas correctivas. Posteriormente, se define el conjunto de
contingencias a simular en el Estudio.
Una vez completadas estas tres etapas, se procede con el análisis de la Robustez de Frecuencia y de
Tensión mediante simulaciones dinámicas en el dominio del tiempo a frecuencia fundamental
(simulaciones RMS, “Root Mean Square” por sus siglas en inglés).
En los casos en que sea necesario representar fenómenos rápidos y exista un modelo
electromagnético representativo del SEN, el Coordinador podrá efectuar simulaciones
electromagnéticas (EMT “Electromagnetic Transient”, por sus siglas en inglés) como complemento
del análisis RMS, o bien, cuando la naturaleza del fenómeno así lo requiera, realizar el análisis de
Robustez exclusivamente en base a simulaciones EMT.
Artículo 3-3 Base de datos
La base de datos para la evaluación de la Robustez deberá contener toda la información necesaria
para representar los diferentes escenarios de operación a considerar en el Estudio para los años ,
y . La proyección del SI incluida en la base de datos se deberá elaborar conforme a lo indicado
𝑇𝑇1
en el Artículo 3-1 del presente Anexo Técnico.
𝑇𝑇3 𝑇𝑇5
Comisión Nacional de Energía 7 de 22

—–——– Título 3 Procedimiento para realizar el Estudio
Artículo 3-4 Modelo dinámico del SI proyectado
El modelo dinámico del SI proyectado para los años , y deberá ser elaborado considerando
la información contenida en la base de datos señalada en el Artículo 3-3 del presente Anexo Técnico.
𝑇𝑇1 𝑇𝑇3 𝑇𝑇5
El modelo deberá representar la topología proyectada del SI, incorporando instalaciones y nueva
infraestructura que se prevea estén operativas dentro del período de análisis.
El modelo dinámico proyectado deberá incluir las unidades generadoras y Sistemas de
Almacenamiento de Energía con sus respectivos sistemas de control, así como todo componente
relevante para la adecuada representación del comportamiento dinámico del SI. Para la nueva
infraestructura proyectada deberán emplearse modelos consistentes con la información técnica
disponible de cada instalación. En caso de no existir antecedentes suficientes, se podrán utilizar
modelos genéricos desarrollados por organismos internacionales reconocidos en el sector1.
Artículo 3-5 Escenarios de operación
Para la identificación de los escenarios de operación a considerar en el Estudio, el Coordinador
deberá identificar, para los años y un conjunto acotado de configuraciones de despacho
que sean creíbles, pero exigentes desde el punto de vista de la Robustez de Frecuencia y de Tensión.
𝑇𝑇1,𝑇𝑇3 𝑇𝑇5
Los escenarios no deberán incluir restricciones operacionales tales como inercia mínima por área o
despacho forzado de unidades sincrónicas. Cada año considerado en el Estudio deberá incluir, al
menos, los siguientes escenarios:
a) Alta demanda neta.
b) Baja demanda neta.
c) Alto nivel de transferencias entre norte y centro-sur del SI.
d) Bajo nivel de transferencias entre norte y centro-sur del SI.
Para cada uno de los escenarios de operación considerados en un año , el Coordinador deberá
calcular el nivel mínimo esperado de potencia de cortocircuito ( ) en, a′l menos, las barras del SI
𝑇𝑇
con niveles de tensión iguales o superiores a 66 kV. Para fines de estos cálculos no se deberá
𝑆𝑆𝑆𝑆𝑆𝑆
considerar el aporte de IBR GFL a los niveles de cortocircuito.
El nivel mínimo esperado de potencia de cortocircuito en una barra del SI ( ) se define como:
′
𝑇𝑇
𝑗𝑗 𝑆𝑆𝑆𝑆𝑆𝑆𝑗𝑗
′ ′ 𝑀𝑀
𝑇𝑇 𝐸𝐸𝑘𝑘𝑇𝑇
𝑆𝑆𝑆𝑆𝑆𝑆𝑗𝑗 =m𝑘𝑘in�𝑠𝑠𝑠𝑠𝑠𝑠𝑗𝑗 �
𝑘𝑘=1
1 Western Electricity Coordinating Council (WECC) [wecc.org], International Electrotechnical Commission (IEC) [iec.ch], IEEE
Xplore [ieeexplore.ieee.org], entre otros organismos.
Comisión Nacional de Energía 8 de 22

—–——– Título 3 Procedimiento para realizar el Estudio
Donde corresponde a la potencia de cortocircuito trifásica disponible en la barra , expresada
′
en MVA2, p 𝐸𝐸 a 𝑘𝑘 r 𝑇𝑇 a el escenario del año y corresponde a la cantidad de escenarios considerados
𝑠𝑠𝑠𝑠𝑠𝑠𝑗𝑗 𝑗𝑗
para dicho año. ′
𝐸𝐸𝑘𝑘 𝑇𝑇 𝑀𝑀
Artículo 3-6 Indicadores para identificación de áreas
El Estudio contempla la determinación de las AdT y AdF, definidas como subsistemas del SI que
comparten características eléctricas y recursos de control similares desde la perspectiva de la
Robustez de Tensión y de Frecuencia, respectivamente. Para la identificación de las AdT y AdF, el
Coordinador deberá utilizar los siguientes indicadores:
a) Sensibilidad de la tensión respecto a variaciones en los flujos de potencia reactiva por barra
( ): indicador que cuantifica la variación del módulo de la tensión en una barra ante
un cambio en la potencia reactiva inyectada o absorbida en la misma barra. Este indicador
∆𝑈𝑈/∆𝑄𝑄
deberá utilizarse para la definición de AdT.
b) Inercia sincrónica equivalente por barra: indicador que representa la inercia equivalente
“vista” desde cada barra del SI, proporcionando información respecto de la distribución
espacial de la inercia sincrónica en la red. Este indicador deberá utilizarse para la definición
de Adf. La inercia sincrónica equivalente en la barra se calcula mediante la siguiente
expresión:
𝑖𝑖
𝑁𝑁
𝐻𝐻𝑖𝑖 = � 𝐷𝐷𝑖𝑖𝑖𝑖𝐻𝐻𝑖𝑖
𝑖𝑖∈𝐺𝐺𝐺𝐺
Donde, corresponde a un índice de proximidad en por unidad entre la barra y la
barra de inyección del generador , corresponde a la inercia sincrónica en segundos
𝐷𝐷𝑖𝑖𝑖𝑖 𝑖𝑖
del generador y la cantidad de generadores sincrónicos interconectados al SI. El índice
𝑔𝑔 𝐻𝐻𝑖𝑖
de proximidad eléctrica se calcula según la siguiente fórmula:
𝑔𝑔 𝑁𝑁
𝐷𝐷𝑖𝑖𝑖𝑖
𝑍𝑍𝑖𝑖𝑖𝑖
𝐷𝐷𝑖𝑖𝑖𝑖 = � �
𝑍𝑍𝑖𝑖𝑖𝑖
Donde es la impedancia en paralelo de la barra y es la impedancia equivalente
entre las barras y , la que se obtiene al invertir la matriz de admitancia del sistema.
𝑍𝑍𝑖𝑖𝑖𝑖 𝑔𝑔 𝑍𝑍𝑖𝑖𝑖𝑖
𝑖𝑖 𝑔𝑔
2 A efectos del cálculo de cortocircuitos, se deberá utilizar el método completo, el cual se basa en una técnica de
superposición. El método completo utiliza un flujo de potencia para representar la condición pre-falla del sistema (para
tensiones y ángulos), con el fin de determinar las corrientes operativas de un sistema que no esté en condiciones de vacío.
Comisión Nacional de Energía 9 de 22

| —–——–         |                                                 |     |     |     | Título 3 Procedimiento para realizar el Estudio  |     |     |
| ------------- | ----------------------------------------------- | --- | --- | --- | ------------------------------------------------ | --- | --- |
| Artículo 3-7  | Determinación de áreas de frecuencia y tensión  |     |     |     |                                                  |     |     |
Para cada año analizado, el Coordinador deberá identificar las AdF y AdT del SI mediante la aplicación
de un método de agrupamiento sobre las barras del SI, considerando los indicadores definidos en el
Artículo 3-6 del presente Anexo Técnico:
a)  Sensibilidad de la tensión respecto de las variaciones en el flujo de potencia reactiva por
barra para la identificación de las AdT.
b)  Inercia sincrónica equivalente por barra para la identificación de las AdF.
El objetivo del método de agrupamiento es minimizar, sobre todos los escenarios de un año  , el
error cuadrático medio entre el valor del indicador en cada barra y el valor representativo de su área
𝑇𝑇
(centroide) en el escenario correspondiente. Sea   el número de áreas (por definir),
el conjunto de todas las barras del sistema,   el conjunto de escenarios del año  ,
|     |     |     |     | 𝐾𝐾  |     | 𝐵𝐵  | = {1,…,𝑀𝑀} |
| --- | --- | --- | --- | --- | --- | --- | ---------- |
el valor del indicador para identificación de área de la barra   en el escenario  . Entonces, el
|     |     |     | E   | = {𝐸𝐸1,…,𝐸𝐸𝑁𝑁} |     |     | 𝑇𝑇 𝑥𝑥𝑖𝑖𝑗𝑗 |
| --- | --- | --- | --- | -------------- | --- | --- | --------- |
problema de agrupamiento se plantea como:
|     |     |     |     |     | 𝑖𝑖  | 𝐸𝐸𝑗𝑗 |     |
| --- | --- | --- | --- | --- | --- | ---- | --- |
|     |     |     | 𝐾𝐾  |     |     |      |     |
2
1
|     |     | min | ��  | � 𝑧𝑧𝑖𝑖𝑘𝑘�𝑥𝑥𝑖𝑖𝑗𝑗 | −𝜇𝜇𝑖𝑖𝑗𝑗� |     |     |
| --- | --- | --- | --- | --------------- | -------- | --- | --- |
𝑀𝑀𝑁𝑁𝑘𝑘=1𝑖𝑖∈𝐵𝐵𝐸𝐸𝑗𝑗∈E
Sujeto a:

𝐾𝐾
|     | �𝑧𝑧𝑖𝑖𝑘𝑘 = | 1, ∀𝑖𝑖 ∈ | 𝐵𝐵  |     |     |     |     |
| --- | --------- | -------- | --- | --- | --- | --- | --- |
𝑘𝑘=1

�𝑧𝑧𝑖𝑖𝑘𝑘
|     | ≥   | 1, ∀𝑖𝑖 ∈𝐵𝐵,∀𝑘𝑘 | = 1,…,𝐾𝐾 |     |     |     |     |
| --- | --- | -------------- | -------- | --- | --- | --- | --- |
𝑖𝑖∈𝐵𝐵
|     |                 |       |                 |     |     |     |     |
| --- | --------------- | ----- | --------------- | --- | --- | --- | --- |
|     | 𝑧𝑧𝑖𝑖𝑘𝑘 ∈ {0,1}, | ∀𝑖𝑖 ∈ | 𝐵𝐵,∀𝑘𝑘 = 1,…,𝐾𝐾 |     |     |     |     |

Donde   corresponde a la variable de asignación de la barra   al área  , es decir,   si
la barra   pertenece al área  ,   si no, y   corresponde al centroide del grupo   en el escenario  ,
| 𝑧𝑧𝑖𝑖𝑘𝑘𝜖𝜖{0,1} |     |     |     |     | 𝑖𝑖  | 𝑘𝑘  | 𝑧𝑧𝑖𝑖𝑘𝑘 = 1 |
| ------------- | --- | --- | --- | --- | --- | --- | ---------- |
es decir:
| 𝑖𝑖  |     | 𝑘𝑘 0 | 𝜇𝜇𝑖𝑖𝑗𝑗 |     |     | 𝑘𝑘  | 𝐸𝐸𝑗𝑗 |
| --- | --- | ---- | ------ | --- | --- | --- | ---- |

∑𝑖𝑖∈𝐵𝐵𝑧𝑧𝑖𝑖𝑘𝑘𝑥𝑥𝑖𝑖𝑗𝑗
𝜇𝜇𝑘𝑘𝑗𝑗 =
Adicionalmente, el método de agrupamiento de∑b𝑖𝑖e∈𝐵𝐵rá  𝑖𝑖i𝑘𝑘ncorporar una restricción de conectividad
𝑧𝑧
topológica, con tal de que cada área solo incluya barras conectadas sin atravesar otras áreas. Sea
  el  grado  de  la  red,  donde    es  el  conjunto  de  pares  de  barras  unidas
directamente por una línea o un transformador y   el conjunto de barras asignadas al área  , es
| 𝐺𝐺 = (𝐵𝐵,ℒ) |     |     | ℒ ⊆ | 𝐵𝐵 x 𝐵𝐵 |     |     |     |
| ----------- | --- | --- | --- | ------- | --- | --- | --- |
decir,  . La restricción de conectividad topológica establece que el subgrafo
|     |     |     |     | 𝑆𝑆𝑘𝑘 |     |     | 𝑘𝑘  |
| --- | --- | --- | --- | ---- | --- | --- | --- |
inducido por   sea conexo, es decir, para cualquier par de barras   existe un camino
| 𝑆𝑆𝑘𝑘                        | = {𝑖𝑖 ∈ 𝐵𝐵:𝑧𝑧𝑖𝑖𝑘𝑘 | = 1 }              |     |     |           |      |     |
| --------------------------- | ----------------- | ------------------ | --- | --- | --------- | ---- | --- |
| contenido completamente en  |                   |  que las conecta:  |     |     |           |      |     |
|                             | 𝑆𝑆𝑘𝑘              |                    |     |     | 𝑏𝑏𝑖𝑖,𝑏𝑏𝑗𝑗 | 𝑆𝑆𝑘𝑘 |     |
∈
𝑆𝑆𝑘𝑘
| Comisión Nacional de Energía  |     |     |     |     |     |     |  10 de 22  |
| ----------------------------- | --- | --- | --- | --- | --- | --- | ---------- |

—–——– Título 3 Procedimiento para realizar el Estudio
La can∀ti𝑏𝑏d𝑖𝑖a,d𝑏𝑏𝑗𝑗 d∈e á𝑆𝑆r𝑘𝑘e,a𝑏𝑏s𝑖𝑖 d≠eb𝑏𝑏e𝑗𝑗r,á∃ d 𝑏𝑏e0t,e𝑏𝑏r1m,…ina,𝑏𝑏rs𝑚𝑚e e∈n𝑆𝑆 f𝑘𝑘u:n 𝑏𝑏ci0ó=n d𝑏𝑏e𝑖𝑖l, e𝑏𝑏r𝑚𝑚ro=r a𝑏𝑏s𝑗𝑗o,c(i𝑏𝑏ad𝑙𝑙−o1 a,𝑏𝑏l p𝑙𝑙)ro∈ceℒs,o∀ d𝑠𝑠e= ag1r,u…pa,m𝑚𝑚iento.
Cabe señalar que la cantidad de AdF y AdT pueden diferir entre sí, producto de que representan
fenómenos de distinta naturaleza.
La Figura 2 ilustra, a modo referencial, un posible resultado para las AdF y AdT en el caso de que el
Estudio considere dos escenarios para los años y ; y tres escenarios para el año . En la figura,
los conjuntos , corresponden a los escenarios
𝑇𝑇1 𝑇𝑇3 𝑇𝑇5
definidos para los años , y , respectivamente. De la Figura 2 se observa que, si bien cada año
{𝐸𝐸1𝑇𝑇1;𝐸𝐸2𝑇𝑇1} {𝐸𝐸1𝑇𝑇3;𝐸𝐸2𝑇𝑇3} 𝑦𝑦 {𝐸𝐸1𝑇𝑇5;𝐸𝐸2𝑇𝑇5;𝐸𝐸3𝑇𝑇5}
considera distintos escenarios, las AdF y AdT son las mismas dentro de un mismo año.
𝑇𝑇1 𝑇𝑇3 𝑇𝑇5
𝑇𝑇
Figura 2: representación esquemática de Adf y AdT para cada año en estudio (ejemplo ilustrativo)
Artículo 3-8 Determinación de contingencias
Para cada una de las AdF y AdT de cada año de evaluación, el Coordinador deberá definir un conjunto
de Contingencias Simples a ser consideradas en el análisis de Robustez. Dicho conjunto deberá
incluir, al menos:
a) Una Contingencia Simple de Severidad 4a para cada AdT. A efectos del presente Anexo
Técnico, se entenderá como Severidad 4a un cortocircuito trifásico a tierra con impedancia
de falla de hasta 1 Ohm, ocurrido en un circuito de líneas de doble circuito o en una línea de
simple circuito con Enmallamiento, seguido de la desconexión del circuito fallado en tiempo
normal por acción de su sistema de protección. Para el cálculo de cortocircuito no se deberá
considerar el aporte de corriente de IBR GFL, y la impedancia de falla deberá ser tal que, la
Comisión Nacional de Energía 11 de 22

| —–——–  |     |   Título 3 Procedimiento para realizar el Estudio  |     |     |
| ------ | --- | -------------------------------------------------- | --- | --- |
corriente cortocircuito sea elevada, aunque ligeramente inferior a la correspondiente a una
falla con impedancia cero.
b)  Una Contingencia Simple de Severidad 5 para cada AdF.
Adicionalmente, el Coordinador podrá considerar en el análisis otras Contingencias Simples que
resulten relevantes para la evaluación de la Robustez en ciertas áreas del SI. En los casos en que una
contingencia genere efectos tanto en la Robustez de Tensión como en la de Frecuencia, dicha
contingencia deberá considerarse en la evaluación de ambas dimensiones de la Robustez.
La Figura 3 ilustra, de manera referencial, las contingencias asociadas a cada AdF y AdT para el mismo
caso presentado en la Figura 2. En la Figura 3, el símbolo “*” corresponde a una Contingencia Simple
de Severidad 4a, mientras que el símbolo “*” a una Contingencia Simple de Severidad 5. De la Figura
3 se observa que cada una de las AdF y AdT tiene asociada, en los distintos escenarios analizados, al
menos una contingencia simple de Severidad 4a en el caso de las AdT y de Severidad 5 en el caso de
las AdF, salvo algunos casos en que se identifican dos contingencias por área. En particular, estas
excepciones se presentan en:
c)  En el área de tensión   del escenario  ;   del escenario  , y   del
| escenario   las cuales incluyen dos contingencias de Severidad 4a; y,  |         |                |        |         |
| ---------------------------------------------------------------------- | ------- | -------------- | ------ | ------- |
|                                                                        | 𝐴𝐴𝐴𝐴𝑇𝑇1 | 𝐸𝐸2𝑇𝑇3 𝐴𝐴𝐴𝐴𝑇𝑇2 | 𝐸𝐸2𝑇𝑇5 | 𝐴𝐴𝐴𝐴𝑇𝑇1 |
d)  Las áreas d𝐸𝐸e3 f𝑇𝑇r5ecuencia   del escenario   y   del escenario   que incluyen dos
contingencias de Severidad 5.
|     | 𝐴𝐴𝐴𝐴𝐴𝐴2 | 𝐸𝐸2𝑇𝑇1 𝐴𝐴𝐴𝐴𝐴𝐴2 | 𝐸𝐸2𝑇𝑇5 |     |
| --- | ------- | -------------- | ------ | --- |

Figura 3: representación de las contingencias asociadas a las AdF y AdT (ejemplo ilustrativo)
| Comisión Nacional de Energía  |     |     |     |  12 de 22  |
| ----------------------------- | --- | --- | --- | ---------- |

—–——– Título 3 Procedimiento para realizar el Estudio
Artículo 3-9 Indicadores de desempeño dinámico
Según lo indicado en el Artículo 1-4 del presente Anexo Técnico, la robustez se evalúa en función del
desempeño dinámico del SI durante contingencias, utilizando para ello indicadores de desempeño
que permitan evaluar la respuesta dinámica del SI proyectado. Los indicadores de desempeño a
considerar deberán incluir, al menos, los siguientes:
a) Índice de desempeño dinámico (IDD) para fallas de Severidad 4a, calculado conforme a lo
establecido en el Artículo 3-10 del presente Anexo Técnico.
b) Frecuencia mínima y RoCoF para contingencias de Severidad 5, calculados conforme a lo
establecido en el Artículo 3-11 del presente Anexo Técnico.
Sin perjuicio de lo anterior, el Coordinador podrá incorporar indicadores adicionales cuando estos
resulten pertinentes para la evaluación del desempeño dinámico del SI.
Los indicadores de desempeño dinámico deberán ser aplicados en cada una de las fases de análisis
descritas en los Artículo 3-13 y Artículo 3-15 del presente Anexo Técnico, según corresponda.
Artículo 3-10 Cálculo del índice de desempeño dinámico
El índice de desempeño dinámico en una barra ( ), para un cortocircuito de Severidad 4a, se define
como el área comprendida entre el valor eficaz de la tensión en dicha barra antes de la falla y su evolución
𝑗𝑗 𝐼𝐼𝐷𝐷𝐷𝐷𝑗𝑗
temporal durante el Régimen Transitorio. El se calcula mediante la siguiente expresión:
𝐼𝐼𝐷𝐷𝐷𝐷𝑗𝑗
𝑡𝑡𝑓𝑓𝑓𝑓
𝐼𝐼𝐷𝐷𝐷𝐷𝑗𝑗 = � �𝑣𝑣𝑗𝑗(𝑡𝑡)−𝑣𝑣𝑗𝑗,0�𝐴𝐴𝑡𝑡
𝑡𝑡𝑓𝑓
Donde se tiene que:
: índice de desempeño dinámico en la barra , en por unidad por segundo.
𝐼𝐼𝐷𝐷𝐷𝐷𝑗𝑗: valor eficaz de la tensión en la barra , en po𝑗𝑗r unidad.
𝑣𝑣𝑗𝑗(𝑡𝑡: )valor eficaz de la tensión en la barra a𝑗𝑗ntes de la falla, en por unidad.
𝑣𝑣𝑗𝑗,:0 instante en el cual ocurre la falla, expre𝑗𝑗sado en segundos.
𝑡𝑡𝑓𝑓 : instante hasta el cual se desea evaluar el indicador, expresado en segundos.
L𝑡𝑡𝑓𝑓a𝑓𝑓 Figura 4 ilustra gráficamente el , destacando el área definida entre el valor eficaz de la tensión antes
de la falla y su evolución temporal durante el Régimen Transitorio.
𝐼𝐼𝐷𝐷𝐷𝐷
Comisión Nacional de Energía 13 de 22

—–——– Título 3 Procedimiento para realizar el Estudio
Figura 4: representación del IDD
Artículo 3-11 Cálculo de frecuencia mínima y RoCoF
La Tasa de Cambio de la Frecuencia (RoCoF) en una barra del SI, evaluada en una ventana de tiempo
definida a partir del instante de ocurrencia de una Contingencia Simple de Severidad 5, se calcula
j
conforme a la siguiente expresión:
∆
𝐴𝐴𝑗𝑗�𝑡𝑡𝑓𝑓 +∆�−𝐴𝐴𝑗𝑗(𝑡𝑡𝑓𝑓)
𝑅𝑅𝑅𝑅𝑆𝑆𝑅𝑅𝐹𝐹𝑗𝑗 =
Donde,
∆
: corresponde a la Tasa de Cambio de Frecuencia en la barra , medida en [Hz/s].
𝑅𝑅𝑅𝑅: 𝑆𝑆co𝑅𝑅r𝐹𝐹r𝑗𝑗esponde al instante de tiempo en el cual ocurre la perturbació𝑗𝑗n, en segundos.
𝑡𝑡𝑓𝑓: ventana de tiempo en la cual se debe calcular el RoCoF, en segundos. A efectos del presente
Estudio se considera una ventana de 500 milisegundos.
∆
: corresponde al valor de la frecuencia en la barra en el instante , en [Hz].
L𝐴𝐴𝑗𝑗a( 𝑡𝑡fr)ecuencia mínima en una barra del SI, luego d𝑗𝑗e ocurrida un𝑡𝑡a contingencia de Severidad 5,
corresponde al menor valor que alcanza la frecuencia en dicha barra desde el instante en que se inicia
j
la perturbación hasta la recuperación del régimen permanente.
Artículo 3-12 Medidas que pueden robustecer el SI
Para el desarrollo del análisis establecido en el Artículo 3-13 y Artículo 3-15 del presente Anexo
Técnico, el Coordinador deberá identificar, para cada año dentro del horizonte de evaluación del
Estudio, un conjunto de posibles medidas que puedan contribuir a la Robustez de Frecuencia y de
Tensión del SI. Dicho conjunto deberá incluir, al menos, las siguientes categorías:
(M-1) Todos aquellos recursos técnicos e infraestructura disponibles en el SI que, en el
marco de los Servicios Complementarios o funcionalidades habilitadas en las distintas
Comisión Nacional de Energía 14 de 22

| —–——–  |     |     |     |     |     |   Título 3 Procedimiento para realizar el Estudio  |     |     |     |
| ------ | --- | --- | --- | --- | --- | -------------------------------------------------- | --- | --- | --- |
instalaciones, estén en condiciones de prestar servicios que mejoren la Robustez de
frecuencia y/o Fortaleza del SI.
(M-2)  Alternativas de nuevas instalaciones, adecuaciones de infraestructura/instalaciones
existentes o incorporación de nuevas instalaciones con el potencial de robustecer áreas
débiles y cuya entrada en operación sea factible dentro del horizonte de evaluación del
Estudio.
(M-3)  Ajustes en la lógica de control de IBR que contribuyan a la Robustez del SI.
En cuanto a las medidas del tipo (M-3), estas comprenden, entre otras, ajustes en los sistemas de
control de las IBR, incluyendo la reconfiguración de su modo de operación (pasando de modo GFL a
GFM o viceversa), cuando corresponda, y el cambio de prioridades de inyección de corriente
activa/reactiva en IBR GFL durante fallas, siempre que tales ajustes sean técnicamente factibles y
mejoren el desempeño dinámico del SI.
Para la selección de potenciales medidas indicadas en el grupo (M-2), el Coordinador deberá adoptar
un enfoque de neutralidad tecnológica, considerando diferentes opciones y tecnologías disponibles
en el mercado que, al momento de la ejecución del Estudio, puedan contribuir a la Robustez del SI.
La  Tabla  1  presenta  ejemplos  de  carácter  referencial  de  recursos  que  pueden  aportar  al
fortalecimiento de un sistema eléctrico, indicando el tipo de Robustez al cual contribuyen. No
obstante, es importante señalar que existen otras alternativas tecnológicas capaces de aportar a la
Robustez, muchas de las cuales corresponden a combinaciones de distintas tecnologías.
Tabla 1: ejemplos de recursos para robustecer un sistema eléctrico
Tipo de  ¿Contribuye a la  ¿Contribuye a robustez de  Particularidades
|     | recurso  | robustez de frecuencia?  |     |     |     | tensión?  |     | técnicas  |     |
| --- | -------- | ------------------------ | --- | --- | --- | --------- | --- | --------- | --- |
Sí
Sí
|     |      |     |     |     | •                               |     |     | •                   |     |
| --- | ---- | --- | --- | --- | ------------------------------- | --- | --- | ------------------- | --- |
|     | UGS  |     |     |     | Control de tensión y capacidad  |     |     | Soporte post-falla  |     |
•  Inercia rotacional
de potencia reactiva
Sí
Sí
•  Control de tensión y capacidad
|     |          | •        |            |     |     |     |     | •                   |     |
| --- | -------- | -------- | ---------- | --- | --- | --- | --- | ------------------- | --- |
|     | IBR GFM  | Inercia  | sintética  | o   |     |     |     | Soporte post-falla  |     |
de potencia reactiva, similar a
virtual
una máquina sincrónica
Parcial
|     |     |     | Parcial  |     |     |     |     | •  Posible  aporte  | post- |
| --- | --- | --- | -------- | --- | --- | --- | --- | ------------------- | ----- |
•  Aporte al control de tensión y
|     |          | •  Aporte               | limitado  | en  |                                 |                        |     | falla  en                | función  del  |
| --- | -------- | ----------------------- | --------- | --- | ------------------------------- | ---------------------- | --- | ------------------------ | ------------- |
|     | IBR GFL  |                         |           |     | capacidad de potencia reactiva  |                        |     |                          |               |
|     |          | función del sistema de  |           |     |                                 |                        |     | sistema de control       |               |
|     |          |                         |           |     | en                              | función  del  sistema  | de  |                          |               |
|     |          | control                 |           |     |                                 |                        |     | •  Sensibles a bajo SCR  |               |
control
Sí
| Condensadores  |            |                        | Sí  |     |                                 |     |     |                     |     |
| -------------- | ---------- | ---------------------- | --- | --- | ------------------------------- | --- | --- | ------------------- | --- |
|                |            |                        |     |     | •                               |     |     | •                   |     |
|                |            |                        |     |     | Control de tensión y capacidad  |     |     | Soporte post-falla  |     |
|                | síncronos  | •  Inercia rotacional  |     |     |                                 |     |     |                     |     |
de potencia reactiva
|     |     |     |     |     |     | Parcial  |     | •  Posible  aporte  | post- |
| --- | --- | --- | --- | --- | --- | -------- | --- | ------------------- | ----- |
SVC  No  •  Regulación  de  tensión  y  falla  en  función  del
|     |     |     |     |     | capacidad de potencia reactiva  |     |     | sistema de control  |       |
| --- | --- | --- | --- | --- | ------------------------------- | --- | --- | ------------------- | ----- |
|     |     |     |     |     |                                 | Sí  |     | •                   |       |
|     |     |     |     |     |                                 |     |     | Posible  aporte     | post- |
STATCOM  No  •  Regulación  de  tensión  y  falla  en  función  del
|                               |     |     |     |     | capacidad de potencia reactiva  |     |     | sistema de control  |            |
| ----------------------------- | --- | --- | --- | --- | ------------------------------- | --- | --- | ------------------- | ---------- |
| Comisión Nacional de Energía  |     |     |     |     |                                 |     |     |                     |  15 de 22  |

—–——– Título 3 Procedimiento para realizar el Estudio
Artículo 3-13 Análisis de Fortaleza o Robustez de Tensión
El análisis de Fortaleza del Estudio tiene por objetivo evaluar la Fortaleza del SI en el corto y mediano
plazo, con el fin de determinar su evolución, identificar tendencias y potenciales áreas débiles, así
como proponer un conjunto de potenciales medidas que permitirían robustecer dichas áreas cuando
ello resulte necesario.
El análisis se desarrolla, para cada año del horizonte de evaluación, mediante simulaciones
dinámicas en el dominio del tiempo, utilizando el modelo dinámico del SI proyectado elaborado
conforme a lo dispuesto en el Artículo 3-4 del presente Anexo Técnico.
El análisis de Fortaleza se estructura en los pasos que se indican a continuación:
(Paso 1) Para cada año en evaluación, el Coordinador deberá simular las contingencias asociadas a
cada una de las AdT, para todos los escenarios de operación definidos conforme al Artículo 3-5 del
presente Anexo Técnico.
En esta etapa, las simulaciones deberán efectuarse sin incorporar medidas orientadas a fortalecer el
SI ni aplicar restricciones de seguridad, con el objeto de caracterizar el desempeño dinámico
intrínseco del sistema y evaluar, de manera objetiva, su nivel de Robustez frente a las contingencias
consideradas.
(Paso 2) Para cada contingencia simulada en el (Paso 1), se debe calcular el IDD conforme a lo
establecido en el Artículo 3-10 del presente Anexo Técnico; considerando que el despeje de la falla
ocurre 120 milisegundos después de iniciada la falla ( milisegundos) y que la
evaluación del indicador se realiza hasta el instante segundos. En caso de que el Estudio
𝑡𝑡𝑑𝑑 −𝑡𝑡𝑓𝑓 = 120
considere indicadores adicionales de desempeño dinámico, estos también deberán ser calculados.
𝑡𝑡𝑓𝑓𝑓𝑓 = 1,12
Considerando nuevamente el mismo caso ilustrativo presentado en la Figura 2, la Figura 5 y Tabla 2
resumen las simulaciones requeridas en el (Paso 1). En este ejemplo, el análisis de Fortaleza
involucra la simulación de un total de 27 contingencias simples de Severidad 4a, asociándose, en
general, una contingencia a cada AdT. Las excepciones se presentan en las siguientes áreas de
tensión: del escenario , del escenario , y del escenario , para las
cuales se consideran dos contingencias de Severidad 4a.
𝐴𝐴𝐴𝐴𝑇𝑇1 𝐸𝐸2𝑇𝑇3 𝐴𝐴𝐴𝐴𝑇𝑇2 𝐸𝐸2𝑇𝑇5 𝐴𝐴𝐴𝐴𝑇𝑇1 𝐸𝐸3𝑇𝑇5
Comisión Nacional de Energía 16 de 22

| —–——–  |     |     |     |     |     | Título 3 Procedimiento para realizar el Estudio  |     |     |     |
| ------ | --- | --- | --- | --- | --- | ------------------------------------------------ | --- | --- | --- |
Figura 5: representación de las contingencias asociadas a las AdT (ejemplo ilustrativo)
Tabla 2: contingencias a simular en cada AdT (ejemplo ilustrativo)
|     |            | Año  |        |        |        |        |        |        |        |
| --- | ---------- | ---- | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
|     | Escenario  |      |        |   𝑻𝑻𝟏𝟏 |        |   𝑻𝑻𝟑𝟑 |        | 𝑻𝑻𝟓𝟓   |        |
|     |            |      | *      | *      | *      | **     | *      | *      | **     |
|     |            |      | 𝐸𝐸1𝑇𝑇1 | 𝐸𝐸2𝑇𝑇1 | 𝐸𝐸1𝑇𝑇3 | 𝐸𝐸2𝑇𝑇3 | 𝐸𝐸1𝑇𝑇5 | 𝐸𝐸2𝑇𝑇5 | 𝐸𝐸3𝑇𝑇5 |
|     |            |      | *      | *      | *      | *      | *      | **     | *      |
𝐴𝐴𝐴𝐴𝑇𝑇1
|     |     |     | *   | *   | *   | *   |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
𝐴𝐴𝐴𝐴𝑇𝑇2
|     |     |     | *   | *   | *   | *   |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
𝐴𝐴𝐴𝐴𝑇𝑇3
|     |     |     |     |     | *   | *   |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
𝐴𝐴𝐴𝐴𝑇𝑇4
| Total de contingencias de  |     | 𝐴𝐴𝐴𝐴𝑇𝑇5 |     |     |     |     |     |     |     |
| -------------------------- | --- | ------- | --- | --- | --- | --- | --- | --- | --- |
|                            |     |         | 4   | 4   | 5   | 6   | 2   | 3   | 3   |
Severidad 4a * por escenario
(Paso 3) Para cada una de las contingencias simuladas según el (Paso 1), se deberán cumplir todos
los estándares aplicables establecidos en la NTSyCS. Sin perjuicio de lo anterior, se deberá verificar,
al menos, que:
i.  Se cumpla lo dispuesto en el Artículo 5-31 de la NTSyCS respecto a la estabilidad del SI frente
a la ocurrencia de una contingencia simple de hasta severidad 7, sin admitir la utilización de
Recursos  Generales  o  Adicionales  de  Control  de  Contingencias  que  impliquen
desprendimientos de carga por frecuencia o por tensión.
ii.  Las tensiones del SI cumplan con el límite inferior de recuperación de tensión definido en el
Artículo 5-34 de la NTSyCS frente a la ocurrencia de una contingencia simple de hasta
severidad 7, sin admitir la utilización de Recursos Generales o Adicionales de Control de
Contingencias que impliquen desprendimientos de carga por frecuencia o por tensión.
Adicionalmente, se deberá verificar que:
iii.  El   calculado en la barra   más cercana al lugar de ocurrencia de la falla cumpla la condición
.
| 𝐼𝐼𝐷𝐷𝐷𝐷 |     |     | 𝑗𝑗  |     |     |     |     |     |     |
| ------ | --- | --- | --- | --- | --- | --- | --- | --- | --- |
Donde el valor 0,16 corresponde al peor valor admisible que puede adquirir el IDD para efectos del
𝐼𝐼𝐷𝐷𝐷𝐷𝑗𝑗
<  0,16
Estudio3.
(Paso 4) Si para un año   determinado existe al menos una contingencia en la cual no se cumple
alguno de los requerimien′tos señalados en el (Paso 3), el AdT asociada a dicha contingencia deberá
𝑇𝑇
ser catalogada como débil, aun cuando el incumplimiento se verifique en un único escenario del año
. En tal caso, deberán aplicarse los pasos (4.a), (4.b), (4.c) y (4.d) descritos a continuación:
′
𝑇𝑇(4.a)  Para el  área  débil  ,  el  Coordinador  deberá analizar  y  proponer  un  conjunto  de
soluciones orientadas a aumentar la fortaleza de dicha área, de manera de garantizar el
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘
cumplimiento de los requerimientos establecidos en el (Paso 3). Las soluciones deberán
considerar medidas del tipo (M-1), (M-2) y (M-3), conforme a la tipificación establecida en
el  Artículo  1-6  del  presente  Anexo  Técnico.  Las  medidas  del  tipo  (M-2)  sólo  podrán

3 Este valor se obtiene tomando como referencia basal la envolvente normativa de recuperación de tensión establecida en
el Artículo 5-34 de la NTSyCS, pero incorporando exigencias adicionales asociadas a la rapidez y calidad de la recuperación
de la tensión, es decir, exigiendo una respuesta más robusta.
| Comisión Nacional de Energía  |     |     |     |     |     |     |     |     |  17 de 22  |
| ----------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | ---------- |

—–——– Título 3 Procedimiento para realizar el Estudio
considerarse si sus plazos de implementación y entrada en operación son compatibles con
el año en que se requiere su aplicación.
Cada solución deberá constituir, por sí sola, una alternativa técnicamente viable que
permita fortalecer el área débil y asegurar el cumplimiento de los requerimientos del
𝑠𝑠𝑖𝑖
(Paso 3). Una solución podrá consistir en una medida individual o en una combinación de
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘
medidas de los tipos (M-1), (M-2) y/o (M-3).
El Coordinador deberá identificar y evaluar múltiples soluciones independientes entre sí, sin
limitarse a proponer una única alternativa, con el objeto de conformar un conjunto de
soluciones técnicamente factibles de implementar. El resultado de esta etapa es un conjunto
de potenciales soluciones , definido como:
′
𝑇𝑇
𝕊𝕊𝐴𝐴𝑑𝑑𝑇𝑇𝑘𝑘 .
′
𝑇𝑇
Donde cada elemento corre
𝕊𝕊
sp𝐴𝐴o𝑑𝑑𝑇𝑇n𝑘𝑘de
=
a
{
u 𝑠𝑠1n
,
a
𝑠𝑠
s2o
,…
luc
𝑠𝑠
ió𝑚𝑚n
}
técnicamente factible que, por sí sola,
permite que el área cumpla con los requerimientos establecidos en el (Paso 3).
𝑠𝑠𝑖𝑖
(4.b) En aquellos casos e𝐴𝐴n𝐴𝐴 q𝑇𝑇𝑘𝑘ue no se identifique ninguna solución factible, esto es, cuando
ninguna medida del tipo (M-1), (M-2) o (M-3), ya sea aplicada de forma individual o
combinada, permita garantizar el cumplimiento de los estándares exigidos en el (Paso 3), el
Coordinador deberá identificar restricciones operacionales aplicables al área débil
correspondiente, para evitar el incumplimiento.
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘
Dichas restricciones podrán incluir, entre otras, la exigencia de una cantidad mínima de UGS
o IBR GFM en operación, o la limitación de la generación de UGBC. Para efectos del Estudio,
estas restricciones deberán aplicarse exclusivamente en el área débil en la que se haya
verificado el incumplimiento.
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘
(4.c) Para cada solución identificada, el Coordinador deberá evaluar y cuantificar la mejora en
los indicadores de desempeño establecidos en el Artículo 3-9 del presente Anexo Técnico,
𝑠𝑠𝑖𝑖
respecto de la condición base, es decir, sin la aplicación de dicha solución (valores obtenidos
en la (Etapa 2)).
Considerando que, para efectos del Estudio, la Robustez se evalúa en función del desempeño
dinámico del SI durante contingencias, la mejora en los indicadores de desempeño
constituye un indicador del aumento de Fortaleza aportado por cada solución. Sin embargo,
dicha mejora no constituye, por sí misma, un criterio de priorización de soluciones. Para una
adecuada priorización, deben considerarse de manera conjunta aspectos técnicos,
incluyendo el aumento de Fortaleza reflejado en los indicadores de desempeño, y
económicos, así como otros criterios que resulten aplicables conforme a la normativa
vigente.
(4.d) Una vez obtenido un conjunto de soluciones factibles para fortalecer una determinada área
débil , el Coordinador deberá seleccionar una solución , de entre todas las soluciones
contenidas en el conjunto e identificadas en el paso (4a), para ser considerada en las
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘 𝑠𝑠∗
′
siguientes simulaciones que𝑇𝑇 se realicen para el mismo año . Concretamente, la solución
𝕊𝕊𝐴𝐴𝑑𝑑𝑇𝑇𝑘𝑘
seleccionada deberá incorporarse en las simulaciones asoc′iadas a las demás áreas de
𝑇𝑇
tensión del mismo año, con . La finalidad de esta selección es fijar un grupo de
𝐴𝐴𝐴𝐴𝑇𝑇𝑗𝑗 𝑗𝑗 ≠ 𝑘𝑘
Comisión Nacional de Energía 18 de 22

| —–——–  |     |   Título 3 Procedimiento para realizar el Estudio  |     |
| ------ | --- | -------------------------------------------------- | --- |
medidas que garantice que el área débil   cumpla con los requerimientos establecidos
en el (Punto 3) en las simulaciones que se realicen para el resto de las AdT del mismo año.
𝐴𝐴𝐴𝐴𝑇𝑇𝑘𝑘
(Paso 5) Una vez concluido el análisis de un año   determinado, para la evaluación de los años
siguientes, las medidas del tipo (M-2) incluidas en ′la solución   de una determinada área débil
𝑇𝑇
deberán considerarse como infraestructura existente para los años siguientes, es decir, como
𝑠𝑠∗
medidas del tipo (M-1).
| Artículo 3-14  Resultados del análisis de Fortaleza   |     |     |     |
| ----------------------------------------------------- | --- | --- | --- |
Como resultado del análisis de Fortaleza descrito en el Artículo 3-13 del presente Anexo Técnico,
aplicado a cada año dentro del horizonte de evaluación del Estudio, se obtendrá:
a)  Conjunto de AdT débiles del SI, para cada año del horizonte de evaluación;
b)  Resultados de las simulaciones dinámicas realizadas, incluyendo el valor de los indicadores
de desempeño correspondientes;
c)  Conjunto de soluciones técnicamente factibles de implementar para robustecer las AdT
débiles y garantizar el cumplimiento de los requerimientos establecidos en el Artículo 3-13
del presente Anexo Técnico; y,
d)  Niveles mínimos esperados de potencia de cortocircuito (SCL) y factores agregados de
interacción IBR ( ) en las barras del SI con niveles de tensión iguales o superiores a 66 kV,
| para cada año del horizonte de evaluación  |     | ,   y  .  |     |
| ------------------------------------------ | --- | --------- | --- |
𝐾𝐾𝑖𝑖
Con respecto al conjunto de soluciones indicadas e𝑇𝑇n1 el𝑇𝑇 l3iter𝑇𝑇a5l c), estas deberán clasificarse según:
i.  Tipo de aporte a la Robustez que realizan;
ii.  Año a partir del cual la solución podría ser necesaria;
iii.  AdT en la cual la medida impacta; y,
iv.  Mejora en los indicadores de desempeño en que se traducen las soluciones.
Considérese nuevamente el caso ilustrativo de la Figura 5. La Tabla 3 a continuación resume las
contingencias simuladas en cada AdT en el (Paso 1), destacando aquellas AdT en las que al menos
una contingencia no cumplió los requerimientos establecidos en el (Paso 3) del Artículo 3-13 del
presente Anexo Técnico. De la Tabla 3 se observa que, en todos los años evaluados, hay un total de
cuatro AdT en las cuales al menos una contingencia no cumple con los requerimientos del Artículo
3-13 del presente Anexo Técnico. En consecuencia, para este ejemplo ilustrativo, las áreas débiles
del SI identificadas para cada año del Estudio son las siguientes:
| •  Para el año  | : áreas de tensión  |  y  .   |     |
| --------------- | ------------------- | ------- | --- |
| •  Para el año  | : áreas de tensión  | .       |     |
|                 | 𝑇𝑇1 𝐴𝐴𝐴𝐴𝑇𝑇1         | 𝐴𝐴𝐴𝐴𝑇𝑇2 |     |
| •  Para el año  | : áreas de tensión  | .       |     |
|                 | 𝑇𝑇3 𝐴𝐴𝐴𝐴𝑇𝑇5         |         |     |

|     | 𝑇𝑇5 𝐴𝐴𝐴𝐴𝑇𝑇1 |     |     |
| --- | ----------- | --- | --- |

| Comisión Nacional de Energía  |     |     |  19 de 22  |
| ----------------------------- | --- | --- | ---------- |

| —–——–  |     |     |     |     |     | Título 3 Procedimiento para realizar el Estudio  |     |     |     |
| ------ | --- | --- | --- | --- | --- | ------------------------------------------------ | --- | --- | --- |
Tabla 3: contingencias simuladas en cada AdT, destacando los casos en que no se cumplieron los
requerimientos (ejemplo ilustrativo)
|     |            | Año       |        |        |        |        |        |        |        |
| --- | ---------- | --------- | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
|     | Escenario  |           |        |        |        |        |        |        |        |
|     |            |           |        | 𝑻𝑻𝟏𝟏   |        | 𝑻𝑻𝟑𝟑   |        | 𝑻𝑻𝟓𝟓   |        |
|     |            |           | *      | *      | *      | **     | *      | *      | **     |
|     |            |           | 𝐸𝐸1𝑇𝑇1 | 𝐸𝐸2𝑇𝑇1 | 𝐸𝐸1𝑇𝑇3 | 𝐸𝐸2𝑇𝑇3 | 𝐸𝐸1𝑇𝑇5 | 𝐸𝐸2𝑇𝑇5 | 𝐸𝐸3𝑇𝑇5 |
|     |            | 𝐴𝐴𝐴𝐴𝑇𝑇1   | *      | *      | *      | *      | *      | **     | *      |
|     |            |           | *      | *      | *      | *      |        |        |        |
𝐴𝐴𝐴𝐴𝑇𝑇2
|     |     |     | *   | *   | *   | *   |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
𝐴𝐴𝐴𝐴𝑇𝑇3
|     |     |     |     |     | *   | *   |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
𝐴𝐴𝐴𝐴𝑇𝑇4
Total de contingencias de
𝐴𝐴𝐴𝐴𝑇𝑇5
|     |     |     | 4   | 4   | 5   | 6   | 2   | 3   | 3   |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
Severidad 4a * por escenario
La Figura 6 a continuación muestra el resultado de las AdT débiles para el ejemplo considerado. De
la Figura 6 se observa que, para el primer año en estudio ( ), se identifican dos AdT débiles,
mientras que para los años   y   se identifica una única AdT débil en cada caso. Este resultado se
𝑇𝑇1
explica por el criterio de clasificación establecido en el Artículo 3-13 del presente Anexo Técnico,
|     |     | 𝑇𝑇3 𝑇𝑇5 |     |     |     |     |     |     |     |
| --- | --- | ------- | --- | --- | --- | --- | --- | --- | --- |
conforme el cual, para un año  , una determinada AdT se deberá catalogar como débil cuando, para
al menos una contingencia, no se cumpla alguno de los requerimientos señalados en el (Paso 3), aun
𝑇𝑇
cuando dicho incumplimiento se verifique en un único escenario   de dicho año. Por esta razón,
para el año  , las áreas de tensión   y   son catalogadas como débiles, aun cuando los
𝐸𝐸
incumplimientos se verificaron únicamente en el escenario   (ver Tabla 3).
|     | 𝑇𝑇1 |     | 𝐴𝐴𝐴𝐴𝑇𝑇1 | 𝐴𝐴𝐴𝐴𝑇𝑇2 |     |     |     |     |     |
| --- | --- | --- | ------- | ------- | --- | --- | --- | --- | --- |
𝐸𝐸1𝑇𝑇1

Figura 6: resultado de las AdT débiles (ejemplo ilustrativo)
| Artículo 3-15  | Análisis de la Robustez de Frecuencia  |     |     |     |     |     |     |     |     |
| -------------- | -------------------------------------- | --- | --- | --- | --- | --- | --- | --- | --- |
El análisis de Robustez de Frecuencia se desarrolla de manera análoga al análisis de Fortaleza
descrito en el Artículo 3-13 del presente Anexo Técnico, salvo por las siguientes diferencias:
a)  En lugar de considerar las AdT, se utilizan las AdF;
b)  En  las  simulaciones,  en  lugar  de  considerar  fallas  de  Severidad  4a,  se  consideran
contingencias de Severidad 5;
| Comisión Nacional de Energía  |     |     |     |     |     |     |     |     |  20 de 22  |
| ----------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | ---------- |

—–——– Título 3 Procedimiento para realizar el Estudio
c) Respecto de los indicadores de desempeño dinámico, definidos en el Artículo 3-9 del
presente Anexo Técnico, se emplean la frecuencia mínima y RoCoF, calculados conforme a
lo establecido en el Artículo 3-11 del presente Anexo Técnico; y,
d) Respecto de los requerimientos establecidos en el (Paso 3), para cada una de las
contingencias simuladas, se deberán cumplir todos los estándares aplicables establecidos
en la NTSyCS. Sin perjuicio de lo anterior, se deberá verificar, al menos, que:
i. Se cumpla con lo dispuesto en el Artículo 5-31 de la NTSyCS respecto de la estabilidad
del SI frente a la ocurrencia de una contingencia simple de hasta severidad 7, sin admitir
la utilización de Recursos Generales o Adicionales de Control de Contingencias que
impliquen desprendimientos de carga por frecuencia o por tensión.
ii. Que los valores de frecuencia mínima y de RoCoF alcanzados por el sistema, medidos en
la barra eléctricamente más cercana al punto de ocurrencia de la perturbación y
calculados conforme al Artículo 3-11 del presente Anexo Técnico, no provoquen la
activación de Recursos Generales o Adicionales de Control de Contingencias que
impliquen desprendimientos de carga por frecuencia o por tensión.
Comisión Nacional de Energía 21 de 22

—–——– Título 4 Disposiciones transitorias
Título 4 Disposiciones transitorias
Artículo 4-1 Publicación del primer Estudio
El Coordinador deberá publicar el primer Estudio en un plazo no superior a 12 meses contados desde
la publicación en el Diario Oficial de la resolución exenta que aprueba el presente Anexo Técnico.
Artículo 4-2 Publicación del primer listado de indicadores SCL y K
El Coordinador deberá publicar, en un plazo no superior a 15 días hábiles contados desde la
publicación en el Diario Oficial de la resolución exenta que aprueba el presente Anexo Técnico, un
listado con los valores de los niveles de cortocircuito (SCL, del inglés “Short Circuit Level”) mínimos
esperados y factores agregados de interacción IBR ( definido en el Artículo 4-8 del Anexo Técnico
de Exigencias Mínimas de Instalaciones Basadas en Convertidores que se conecten al Sistema
𝐾𝐾
Eléctrico Nacional). La vigencia del referido listado se extenderá desde la fecha de su publicación en
el sitio web del Coordinador hasta la publicación del primer Estudio a la cual se refiere el Artículo 4-
1 del presente Anexo Técnico.
Para efectos de lo anterior, el Coordinador podrá utilizar escenarios simplificados con el fin de
evaluar un conjunto acotado de configuraciones de despacho que sean creíbles, pero exigentes
desde el punto de vista de la Robustez de Frecuencia y de Tensión. En estos escenarios se deberá
calcular el nivel mínimo esperado de SCL y su respectivo resultado de en, al menos, las barras del
SI con niveles de tensión iguales o superiores a 66 kV. Estos indicadores deberán ser calculados
𝐾𝐾
considerando el período anual 2026.
Comisión Nacional de Energía 22 de 22