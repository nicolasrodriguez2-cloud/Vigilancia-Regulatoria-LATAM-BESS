NORMA TÉCNICA DE SEGURIDAD Y
CALIDAD DEL SERVICIO

ANEXO TÉCNICO DE EXIGENCIAS MÍNIMAS DE INSTALACIONES
BASADAS EN CONVERTIDORES QUE SE CONECTEN AL SISTEMA
ELÉCTRICO NACIONAL

Enero de 2026

Santiago, Chile

—–——–

ÍNDICE

Título 1

Aspectos generales .......................................................................................... 3
Objetivo................................................................................................................. 3

Artículo 1-1

Artículo 1-2

Alcance .................................................................................................................. 3

Artículo 1-3

Abreviaturas .......................................................................................................... 3

Artículo 1-4

Deﬁniciones .......................................................................................................... 4

Título 2

Artículo 2-1

Artículo 2-2

Título 3

Artículo 3-1

Obligaciones y funciones .................................................................................. 6
Obligaciones y funciones del Coordinador ........................................................... 6

Obligaciones de los Coordinados .......................................................................... 6
Exigencias mínimas para IBR GFM .................................................................... 7
Exigencias generales para IBR GFM ...................................................................... 7

Artículo 3-2

Controlador de Tensión ......................................................................................... 8

Artículo 3-3

Requerimientos al Controlador de Tensión en operación normal ........................ 9

Artículo 3-4

Requerimientos del Controlador de Tensión en operación ante fallas ............... 10

Artículo 3-5

Control de inyección rápida de corriente ........................................................... 10

Artículo 3-6

Controlador Frecuencia/Potencia ....................................................................... 11

Artículo 3-7

Respuesta inercial ............................................................................................... 12

Artículo 3-8

Control activo de salto de fase ............................................................................ 12

Artículo 3-9

Control de amortiguamiento de potencia .......................................................... 12

Artículo 3-10

Capacidad de operar en una Isla Eléctrica .......................................................... 13

Artículo 3-11

Capacidad de Partida Autónoma ........................................................................ 13

Artículo 3-12

Exigencias a la interconexión de los Sistemas de Almacenamiento de Energía . 14

Título 4

Exigencias mínimas para IBR GFL ..................................................................... 15
Exigencias Generales para IBR GFL ..................................................................... 15

Artículo 4-1

Artículo 4-2

Controlador de Tensión ....................................................................................... 16

Artículo 4-3

Requerimientos al Controlador de Tensión en operación normal ...................... 16

Artículo 4-4

Requerimientos del Controlador de Tensión en operación ante fallas ............... 17

Artículo 4-5

Operación de la IBR GFL ante fallas .................................................................... 18

Artículo 4-6

Cambio de prioridad de inyección de corriente ante fallas ................................ 18

Artículo 4-7

Controlador de Frecuencia/Potencia .................................................................. 19

Artículo 4-8

Requisitos para la interconexión al SI ................................................................. 19

Título 5

Modelos y pruebas ......................................................................................... 21
Requisitos generales para modelos EMT ............................................................ 21

Artículo 5-1

Artículo 5-2

Requisitos especíﬁcos de modelos EMT ............................................................. 21

Comisión Nacional de Energía

 1 de 30

—–——–

Artículo 5-3

Parámetros técnicos de modelos EMT de las IBR GFM ...................................... 23

Artículo 5-4

Informes de validación de modelos EMT ............................................................ 24

Artículo 5-5

Desempeño de la IBR GFM ................................................................................. 24

Artículo 5-6

Desempeño de la IBR GFL ................................................................................... 24

Artículo 5-7

Título 6

Artículo 6-1

Validación del desempeño de los modelos EMT ................................................ 24
Monitoreo y actualización de parámetros ........................................................ 26
Señales adicionales de monitoreo ...................................................................... 26

Artículo 6-2

Actualización de parámetros de control ............................................................. 26

Título 7

Disposiciones Transitorias ............................................................................... 27
Entrada en vigencia del Anexo ............................................................................ 27

Artículo 7-1

Artículo 7-2

Exención de aplicación del Título 3 del Anexo .................................................... 27

Artículo 7-3

Aplicación de requisitos para la interconexión de IBR GFL ................................. 27

Artículo 7-4

Entrega de modelos EMT de las instalaciones interconectadas al SI .................. 28

Artículo 7-5

Exigencias para las IBR GFL existentes ................................................................ 28

Artículo 7-6

Requisitos de Información adicional para una IBR GFM ..................................... 29

Comisión Nacional de Energía

 2 de 30

—–——–

Título 1 Aspectos generales

Título 1  Aspectos generales

Artículo 1-1

Objetivo

El Anexo Técnico tiene por objeto establecer las exigencias técnicas mínimas complementarias a las
establecidas en la Norma Técnica de Seguridad y Calidad de Servicio, para las Instalaciones Basadas
en Convertidores, a efecto de que éstas garanticen el cumplimiento de los objetivos de seguridad y
calidad de servicio.

Artículo 1-2

Alcance

Las disposiciones establecidas en el Anexo Técnico serán aplicables a las Instalaciones Basadas en
Convertidores  que  se  encuentran  interconectadas  o  que  se  vayan  a  interconectar  al  Sistema  de
Transmisión del Sistema Eléctrico Nacional.

Artículo 1-3

Abreviaturas

Adicionalmente de las abreviaturas establecidas en el Título 1-2 de la Norma Técnica de Seguridad y
Calidad de Servicio, para ﬁnes de este Anexo Técnico se establecen las siguientes:

1.

AT IBR, Anexo o Anexo Técnico

2.

FIV

3.  HIL

4.

IBR GFL

5.

IBR GFM

6.

EMT

7.  NTSyCS

8.  OEM

9.

PLL

: Anexo Técnico de Exigencias Mínimas de Instalaciones
Basadas en Convertidores que se conecten al Sistema
Eléctrico Nacional de la NTSyCS.

: Fuente Interna de Voltaje.

: hardware en el bucle, del Inglés Hardware In the loop.

: Instalación Basada en Convertidores que opera como
un Convertidor Seguidor de Red.

: Instalación Basada en Convertidores que opera como
un Convertidor Formador de Red.

transitorios

:
Electromagnetic Transient.

electromagnéticos,

del

inglés

: Norma Técnica de Seguridad y Calidad de Servicio.

: del fabricante original, del inglés Original Equipment
Manufacturer.

: lazo de sincronización de fase, del inglés Phase Locked
Loop.

Comisión Nacional de Energía

 3 de 30

—–——–

Título 1 Aspectos generales

Artículo 1-4

Deﬁniciones

Adicionalmente a las deﬁniciones establecidas en el Título 1-2 de la Norma Técnica de Seguridad y
Calidad de Servicio, para ﬁnes de este Anexo Técnico se establecen las siguientes:

1.  Banda  de  Establecimiento:  rango  dentro  del  cual  la  señal  de  salida  del  Controlador  de
Frecuencia/Potencia  o  Controlador  de  Tensión  de  una  IBR  debe  estabilizarse  y  permanecer
dentro de este, luego de una desviación en la señal de entrada.

2.  Banda de Operación Normal: intervalo de tensiones o frecuencias dentro del cual el Controlador
de Tensión o Controlador de Frecuencia/Potencia de una IBR puede operar de forma continua,
en cualquiera de sus modos de operación, sin activar los sistemas de protección.

3.  Convertidor(es) Formador(es) de Red: equipo que utiliza electrónica de potencia, cuyo modo
de operación le permite establecer y controlar el fasor de tensión en el Punto de Conexión al SI.
Es capaz de operar de manera independiente, incluso en ausencia de otras fuentes de tensión.
Su funcionamiento le permite actuar como una fuente de tensión, controlando su propio fasor
de tensión interno.

4.  Convertidor(es) Seguidor(es) de Red: equipo que utiliza electrónica de potencia, cuyo modo de
operación  se  basa en  un PLL, siguiendo  el fasor  de  tensión y  la  frecuencia establecidas en el
Punto de Conexión al SI.

5.  Amortiguamiento de Oscilaciones Subsíncronas: corresponde a la capacidad de una IBR para

atenuar las oscilaciones que se presentan a frecuencias inferiores a la nominal del SI.

6.  Cambio(s) de Ángulo de Fase: corresponde a la diferencia entre el ángulo de fase de la tensión
medida en el Punto de Conexión al SI en un semiciclo del sistema eléctrico, respecto del ángulo
de fase medido en el semiciclo anterior.

7.

8.

Inercia Sintética: capacidad de un Convertidor Formador de Red de entregar o reducir potencia
activa, de manera instantánea, en respuesta a una perturbación en el SI. Dicha respuesta inicial
es automática y no requiere mediciones de frecuencia en el Punto de Conexión al SI.

Inestabilidad  del  PLL:  fenómeno  dinámico  que  afecta  a  las  IBR  GFL,  caracterizado  por  la
incapacidad del PLL del convertidor para seguir correctamente el ángulo de fase de la tensión
en el Punto de Conexión al SI.

9.  Factor Equivalente de Amortiguamiento (z): parámetro que mide la capacidad de la instalación
para  amortiguar  oscilaciones  y  estabilizar  el  sistema  eléctrico  ante  perturbaciones.  Dicho
parámetro  representa  el  nivel  de  amortiguamiento  activo  que  el  convertidor  puede
proporcionar para evitar ﬂuctuaciones excesivas en la frecuencia y el fasor de tensión del SI.

10. Fuente  Interna  de  Voltaje:  es  la  componente  fundamental  de  la  forma  de  onda  de  tensión
generada  a  través  de  dispositivos  electrónicos  de  potencia.  Esta  fuente  opera  de  manera
sincronizada con el SI bajo condiciones normales de operación.

Comisión Nacional de Energía

 4 de 30

—–——–

Título 1 Aspectos generales

11. Potencia por Salto de Fase: potencia activa o reactiva inyectada o absorbida por un Convertidor
Formador de Red en respuesta a Cambios de Ángulo de Fase entre su FIV y el Punto de Conexión
al SI.

12. Potencia de Amortiguamiento: respuesta controlada de la potencia activa o reactiva de una IBR,
ante  oscilaciones  de  la  tensión  o  frecuencia  en  el  Punto  de  Conexión  al  SI.  En Convertidores
Formadores de Red, se logra mediante una respuesta natural del control, en cambio, para los
Convertidores Seguidores de Red, se obtiene mediante controles activos externos.

13. Tiempo de Establecimiento: intervalo de tiempo que transcurre desde que el Controlador de
Frecuencia/Potencia o Controlador de Tensión detecta una desviación en la señal de entrada,
hasta  que  la  señal  de  salida  correspondiente  ingresa  y  permanece  dentro  de  la  Banda  de
Establecimiento.

14. Tiempo de Reacción: intervalo de tiempo que transcurre entre la ocurrencia de un cambio en la
señal de entrada y el instante en que el Controlador de Frecuencia/Potencia o Controlador de
Tensión inicia su respuesta mediante un cambio en la señal de salida correspondiente.

15. Tiempo  de  Crecimiento:

requerido  por  el  Controlador  de
Frecuencia/Potencia o Controlador de Tensión, para que, ante un cambio en la señal de entrada,
la señal de salida correspondiente aumente del 10% al 90% de su valor ﬁnal.

intervalo  de  tiempo

Comisión Nacional de Energía

 5 de 30

—–——–

Título 2 Obligaciones y funciones

Título 2  Obligaciones y funciones

Artículo 2-1

Obligaciones y funciones del Coordinador

Con el objeto de dar cumplimiento a lo establecido en el Anexo, el Coordinador deberá:

a)  Exigir el cumplimiento de las disposiciones del Anexo por parte de los Coordinados, requiriendo
para  esto  los  estudios,  modelos, ensayos, planos y  antecedentes  que  sean  necesarios, en  las
instancias correspondientes establecidas en la normativa vigente.

b)  Publicar y mantener actualizada la información señalada en el literal precedente. Sin perjuicio
de ello, deberá adoptar las medidas necesarias para resguardar la conﬁdencialidad y reserva de
aquella información que tenga carácter económica o comercialmente sensible.

c)

Informar a la Superintendencia aquellos incumplimientos de las disposiciones del Anexo.

d)  Dar cumplimiento a las exigencias del Anexo y la NTSyCS, en las materias que corresponda.

e)  Solicitar antecedentes adicionales o realizar auditorías, con el ﬁn de resguardar la veracidad de
la  información  presentada  por  los  Coordinados,  y  veriﬁcar  el  cumplimiento  de  las  exigencias
establecidas en el Anexo.

Artículo 2-2

Obligaciones de los Coordinados

Con el objeto de dar cumplimiento a lo establecido en el Anexo, los Coordinados deberán:

a)  Dar cumplimiento a las exigencias establecidas en el Anexo y en la NTSyCS, según corresponda.

b)  Entregar  la  información técnica  necesaria  para el  correcto cumplimiento  de  las funciones  del

Coordinador, en el ámbito del Anexo.

c)  Actualizar en forma continua toda la información que el Coordinador requiera para cumplir sus

funciones.

d)  Ajustar los parámetros técnicos a requerimientos del Coordinador, cuando corresponda.

e)  Cumplir con las demás disposiciones que expresamente se determinan en el Anexo.

Comisión Nacional de Energía

 6 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

Título 3  Exigencias mínimas para IBR GFM

Artículo 3-1

Exigencias generales para IBR GFM

Las IBR GFM deberán cumplir con, al menos, las siguientes exigencias:

a)  Regular la tensión y frecuencia de forma autónoma en el Punto de Conexión al SI, resguardando

los límites técnicos de la instalación.

b)  Mantener  su  FIV  predominantemente  constante  en  el  Régimen  Transitorio.  Dicha  FIV  debe
controlarse para mantener el sincronismo con otras instalaciones del SI y también debe regular
la potencia activa y reactiva para dar soporte a la red.

c)  Por  diseño,  la energía  debe  estar  disponible  de  forma  instantánea  para  el  SI,  sin  que  se vea
retrasada por algoritmos de control en el lado de corriente continua. Se considera un tiempo
de respuesta instantánea aquella con un Tiempo de Reacción menor a 10 milisegundos y un
Tiempo de Establecimiento menor a 20 milisegundos.

d)  Por diseño, deberá poseer una capacidad de sobrecorriente de, al menos, 1,3 por unidad de la
corriente  nominal  de  la  instalación  por  5  segundos,  sin  comprometer  la  integridad  de  la
instalación.

e)  Responder  ante  variaciones  en  los  parámetros  o  eventos  del  SI  de  manera  equivalente  en
magnitud  y  tiempo  de  respuesta,  conforme  a  los  parámetros  establecidos  en  el  Anexo.
Excepcionalmente, podrá entregar una respuesta no equivalente en los siguientes casos:

i.

ii.

Para proteger la instalación, evitando daños en su operación; y,

Cuando la energía disponible para inyección o absorción no sean iguales.

f)  Operar de manera estable conectada a una Red Débil.

g)  Proporcionar corrientes de cortocircuito dentro de los rangos de operación de diseño, conforme

al Artículo 3-5 del Anexo.

h)  Proporcionar respuesta inercial conforme al Artículo 3-7 del Anexo.

i)  Gestionar  fallas  y  perturbaciones,  en  el  sentido  de  brindar  soporte  al  SI  durante  caídas  de
tensión u otras condiciones transitorias sin desconectarse, resguardando los límites técnicos de
la instalación.

En  caso  de  sobretensiones  mayores  a  1,1  y  menores  o  iguales  a  1,2  por  unidad, la  IBR  GFM
deberá operar de manera continua e ininterrumpida durante al menos 1 segundo.

En cuanto a las caídas de tensión, la IBR GFM deberán permanecer conectadas al SI. Para ello, la
tensión fase-tierra en el Punto de Conexión al SI de las fases falladas deberá variar dentro de la
zona achurada de la Figura 1 (zona de no-desconexión), siempre que las tensiones en las fases

Comisión Nacional de Energía

 7 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

no  falladas  no  sobrepasen  las  tensiones  máximas  de  servicio.  Para  estos  efectos,  la  tensión
deberá medirse en el lado de mayor tensión del Punto de Conexión al SI.

Figura 1: zona de no desconexión para una IBR GFM

Siendo:

 = 0 milisegundos, tiempo de inicio de la falla.

  =  tiempo  máximo  de  despeje  de  falla  establecido  en  el  Artículo  5-40  de  la  NTSyCS,

𝑇𝑇0
según el nivel de tensión del Punto de Conexión al SI.
𝑇𝑇1

 =

+20 milisegundos.

𝑇𝑇2

 = 1000 milisegundos.

𝑇𝑇1

j)  Proporcionar amortiguamiento a las oscilaciones indeseadas de potencia en el SI, de acuerdo

𝑇𝑇3

con el Artículo 3-9 del Anexo.

k)  Ante contingencias que provoquen la formación de Islas Eléctricas, la IBR GFM deberá operar
de  manera  independiente,  es  decir,  sin  requerir  apoyo  de  otras  unidades  generadoras
sincrónicas u otras IBR GFM. Lo anterior, considerando la disponibilidad del recurso energético.

l)  Proporcionar  corriente  de  secuencia  negativa,  resguardando  los  límites  técnicos  de  la

instalación.

Artículo 3-2

Controlador de Tensión

Las  IBR  GFM  que  operen  conectadas  al  SI  deberán  disponer  de  un  Controlador  de  Tensión  que
distinga entre condiciones de operación normal y condiciones de operación ante fallas.

Comisión Nacional de Energía

 8 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

La instalación deberá activar su operación ante fallas cuando se produzca un descenso de tensión en
el Punto de Conexión al SI, que supere el umbral de tensión de operación normal, de acuerdo con el
literal l) del Artículo 3-3 del Anexo.

Artículo 3-3

Requerimientos al Controlador de Tensión en operación normal

En  estado  de  operación  normal,  el  Controlador  de  Tensión  deberá  cumplir  con,  al  menos,  los
siguientes requerimientos:

a)  Ser  autónomo,  permitiéndole  mantener

límites  permitidos
correspondientes en el Punto de Conexión al SI, de acuerdo con lo establecido en la NTSyCS, sin
requerir el apoyo de otras unidades generadoras sincrónicas u otras IBR GFM.

la  tensión  dentro  de

los

b)  Estar  diseñado  para  operar  en  cualquiera  de  los  siguientes  modos  de  control,  los  cuales  son

excluyentes entre sí:

i.

ii.

Regulación de tensión o regulación de tensión con Estatismo Permanente;

Regulación del factor de potencia a consigna; y,

iii.

Regulación de potencia reactiva en base a un valor de consigna.

c)  Permitir la conmutación entre los modos de control señalados en la letra b).

d)  El Tiempo de Reacción deberá ser inferior a 200 milisegundos, medido en el Punto de Conexión

al SI.

e)  El Tiempo de Crecimiento deberá ser inferior a 1 segundo, medido en el Punto de Conexión al

SI. El Coordinador, justiﬁcadamente, podrá instruir un tiempo mayor.

f)  El Tiempo de Establecimiento deberá ser menor a 5 segundos, medido en el Punto de Conexión

al SI.

g)  La Banda de Establecimiento deberá ser inferior a ±5%, medido en el Punto de Conexión al SI.

h)  El porcentaje de la sobreoscilación no deberá exceder un 5%, manteniéndose así dentro de la
Banda de Establecimiento. Este porcentaje corresponde a la diferencia entre el valor máximo de
salida y el valor ﬁnal estabilizado, dividida por el cambio real en la salida (desde el valor inicial
hasta el ﬁnal estabilizado).

i)  El Estatismo Permanente será ajustable dentro del rango del 2% al 10%.

j)  Cuando la instalación opere en modo de regulación del factor de potencia, deberá ser capaz de
mantener  dicho  factor  dentro  de  un  margen  de  ±5%  de  la  potencia  aparente  nominal  de  la
instalación.

k)  Cuando la instalación opere en el modo de control de regulación de potencia reactiva, deberá
mantener el valor de consigna dentro de un margen de ±5% de la potencia aparente nominal de
la instalación.

Comisión Nacional de Energía

 9 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

l)

Incorporar un umbral de tensión conﬁgurable para la activación de la operación ante fallas, cuyo

valor por defecto será de ±10% de

. Cuando la tensión en el Punto de Conexión al SI exceda

dichos límites, el sistema de control de tensión en operación normal no deberá intervenir con la
actuación del control de inyección rápida de corriente, conforme a lo establecido en el Artículo
3-5 del Anexo.

Δ𝑈𝑈
𝑈𝑈𝑛𝑛𝑛𝑛𝑛𝑛

m)  El  funcionamiento  del  Controlador  de  Tensión  de  la  instalación  estará  limitado  por  la

disponibilidad del recurso energético.

Considerando los requisitos anteriores, el Coordinador determinará el ajuste especíﬁco que deberán
implementar las IBR GFM conforme a sus limitaciones técnicas, en atención a la seguridad y calidad
de servicio, y de conformidad con lo establecido en el Artículo 3-5 de la NTSyCS.

Artículo 3-4

Requerimientos del Controlador de Tensión en operación ante fallas

En condiciones de operación ante fallas, el Controlador de Tensión deberá cumplir con, al menos,
los siguientes requerimientos:

a)  La inyección de corriente deberá cumplir con las exigencias establecidas en el Artículo 3-5 del

Anexo.

b)  La  FIV  del  convertidor  deberá  mantenerse  predominantemente  constante  en  el  Régimen

Transitorio, sin exceder los límites técnicos de la instalación.

c)  Luego  del  despeje  de  la  falla,  el  Controlador  de  Tensión  deberá  minimizar  el  riesgo  de

sobretensiones transitorias.

d)  Una vez que la tensión medida en el Punto de Conexión al SI regrese a los límites de la Banda de
Operación Normal del Controlador de Tensión, el sistema de control de la instalación deberá
operar  según  las  disposiciones  del  artículo  precedente.  Asimismo,  la  instalación  deberá
recuperar el aporte de potencia activa previo a la caída de tensión en un tiempo inferior a 1
segundo.

Artículo 3-5

Control de inyección rápida de corriente

En  condiciones  de  operación  ante  fallas,  las  IBR  GFM  inyectarán  corrientes  de  cortocircuito
considerando lo siguiente:

a)  Deberá poseer una respuesta instantánea, de modo que la energía inyectada contribuya a la
recuperación  de  la  tensión  del  SI.  La  corriente  inyectada  deberá  oponerse  a  la  variación  de
tensión  medida  en  los  terminales  del  convertidor.  Para  estos  efectos,  se  considera  como
respuesta instantánea aquella que posee un Tiempo de Reacción inferior a 10 milisegundos y
un Tiempo de Establecimiento inferior a 20 milisegundos.

b)  Sin  excepción,  toda  IBR  GFM  deberá  inyectar  una  corriente  reactiva  superior  a  la  que
suministraba  previo  a  la  contingencia.  Asimismo,  durante  la  inyección  rápida  de  corriente

Comisión Nacional de Energía

 10 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

reactiva,  la  corriente  activa  deberá  mantenerse  en  su  mayor  valor  posible,  siempre  que  no
exceda los estándares de seguridad de la instalación.

c)  Ante  fallas  asimétricas,  la  IBR  GFM  deberá  inyectar  corrientes  asimétricas,  incluyendo
componentes  de  secuencia  negativa,  con  el  ﬁn  de propender  a  mantener  una  tensión
balanceada en el Punto de Conexión al SI.

d)  La  inyección  de  corriente  deberá  continuar  operando  mientras  se  encuentre  en  Régimen

Transitorio.

e)  La  instalación  deberá  contar  con  un  margen  de  sobrecorriente  reactiva  considerando  la

capacidad señalada en el literal d) del Artículo 3-1 del Anexo.

f)  Las  exigencias  anteriores  deberán  considerar,  en  todo  momento,  los  límites  técnicos  de  la

instalación.

Artículo 3-6

Controlador Frecuencia/Potencia

El Controlador de Frecuencia/Potencia de una IBR GFM deberá ser autónomo, permitiéndole operar
dentro  de  los  márgenes  de  frecuencia  establecidos  en  la  NTSyCS  sin  requerir  el  apoyo  de  otras
máquinas sincrónicas u otras IBR GFM. Asimismo, deberá ser capaz de responder a variaciones de la
frecuencia del SEN, medidas en el Punto de Conexión al SI.

El Controlador de Frecuencia/Potencia deberá cumplir con, al menos, los siguientes requisitos:

a)  El Tiempo de Reacción deberá ser inferior a 1 segundo, medido en el Punto de Conexión al SI.

b)  El Tiempo de Crecimiento deberá ser inferior a 4 segundos, medido en el Punto de Conexión al

SI.

c)  El  Tiempo  de  Establecimiento  deberá  ser  inferior  a  10  segundos,  medido  en  el  Punto  de

Conexión al SI.

d)  La Banda de Establecimiento deberá ser inferior a ±5%, medido en el Punto de Conexión al SI.

e)  El Estatismo Permanente del controlador deberá ser ajustable dentro del rango del 2% al 5%.

f)  La banda muerta deberá ser menor o igual a ±30 [mHz].

g)  El  Controlador  de  Frecuencia/Potencia  no  deberá  intervenir  con  la  respuesta  inercial  de  la

instalación a que se reﬁere el Artículo 3-7 del Anexo.

h)  El  funcionamiento  del  controlador  podrá  estar  limitado  por  la  disponibilidad  del  recurso

energético.

Considerando los requisitos anteriores, el Coordinador determinará el ajuste especíﬁco que deberán
implementar las IBR GFM conforme a sus limitaciones técnicas, en atención a la seguridad y calidad
de servicio, y de conformidad con lo establecido en el Artículo 3-5 de la NTSyCS.

Comisión Nacional de Energía

 11 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

Artículo 3-7

Respuesta inercial

Las IBR GFM deberán proporcionar Inercia Sintética considerando lo siguiente:

a)  En  Régimen  Transitorio  deberá  poseer  una  respuesta  instantánea,  de  modo  que  la  energía
inyectada contribuya a reducir la magnitud del RoCoF del SI, considerando la capacidad técnica
de  la  instalación.  Para  estos  efectos,  se  considera  como  respuesta  instantánea  aquella  que
posee  un  Tiempo  de  Reacción  inferior  a  10  milisegundos  y  un  Tiempo  de  Establecimiento
inferior a 20 milisegundos.

b)  Posterior al Régimen Transitorio, el controlador deberá responder a los ajustes de frecuencia
del Controlador de Frecuencia/Potencia de acuerdo con lo señalado en el artículo precedente.

c)  La instalación deberá contar con un margen de sobrecorriente activa considerando la capacidad

señalada en el literal d) del Artículo 3-1 del Anexo.

Artículo 3-8

Control activo de salto de fase

Las IBR GFM deberán estar conﬁguradas para aportar Potencia por Salto de Fase. Para tal efecto,
deberá cumplir con las siguientes exigencias:

a)  Su respuesta deberá ser instantánea. Se considera un tiempo de respuesta instantánea aquella
que posee un Tiempo de Reacción inferior a 10 milisegundos y un Tiempo de Establecimiento
inferior a 20 milisegundos

b)  El ángulo máximo de salto de fase deberá permitir una respuesta lineal y controlada, sin activar
las  funciones  de  limitación  de  corriente,  considerando  un  ángulo  de  referencia  cercano  a  0
grados, el cual será el punto de operación normal en Régimen Permanente. El ángulo máximo
de salto de fase no podrá ser inferior a 30 grados.

c)  En  Régimen  Transitorio  la  instalación  deberá  continuar  operando  de  manera  estable  con  las

funciones de limitación de corriente activadas.

A  efectos  de  la  aplicación  del  presente  artículo,  los  Coordinados  deberán  entregar  toda  la
información técnica relativa a las características técnicas del desempeño del control activo de salto
de fase, de acuerdo con lo señalado en el Artículo 7-6 del Anexo.

Artículo 3-9

Control de amortiguamiento de potencia

Las  IBR  GFM  deberán  proveer  Amortiguamiento  de  Oscilaciones  Subsíncronas  a  las  oscilaciones
indeseadas del SEN, resguardando las siguientes características:

a)  Entregar Potencia de Amortiguamiento frente a oscilaciones del SI entre 0,05 [Hz] a 1 [Hz] peak

to peak.

b)  A ﬁn de contribuir positivamente al amortiguamiento de las oscilaciones en la mayoría de las
condiciones de operación, la respuesta de la impedancia de secuencia positiva deberá contar
con un ángulo de fase inductivo o capacitivo.

Comisión Nacional de Energía

 12 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

c)  Las  características  de  amortiguamiento  deberán  ser  ajustables  mediante  software.  Estas
características deberán determinarse y ajustarse en función del comportamiento dinámico del
SI en su Punto de Conexión.

d)  La  conﬁguración  y  parametrización  de  la  instalación  no  deberá  introducir  nuevos  modos

oscilatorios inestables en el SI, ni exacerbar los modos oscilatorios existentes.

e)  El  sistema  de  control  deberá  ser  capaz  de  proporcionar  amortiguamiento  a  las  oscilaciones
subsincrónicas resultantes de las Interacciones de Control, especialmente en una Red Débil.

f)  Evitar  resonancias  a  frecuencias  elevadas  producto  de  capacitancias  en  derivación  o  serie,
cargas  de  línea  o  Interacciones  de  Control.  Se  podrán  justiﬁcar  excepciones  cuando  una
resonancia interna de la IBR coincida con una resonancia del SI, priorizando, en estos casos, la
protección de los equipos de la instalación sobre la provisión de amortiguamiento.

El amortiguamiento proporcionado por la IBR GFM deberá permitir que este opere dentro de sus
capacidades técnicas.

Artículo 3-10

Capacidad de operar en una Isla Eléctrica

La IBR GFM deberá ser capaz de mantener su operación en Isla Eléctrica, cuando corresponda. Para
ello, deberá cumplir con las siguientes exigencias:

a)  Operar de manera estable en Isla Eléctrica, sin requerir el apoyo de otras IBR GFM o unidades

generadoras sincrónicas.

b)  Operar de manera estable junto con otras IBR GFM o GFL, en ausencia de generación sincrónica.

c)  Operar de manera estable ante fallas o perturbaciones, en la medida que estas no activen los
sistemas de protección que desconecten la IBR GFM, y siempre que la Isla Eléctrica cuente con
los  recursos  necesarios  para  una  operación  estable  en  dichas  condiciones,  que  la  IBR  GFM
cuente con suﬁciente energía almacenada o recurso energético para ello.

d)  Continuar  operado  cuando  el  SI  deje  de  contar  con  unidades  generadoras  sincrónicas,  sin
requerir  controles  externos  ni  sistemas  de  comunicación,  siempre  que  el  SI  cuente  con  los
recursos necesarios para una operación estable.

e)  Continuar  operando  de  manera  estable  ante  la  reconexión  de  unidades  de  generación

sincrónica o al integrarse al SI, ya sea en una Red Débil o Fuerte.

Artículo 3-11

Capacidad de Partida Autónoma

La  IBR  GFM  que  cuente  con  capacidad  de  Partida  Autónoma  deberá  cumplir  con  las  siguientes
exigencias, sujeto a la disponibilidad de recurso energético:

a)

Iniciar  su  operación,  estableciendo  una  referencia  de  tensión  y  frecuencia  sin  contar  con
suministro eléctrico externo proveniente del SI.

b)  Alimentar los sistemas auxiliares necesarios para su operación y energizar una parte del SI o Isla

Eléctrica.

Comisión Nacional de Energía

 13 de 30

—–——–

Título 3 Exigencias mínimas para IBR GFM

c)  Suministrar corrientes de entrada adecuadas para la energización de transformadores (inrush

current), el arranque de motores auxiliares de unidades generadoras sincrónicas, entre otros.

d)  Contar con la capacidad de aumentar la tensión de referencia hasta su valor nominal con una
tasa  de  rampa  controlada,  evitando  corrientes  de  entrada  excesivas  que  puedan  afectar  la
energización de transformadores y líneas de transmisión.

e)  Proporcionar una referencia de tierra para permitir una ruta de partida en negro.

f)  Proporcionar una referencia de tensión constante que permita la sincronización y restauración

progresiva del SI.

g)  Participar  en  un  arranque  autónomo  colectivo,  en  aquellos  casos  en  que  la  instalación  está
diseñada para operar en paralelo con otras instalaciones que posean Partida Autónoma.

Artículo 3-12

Exigencias a la interconexión de los Sistemas de Almacenamiento de Energía

Todo Sistema de Almacenamiento de Energía o componente de almacenamiento de una CRCA que
se interconecten al SEN deberá cumplir con ser una IBR GFM.

A partir de los resultados del Estudio de Análisis de Robustez del SEN, el Coordinador podrá instruir
el cambio del modo de operación entre IBR GFM e IBR GFL, según corresponda, estableciendo para
ello  un  plazo  de  implementación.  Dicha  modiﬁcación  se  limitará  exclusivamente  a  ajustes  de
software y adecuaciones en los sistemas de comunicaciones, cuando estas sean necesarias.

Comisión Nacional de Energía

 14 de 30

—–——–

Título 4 Exigencias mínimas para IBR GFL

Título 4  Exigencias mínimas para IBR GFL

Artículo 4-1

Exigencias Generales para IBR GFL

Las IBR GFL deberán cumplir con, al menos, las siguientes exigencias:

a)  Operar sincronizados con el SI, sin provocar interacciones indebidas con otros equipos.

b)  Gestionar  fallas  o  perturbaciones,  brindando  soporte  al  SI  durante  caídas  de  tensión  u  otras

condiciones transitorias sin desconectarse.

En caso de sobretensiones mayores a 1,1 por unidad y menores o iguales a 1,2 por unidad, la
IBR GFL deberá operar de manera continua e ininterrumpida durante al menos 1 segundo.

En cuanto a las caídas de tensión, la IBR GFL deberán permanecer conectadas al SI. Para ello, la
tensión fase-tierra en el Punto de Conexión al SI de las fases falladas deberá variar dentro de la
zona achurada de la Figura 2 (zona de no-desconexión), siempre que las tensiones en las fases
no  falladas  no  sobrepasen  las  tensiones  máximas  de  servicio.  Para  estos  efectos,  la  tensión
deberá medirse en el lado de mayor tensión del Punto de Conexión.

Figura 2: zona de no desconexión para una IBR GFL

Siendo:

 = 0 milisegundos, tiempo de inicio de la falla.

 = tiempo máximo de despeje de falla establecido en el Artículo 5-40 de la NTSyCS, según el

𝑇𝑇0
nivel de tensión del Punto de Conexión al SI.
𝑇𝑇1

 =

+20 milisegundos.

𝑇𝑇2

𝑇𝑇1

Comisión Nacional de Energía

 15 de 30

—–——–

Título 4 Exigencias mínimas para IBR GFL

 = 1000 milisegundos.

c)  Durante la operación ante fallas, el sistema de control de la instalación deberá tener la capacidad
𝑇𝑇3
de  conmutar  entre  operación  con  prioridad  de  corriente  activa  y  operación  con  prioridad  de
corriente  reactiva,  según  corresponda.  Por  defecto,  ante  eventos  que  involucren  caídas  de
tensión que excedan la banda de operación del Controlador de Tensión, la instalación deberá
operar conforme el Artículo 4-5 del Anexo.

d)  Ante Cambios de Ángulo de Fase de hasta 25 grados de la secuencia positiva de la tensión en el
Punto de Conexión al SI, la instalación deberá continuar operando de forma estable conectada
al SEN.

Adicionalmente, la instalación deberá continuar operando de forma estable conectada al SI ante
cualquier  Cambio  de  Ángulo  de  Fase  de  las  fases  individuales  de  la  tensión  en  el  Punto  de
Conexión al SI, esto, siempre que la variación del ángulo de la componente de secuencia positiva
no exceda los 25 grados señalados en el inciso anterior.

Artículo 4-2

Controlador de Tensión

Las IBR GFL que operen conectadas al SI deberán disponer de un Controlador de Tensión que distinga
entre condiciones de operación normal y condiciones de operación ante fallas.

La instalación deberá activar su operación ante fallas cuando se produzca un descenso de tensión en
el Punto de Conexión al SI que supere el umbral de tensión de operación normal, establecido en el
literal k) Artículo 4-3 del Anexo.

Artículo 4-3

Requerimientos al Controlador de Tensión en operación normal

En  estado  de  operación  normal,  el  Controlador  de  Tensión  deberá  cumplir  con,  al  menos,  los
siguientes requerimientos:

a)  Estar  diseñado  para  operar  en  cualquiera  de  los  siguientes  modos  de  control,  los  cuales  son

excluyentes entre sí:

i.

ii.

Regulación de tensión o regulación de tensión con Estatismo Permanente;

Regulación del factor de potencia a consigna; y,

iii.

Regulación de potencia reactiva en base a un valor de consigna.

b)  Permitir la conmutación entre los modos de control señalados en la letra a).

c)  El Tiempo de Reacción deberá ser inferior a 200 milisegundos, medido en el Punto de Conexión

al SI.

d)  El Tiempo de Crecimiento deberá ser inferior a 1 segundo, medido en el Punto de Conexión al

SI. El Coordinador, justiﬁcadamente, podrá instruir un tiempo mayor.

e)  El Tiempo de Establecimiento deberá ser menor a 5 segundos, medido en el Punto de Conexión

al SI.

Comisión Nacional de Energía

 16 de 30

—–——–

Título 4 Exigencias mínimas para IBR GFL

f)  La Banda de Establecimiento deberá ser inferior a ±5%, medida en el Punto de Conexión al SI.

g)  El porcentaje de la sobreoscilación no debe ser mayor a un 5%, manteniéndose así dentro de la
Banda de Establecimiento. Este porcentaje corresponde a la diferencia entre el valor máximo de
salida y el valor ﬁnal estabilizado, dividida por el cambio real en la salida (desde el valor inicial
hasta el ﬁnal estabilizado).

h)  El Estatismo Permanente será ajustable dentro del rango del 2% al 10%.

i)  Cuando la instalación opere en modo de regulación del factor de potencia, deberá ser capaz de
mantener el factor de potencia dentro de un margen de ±5% de la potencia aparente nominal
de la instalación.

j)  Cuando la instalación opere en el modo de control de regulación de potencia reactiva, deberá
mantener el valor de consigna dentro de un margen de ±5% de la potencia aparente nominal de
la instalación.

k)

Incorporar un umbral de tensión conﬁgurable para la activación de la operación ante fallas, cuyo

valor por defecto será de ±10% de

. Cuando la tensión en el Punto de Conexión al SI exceda

dichos límites, el sistema de control de tensión en operación normal no deberá intervenir con la
operación del controlador ante fallas, conforme a lo establecido en el Artículo 4-5 del Anexo.

Δ𝑈𝑈
𝑈𝑈𝑛𝑛𝑛𝑛𝑛𝑛

l)  El  funcionamiento  del  Controlador  de  Tensión  de  la  instalación  estará  limitado  por  la

disponibilidad del recurso energético.

Considerando los requisitos anteriores, el Coordinador determinará el ajuste especíﬁco que deberán
implementar las IBR GFM conforme a sus limitaciones técnicas, en atención a la seguridad y calidad
de servicio, y de conformidad con lo establecido en el Artículo 3-5 de la NTSyCS.

Artículo 4-4

Requerimientos del Controlador de Tensión en operación ante fallas

En condiciones de operación ante fallas, el Controlador de Tensión deberá cumplir con, al menos,
los siguientes requerimientos:

e)  La operación ante fallas deberá activarse automáticamente dentro de un tiempo no superior a
30 milisegundos desde la detección de la condición de baja tensión, hasta el inicio de inyección
de corriente de acuerdo con el Artículo 4-5 del Anexo.

f)  El  Tiempo  de  Establecimiento  deberá  ser  inferior  a  80  milisegundos,  medido  en  el  Punto  de

Conexión al SI.

g)  La Banda de Establecimiento deberá ser inferior a ±10%, medida en el Punto de Conexión al SI.

h)  La inyección de corriente deberá cumplir con las exigencias establecidas en el Artículo 4-5 del

Anexo.

i)  Cuando la tensión medida en el Punto de Conexión al SI regrese dentro de los límites de la Banda
de Operación Normal del Controlador de Tensión, el sistema de control de la instalación deberá
activar la operación en condición normal, de acuerdo con el Artículo 4-3 del Anexo.

Comisión Nacional de Energía

 17 de 30

—–——–

Título 4 Exigencias mínimas para IBR GFL

Considerando los requisitos anteriores, el Coordinador determinará el ajuste especíﬁco que deberán
implementar las IBR GFM conforme a sus limitaciones técnicas, en atención a la seguridad y calidad
de servicio, y de conformidad con lo establecido en el Artículo 3-5 de la NTSyCS.

Artículo 4-5

Operación de la IBR GFL ante fallas

En  condiciones  de  operación  ante  fallas,  la  instalación  deberá  priorizar  la  inyección  de  corriente
reactiva.  En  dicho  modo,  la  instalación  deberá  suministrar  corriente  reactiva  adicional  (∆
)
equivalente al 2% de la corriente nominal (
 en el Punto de Conexión.
𝐼𝐼𝑟𝑟

) por cada 1% de Δ

/

𝑈𝑈

𝑈𝑈𝑛𝑛𝑛𝑛𝑛𝑛

𝐼𝐼𝑛𝑛𝑛𝑛𝑛𝑛

Δ𝐼𝐼𝑟𝑟
𝐼𝐼𝑛𝑛𝑛𝑛𝑛𝑛 = 2

ΔU
𝑈𝑈𝑛𝑛𝑛𝑛𝑛𝑛

Donde se tiene que:

•

•

Δ𝐼𝐼𝑟𝑟

= 𝐼𝐼𝑟𝑟 − 𝐼𝐼𝑟𝑟0
=

ΔU
•  Con

𝑈𝑈 − 𝑈𝑈0
 y

 la corriente reactiva y tensión antes de la falla, respectivamente.

𝑈𝑈0

𝐼𝐼𝑟𝑟0

La IBR GFL que se encuentre en condiciones de operación ante falla, deberá inyectar una corriente
. Esta acción del sistema de control de la
aparente de secuencia positiva de hasta el 100% de la
instalación deberá mantenerse hasta que la tensión, medida en el lado de mayor tensión del Punto
de  Conexión,  retorne  dentro  de  los  límites  deﬁnidos  por  la  Banda  de  Operación  Normal  de  su
Controlador de Tensión.

𝐼𝐼𝑛𝑛𝑛𝑛𝑛𝑛

A partir del instante en que se despeje la falla o ﬁnalice el evento que produjo la caída de tensión en
el Punto de Conexión, y dicha tensión retorne dentro de Banda de Operación Normal del Controlador
de Tensión, la IBR GFL deberá reestablecer su inyección de potencia activa al valor previo al evento,
en el menor tiempo posible. Para ello, deberá encontrarse dentro de la Banda de Establecimiento
de ±10% de la misma en un tiempo no mayor a 1 segundo, considerando la disponibilidad del recurso
energético.  Lo  anterior,  con  la  ﬁnalidad  de  asegurar  que  el  Controlador  de  Frecuencia/Potencia
permanezca operativo y cumpla con los requisitos de desempeño establecidos en el Artículo 4-7 del
Anexo, una vez ﬁnalizada la acción del sistema de control asociado al evento.

Sin perjuicio de lo anterior, el Coordinador podrá disponer un cambio de prioridad de inyección de
corriente ante falla, de acuerdo con lo señalado en el siguiente Artículo 4-6 del Anexo.

Artículo 4-6

Cambio de prioridad de inyección de corriente ante fallas

El Coordinador podrá instruir justiﬁcadamente a una IBR GFL que, en condiciones de operación ante
fallas de acuerdo con lo dispuesto en el Artículo 4-5 del Anexo, priorice la inyección de corriente
activa por sobre la inyección de corriente reactiva o viceversa, de acuerdo con los resultados del
Estudio de Análisis de Robustez del SEN vigente. Dicha prioridad se establecerá mediante un ajuste
de parámetros del controlador y no como una acción durante el trascurso de una falla.

Comisión Nacional de Energía

 18 de 30

—–——–

Título 4 Exigencias mínimas para IBR GFL

El  Coordinador  deberá  comunicar  la  instrucción  de  cambio  de  prioridad  a  los  Coordinados  que
correspondan,  indicando  expresamente  las  instalaciones  involucradas,  la  fecha  de  inicio  de  la
instrucción y las condiciones bajo las cuales se aplicará. El Coordinado deberá ejecutar la instrucción
dentro del plazo que deﬁna el Coordinador, el cual no podrá ser inferior a 30 días corridos.

Artículo 4-7

Controlador de Frecuencia/Potencia

IBR  GFL  que  operen  conectadas  al  SI  deberán  disponer  de  un  Controlador  de

Las
Frecuencia/Potencia, el cual deberá cumplir con, al menos, los siguientes requisitos mínimos:

a)  El Tiempo de Reacción deberá ser inferior a 1 segundo, medido en el Punto de Conexión al SI. El
Coordinador podrá aceptar retardos superiores sólo en caso de que el Coordinado proporcione
evidencias técnicas que lo justiﬁquen.

b)  El Tiempo de Crecimiento deberá ser inferior a 4 segundos, medido en el Punto de Conexión al

SI.

c)  El  Tiempo  de  Establecimiento  deberá  ser  inferior  a  10  segundos,  medido  en  el  Punto  de

Conexión al SI.

d)  La Banda de Establecimiento deberá ser inferior a ±10%, medida en el Punto de Conexión al SI.

e)  El Estatismo Permanente deberá ser ajustable dentro del rango del 2% al 5%.

f)  La banda muerta deberá ser menor o igual a ±30 [mHz].

g)  El funcionamiento del Controlador de Frecuencia/Potencia de las instalaciones estará limitado

por la disponibilidad del recurso energético.

Las IBR GFL deberán contar también con funciones de control que aseguren que la tasa de toma de
carga no supere un valor ajustable entre 0 a 20% de la potencia nominal de la instalación por minuto,
en su arranque y durante su operación normal.

Considerando los requisitos anteriores, el Coordinador determinará el ajuste especíﬁco que deberán
implementar las IBR GFL conforme a sus limitaciones técnicas, en atención a la seguridad y calidad
de servicio, y de conformidad con lo establecido en el Artículo 3-5 de la NTSyCS.

Artículo 4-8

Requisitos para la interconexión al SI

Las IBR GFL deberán veriﬁcar que la relación de cortocircuito (SCR del inglés Short Circuit Ratio) en
la  barra  o  Punto  de  Conexión  al  SI  sea  mayor  o  igual  que  3  (
),  y  que  la  relación  de
cortocircuito  equivalente  (ESCR  del  inglés  Equivalent  Short  Circuit  Ratio)  sea  mayor  o  igual  a  1,5
),  considerando  los  valores  vigentes  para  su  cálculo  a  la  fecha  de  obtención  de  la
(
declaración en construcción.
𝐸𝐸𝑆𝑆𝑆𝑆𝑆𝑆 ≥ 1,5
El SCR de la barra

 o Punto de Conexión al SI, se deberá calcular de acuerdo con:

𝑆𝑆𝑆𝑆𝑆𝑆 ≥ 3

𝑖𝑖

𝑆𝑆𝑆𝑆𝑆𝑆𝑖𝑖 =

𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖
𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺

Comisión Nacional de Energía

 19 de 30

Título 4 Exigencias mínimas para IBR GFL

—–——–

Donde,

:  relación  de  cortocircuito  en  la  barra

potencia aparente de cortocircuito (
𝑆𝑆𝑆𝑆𝑆𝑆𝑖𝑖

𝑖𝑖

  o  Punto  de  Conexión  al  SI.  Este  índice  relaciona  la
).

) y la potencia nominal de la IBR GFL a conectar (

: nivel de cortocircuito en la barra
𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖

 o Punto de Conexión al SI, en MVA, de acuerdo con los

𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺

resultados del Estudio de Análisis de Robustez del SEN vigente.
𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖

𝑖𝑖

: Potencia activa nominal, en MW, de la IBR GFL a conectar en la barra

 o Punto de Conexión

al SI.
𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺
A su vez, el ESCR de la barra

𝑖𝑖

Donde,

 o Punto de Conexión al SI, se deberá calcular de acuerdo con:

𝑖𝑖

𝐸𝐸𝑆𝑆𝑆𝑆𝑆𝑆𝑖𝑖 =

𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖
𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺 + 𝐾𝐾𝑖𝑖

:  relación  de  cortocircuito equivalente de  la  barra

relaciona  la  potencia  aparente  de  cortocircuito  (
𝐸𝐸𝑆𝑆𝑆𝑆𝑆𝑆𝑖𝑖
conectar (

) más el factor agregado de interacción IBR (

𝑖𝑖

).

 o Punto  de  Conexión al SI.  Este índice
)  con  la  potencia  nominal  de  la  IBR  GFL  a

𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖

𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺

: nivel de cortocircuito en la barra

𝐾𝐾𝑖𝑖
resultados del Estudio de Análisis de Robustez del SEN vigente.
𝑆𝑆𝑆𝑆𝐿𝐿𝑖𝑖

𝑖𝑖

 o Punto de Conexión al SI, en MVA, de acuerdo con los

: potencia activa nominal, en MW, de la IBR GFL a conectar en la barra

 o Punto de Conexión

al SI.
𝑃𝑃𝐼𝐼𝐼𝐼𝐼𝐼 𝐺𝐺𝐺𝐺𝐺𝐺

𝑖𝑖

:  es  el  factor  agregado  de  interacción  IBR  en  la  barra

  o  Punto  de  Conexión  al  SI,  en  MW,  de
acuerdo  con  los  resultados  del  Estudio  de  Análisis  de  Robustez  del  SEN  vigente.  Que  se  deberá
𝐾𝐾𝑖𝑖
calcular de acuerdo con:

𝑖𝑖

Donde,

𝑛𝑛

𝐾𝐾𝑖𝑖 = �(𝐼𝐼𝐹𝐹𝑗𝑗𝑖𝑖 × 𝑃𝑃𝑗𝑗)

𝑗𝑗

: factor de interacción entre las barras

 y

:

𝐼𝐼𝐹𝐹𝑗𝑗𝑖𝑖

𝑖𝑖

𝑗𝑗

: es la potencia activa neta despachada de las IBR GFL, de acuerdo con los escenarios del
 es la cantidad de barras

Estudio de Análisis de Robustez del SEN, conectadas en la barra
𝑃𝑃𝑗𝑗
en el SEN, considerando la barra

 y

.

𝑗𝑗

𝑛𝑛

𝐼𝐼𝐹𝐹𝑗𝑗𝑖𝑖 =

Δ𝑈𝑈𝑗𝑗
Δ𝑈𝑈𝑖𝑖

En caso de que la barra o Punto de Conexión al SI no se encuentre en los resultados del Estudio de
Análisis de Robustez del SEN vigente, los valores de
 corresponderán a los de la barra más
cercana considerando la mínima distancia eléctrica.

 y

𝑖𝑖

𝑆𝑆𝑆𝑆𝐿𝐿

𝐾𝐾

Comisión Nacional de Energía

 20 de 30

—–——–

Título 5 Modelos y pruebas

Título 5  Modelos y pruebas

Artículo 5-1

Requisitos generales para modelos EMT

Los  propietarios,  arrendatarios,  usufructuarios  o  quienes  operen,  a  cualquier  título,
las
instalaciones indicadas en el Artículo 1-2 del Anexo, deberán presentar al Coordinador, previo a la
Entrada en Operación, modelos EMT que permitan realizar simulaciones y análisis de transitorios
electromagnéticos, los cuales deberán ser validados por el Coordinador.

En  caso  de  modiﬁcación  relevante  de  la  IBR  que  afecte  su  operación,  deberá  ser  informada  al
Coordinador  e  incorporada  en  los  modelos  EMT,  de  acuerdo  con  el  Anexo  Técnico  “Requisitos
Técnicos Mínimos de Instalaciones que se Interconectan al SI” de la NTSyCS.

Estos modelos EMT deberán cumplir los siguientes requisitos generales:

a)  Deben ser modelos OEM que permitan realizar simulaciones precisas de las respuestas de la
instalación  en  su  conjunto  ante  eventos.  Estos  modelos  deben  reﬂejar  las  características
técnicas propias de su diseño como, por ejemplo, componentes especíﬁcos, conﬁguraciones,
controles, protecciones, entre otros.

b)  Representar  con  precisión  la  IBR,  incluyendo  todos  los  controles  y  protecciones  relevantes,

tanto de software como de hardware.

c)  Permitir  un  análisis  preciso  de  transitorios  electromagnéticos  de  la  interacción  entre  la

instalación y el SI.

d)  El modelo deberá ser compatible y ejecutable en el software de simulación especializado en
análisis de transitorios electromagnéticos en sistemas eléctricos de potencia. Dicho software
deberá ser deﬁnido por el Coordinador justiﬁcadamente, considerando para ello criterios no
arbitrarios.

Adicionalmente, se deberá entregar junto al modelo EMT, los siguientes antecedentes:

e)  Guía de usuario elaborada por el proveedor o fabricante de los equipos. Esta guía debe describir
las  particularidades  de  los  modelos,  funcionalidades,  modos  de  operación,  parámetros  de
entrada, parámetros de salida, entre otros.

f)  Modelo con sus ajustes basados en el ﬁrmware de la planta misma en operación, en formato
DLL  o  código  fuente,  junto  con  los  archivos  de  conﬁguración  necesarios  que  permitan
representar íntegramente la instalación.

g)

Informe de validación del modelo de acuerdo con lo señalado en el Artículo 5-4 del Anexo.

Artículo 5-2

Requisitos especíﬁcos de modelos EMT

Los modelos EMT deberán cumplir con los siguientes requisitos especíﬁcos:

Comisión Nacional de Energía

 21 de 30

—–——–

Título 5 Modelos y pruebas

a)  Representar  con  exactitud  la  respuesta  de  la  IBR  a  eventos  en  el  SI,  tales  como:  fallas,
perturbaciones en la frecuencia del SI, conexión o desconexión de líneas de transmisión, entre
otros, incluyendo el modelo los siguientes elementos:

i.

Controles a nivel de la instalación y los bucles de control internos del convertidor;

ii.  Módulos de medición y ﬁltrado de la señal de entrada, basados en algoritmos y ﬁltros
reales de procesamiento de señales, asegurando que los retardos de comunicación y el
procesamiento de señales estén adecuadamente representados; y,

iii.  Modelación de los interruptores electrónicos de potencia, que podrá realizarse, entre
otros,  mediante  modelos  de  conmutación  detallados  o  modelos  de  representación
mediante  fuente  de  tensión  o  corriente  controladas.  En  caso  de  utilizar  esta
representación, se deberá veriﬁcar que las funciones de control y protección no estén
simpliﬁcadas, asegurando un adecuado análisis de respuesta dinámica.

Los modelos antes mencionados podrán representarse sin dar a conocer su estructura interna,
manteniendo el acceso a las señales de entrada y salida correspondientes.

b)  Incorporar  todas  las  funciones  de  control  y  protección  a  nivel  de  planta  y  convertidor,

incluyendo:

i.

ii.

iii.

Ajustes en los sistemas de protección de la instalación;

Conﬁguración de tolerancia a descensos de tensión, especiﬁcando las condiciones de
activación y desactivación del Controlador de Tensión; y,

Ajustes  de  inyección  y  absorción  de  corriente  activa  y  reactiva  en  condiciones  de
operación ante fallas.

c)

Incorporar  los  sistemas  críticos  que  afectan  la  estabilidad,  respuesta  y  tolerancia  de  la
instalación frente a perturbaciones, tales como:

i.

ii.

iii.

iv.

PLL;

Chopper del enlace de corriente continua;

Protección y control del enlace de corriente continua; y,

Funciones de limitación de corriente del convertidor.

d)  Incluir detalles de componentes mecánicas tales como, características de las turbinas eólicas,
así como detalles de componentes eléctricas como, por ejemplo, los señalados en el Artículo 5-
3 del Anexo.

e)  Proporcionar acceso a los parámetros de entrada disponibles para el usuario ﬁnal, incluyendo:

i.

Selección del modo de operación tales como, control de tensión, control de potencia
reactiva, control de factor de potencia, entre otros;

Comisión Nacional de Energía

 22 de 30

—–——–

ii.

iii.

Título 5 Modelos y pruebas

Ajustes  conﬁgurables  por  el  usuario  tales  como  la  potencia  de  la  planta,  tensión  de
referencia, respuesta rápida de frecuencia, ajuste de rampas y bandas muertas, entre
otros; y,

Opciones  de  controles  conﬁgurables,  tales  como  amortiguamiento,  inyección  de
corriente reactiva o activa en condiciones de operación ante falla, entre otras.

f)  Dar acceso a señales internas necesarias para la interpretación del comportamiento del modelo
y la realización de estudios eléctricos, como señales de disparo de los sistemas de protección y
alarmas.  Las  descripciones  de  las  señales  internas  deberán  estar  contenidas  en  la  guía  de
usuarios señalada en el literal e) del Artículo 5-1 del Anexo.

g)  El proveedor o fabricante del convertidor deberá especiﬁcar si el modelo EMT suministrado es
adecuado  para  estudios  de  impacto  armónico.  En  caso  contrario,  deberá  proporcionar  un
modelo  adecuado  para  dichos  estudios.  Para  estos  efectos,  el  Coordinador  deberá  deﬁnir
explícitamente,  de  forma  previa,  los  requerimientos  que  deberá  cumplir  el  modelo  para  la
evaluación de armónicos.

h)  Permitir  visualizar  los  parámetros  técnicos  señalados  en  Artículo  5-3  del  Anexo,  según

corresponda.

El Coordinador podrá solicitar requisitos adicionales en los modelos, justiﬁcadamente, con el ﬁn de
validar el comportamiento de los controladores exigidos en el Anexo.

Artículo 5-3

Parámetros técnicos de modelos EMT de las IBR GFM

Los  modelos  EMT  de  las  IBR  GFM  deberán  permitir  la  visualización  de,  al  menos,  los  siguientes
parámetros:

a)  Reactancia primaria del Convertidor Formador de Red, es decir la reactancia entre la FIV y los

terminales del referido convertidor.

b)  Reactancia adicional entre el terminal del Convertidor Formador de Red y el Punto de Conexión

al SI.

c)  El  ángulo  entre  la  FIV  y  los  terminales  de  entrada  del  Convertidor  Formador  de  Red  deberá

permitir la visualización en grados.

d)  El ángulo entre la FIV y el Punto de Conexión al SI deberá permitir la visualización de grados.

e)  La  tensión  de  la  FIV  deberá  visualizarse  por  unidad  de  la  tensión  nominal  del  Convertidor

Formador de Red.

f)  El ángulo de la FIV deberá visualizarse por grados.

g)  El ángulo eléctrico entre la corriente y tensión en la entrada del transformador de potencia del

SI deberá visualizarse en grados.

El  Coordinador  podrá  solicitar  la  visualización  de  parámetros  adicionales  en  los  modelos  antes
mencionados, justiﬁcadamente, con el ﬁn de validar el comportamiento de la IBR GFM.

Comisión Nacional de Energía

 23 de 30

—–——–

Título 5 Modelos y pruebas

Artículo 5-4

Informes de validación de modelos EMT

Los modelos EMT deberán ser validados por los fabricantes. Para ello, podrán utilizar alguno de los
siguientes métodos de validación:

a)

Informes de pruebas de fábrica sobre el desempeño del convertidor ante eventos del SI.

b)  Pruebas de validación HIL.

c)  Mediciones de campo del equipo instalado tras una falla en el SI.

d)  Mediante pruebas de laboratorio del equipo.

e)  Mapeo de la versión del ﬁrmware real del convertidor, a nivel de instalación, con la versión del

modelo EMT.

El Coordinador, justiﬁcadamente, podrá deﬁnir otro método o conjunto de pruebas de validación
de los modelos EMT.

Artículo 5-5

Desempeño de la IBR GFM

El  modelo  EMT  deberá  permitir  la  veriﬁcación  del  desempeño  de,  al  menos,  las  siguientes
componentes de una IBR GFM:

a)  Controlador de Tensión.

b)  Controlador de inyección rápida de corriente.

c)  Controlador de Frecuencia/Potencia.

d)  Respuesta inercial.

e)  Control activo de salto de fase.

La veriﬁcación del desempeño deberá evaluarse en el Punto de Conexión al SI, considerando una
Red Débil.

Artículo 5-6

Desempeño de la IBR GFL

El  modelo  EMT  deberá  permitir  la  veriﬁcación  del  desempeño  de,  al  menos,  las  siguientes
componentes de una IBR GFL:

a)  Controlador de Tensión tanto en condiciones de operación normal como ante fallas.

b)  Controlador de Frecuencia/Potencia.

La veriﬁcación del desempeño deberá evaluarse en el Punto de Conexión al SI.

Artículo 5-7

Validación del desempeño de los modelos EMT

El Coordinador previo a la Entrada en Operación de la instalación deberá validar el desempeño de
los  modelos  EMT,  de  acuerdo  con  lo  señalado  en  el Artículo  5-5 y  Artículo  5-6 del  Anexo,  según

Comisión Nacional de Energía

 24 de 30

—–——–

Título 5 Modelos y pruebas

corresponda.  Para  ello,  el  Coordinador  deberá  deﬁnir  un  set  de  pruebas  que  asegure  el
cumplimiento de los requerimientos establecidos en el Anexo.

Adicionalmente, el Coordinador deberá validar los modelos EMT, en los siguientes aspectos en el
caso de las IBR GFM:

a)  La  transición  estable  entre  su  Controlador  de  Tensión  en  operación  normal  y  ante  falla

considerando el inicio de la falla y su despeje.

b)  La transición estable entre el Controlador de Frecuencia/Potencia y la respuesta inercial de la

instalación.

c)  La estabilidad operativa ante saltos de fase de hasta 60 grados, determinando el límite máximo

tolerado.

d)  Capacidad de operar en una Isla Eléctrica y demostrar estabilidad en su operación.

e)  Capacidad de proporcionar Partida Autónoma, si corresponde.

Comisión Nacional de Energía

 25 de 30

—–——–

Título 6 Monitoreo y actualización de parámetros

Título 6  Monitoreo y actualización de parámetros

Artículo 6-1

Señales adicionales de monitoreo

Las  IBR  GFM  deberán  estar  equipadas  con  sistemas  de  registro  capaces  de  medir  los  siguientes
parámetros:

a)  RoCoF conforme al Artículo 3-11 de la NTSyCS.

b)  Registro del ángulo de salto de fase de la red, mediante un método que registre el período de

cada medio ciclo con una resolución de 10 microsegundos.

Artículo 6-2

Actualización de parámetros de control

Las IBR deberán contar con la capacidad de ajustar sus parámetros de control a través de software,
en función de las condiciones del SI o de nuevos requerimientos normativos.

Deben ser ajustables en, al menos, los siguientes parámetros:

a)  Estatismo Permanente del Controlador Frecuencia/Potencia y el Controlador de Tensión.

b)  Tiempos de Respuesta.

c)  Ajustes de banda muerta.

Cualquier  modiﬁcación  en  los  parámetros  de  control  deberá  contar  con  la  autorización  del
Coordinador previo a su implementación y estar en concordancia con las características técnicas de
la instalación.

Comisión Nacional de Energía

 26 de 30

—–——–

Título 7 Disposiciones Transitorias

Título 7  Disposiciones Transitorias

Artículo 7-1

Entrada en vigencia del Anexo

Las disposiciones del Anexo entrarán en vigencia a contar de la publicación, en el Diario Oﬁcial, de
la resolución exenta que lo aprueba.

No obstante, las exigencias relativas a las IBR GFM, establecidas en los Títulos 3, 5, y 6 del Anexo, no
serán  aplicables  a  las  instalaciones  cuya  Entrada  en  Operación  ocurra  dentro  de  los  seis  meses
siguientes a la referida publicación, de acuerdo con lo establecido en la letra e) del artículo 6 del
Decreto N°316, del 07 de Julio de 2023, del Ministerio de Relaciones Exteriores. Asimismo, no les
serán  aplicables  dichas  disposiciones  a  aquellas  instalaciones  declaradas  en  construcción  por  la
Comisión con anterioridad a la fecha de publicación en el Diario Oﬁcial, sin perjuicio de lo señalado
en el Artículo 7-2 del Anexo.

Artículo 7-2

Exención de aplicación del Título 3 del Anexo

Los Sistemas de Almacenamiento de Energía y la componente de almacenamiento de las Centrales
Renovables  con  Capacidad  de  Almacenamiento  que  hayan  sido  declarados  en  construcción  con
anterioridad a la fecha de la publicación de la resolución que aprueba el Anexo, y cuya Entrada en
Operación ocurra transcurridos seis meses desde dicha publicación en el Diario Oﬁcial, deberán dar
cumplimiento a lo establecido en el Título 3 del Anexo.

No  obstante,  los  titulares  de  dichos  proyectos  podrán  solicitar  justiﬁcadamente  a  la  Comisión  la
exención de la aplicación del referido Título 3, dentro de un plazo máximo de cinco meses contados
desde la publicación de la resolución que aprueba el Anexo. Para tal efecto, el interesado deberá
presentar un estudio técnico que fundamente y justiﬁque la imposibilidad de dar cumplimiento a las
exigencias establecidas en dicho Título.

Se considerarán como casos debidamente justiﬁcados, entre otros, aquellos en que el cumplimiento
de las exigencias del Título 3 requiera de ampliaciones o modiﬁcaciones que impliquen adecuaciones
relevantes  al  diseño  original  del  proyecto.  La  Comisión  se  pronunciará  respecto  de  la  solicitud
mediante  resolución  exenta,  pudiendo  eximir  total  o  parcialmente  al  proyecto  respectivo  del
cumplimiento de las exigencias del referido Título 3. Para dicho pronunciamiento, la Comisión podrá
solicitar antecedentes adicionales al Coordinador.

Artículo 7-3

Aplicación de requisitos para la interconexión de IBR GFL

Las  disposiciones  establecidas  en el  Artículo 4-8 del Anexo no  serán  aplicables a  las  IBR GFL que
hubieren obtenido la declaración en construcción al momento de la publicación de la resolución que
aprueba el Anexo en el Diario Oﬁcial.

Comisión Nacional de Energía

 27 de 30

—–——–

Título 7 Disposiciones Transitorias

Artículo 7-4

Entrega de modelos EMT de las instalaciones interconectadas al SI

Las  IBR  interconectadas  al  SI  deberán  presentar  al  Coordinador  los  modelos  EMT  a  los  que  hace
referencia el Artículo 5-1 del Anexo. Para ello, el Coordinador, en un plazo no mayor a tres meses
contado  desde  la  publicación  de  la  resolución  que  aprueba  el  Anexo  en  el  Diario  Oﬁcial,  deberá
deﬁnir un cronograma para la entrega de estos modelos. La asignación de fechas deberá considerar,
entre  otros,  criterios  de  seguridad  e  impacto  en  la  operación  del  SI.  El  cronograma  no  podrá
extenderse por más de un año desde su emisión.

Asimismo, el Coordinador deberá validar los modelos en un plazo no mayor a cuarenta y cinco días
hábiles, contados desde la recepción de estos.

Para las instalaciones existentes que no dispongan de modelos EMT tipo OEM, se podrán entregar
modelos genéricos debidamente validados por un especialista, conforme a los métodos indicados
en el Artículo 5-4 del Anexo.

Artículo 7-5

Exigencias para las IBR GFL existentes

Para dar cumplimiento a las exigencias indicadas en el Artículo 3-9 de la NTSyCS y en el Artículo 4-1,
el Artículo 4-2, el Artículo 4-3, el Artículo 4-4, el Artículo 4-7 y el Artículo 6-2 todos del Anexo, los
titulares de las IBR GFL conectadas al SEN, así como aquellas con declaración en construcción a la
fecha de publicación de la resolución que aprueba el Anexo, deberán presentar al Coordinador, en
un  plazo  no  superior  a  nueve  meses,  un  plan  de  adecuaciones  que  les  permita  cumplir  con  las
exigencias anteriormente referidas.

Dicho plan deberá detallar las modiﬁcaciones de software o hardware de los sistemas de control
vinculados  a  los  convertidores,  incluyendo  una  descripción  de  las  obras,  plazos  de  ejecución,
cronograma de actividades que contemple la coordinación con el Coordinador, entre otros aspectos.
Asimismo,  los  titulares  de  los  Sistemas  de  Almacenamiento  de  Energía  o  la  componente  de
almacenamiento de una Central Renovable con Capacidad de Almacenamiento deberán informar al
Coordinador, en el mismo plazo, la factibilidad de actualizar sus sistemas para operar como una IBR
GFM.

El  Coordinador,  dentro  de  los  seis  meses  siguientes  al  vencimiento  del  plazo  de  nueve  meses
señalado en el inciso anterior, elaborará y publicará en su sitio web un cronograma de adecuaciones,
deﬁniendo  los  plazos  máximos  de  ejecución  de  dichas  adecuaciones  en  función  de  criterios  de
seguridad y de la factibilidad técnica de las mismas. Con todo, el plazo máximo de ejecución de las
adecuaciones no deberá sobrepasar los veinticuatro meses desde la publicación del cronograma.
Excepcionalmente, el Coordinador podrá ampliar el plazo máximo para aquellas instalaciones que
no tengan un mayor impacto en la operación.

En  el  caso  de  las  instalaciones  técnicamente  imposibilitadas  de  cumplir  con  los  requisitos  antes
señalados, los titulares tendrán la obligación de notiﬁcar esta situación al Coordinador en un plazo
máximo de nueve meses a partir de la publicación de la resolución que aprueba el Anexo en el Diario
Oﬁcial, justiﬁcando la referida imposibilidad a través de un informe técnico.

Comisión Nacional de Energía

 28 de 30

—–——–

Título 7 Disposiciones Transitorias

El Coordinador, en un plazo máximo de nueve meses, deberá analizar las razones técnicas expuestas
en el informe técnico y comunicar a la Comisión el análisis realizado. La Comisión deberá emitir una
resolución pronunciándose con un listado de instalaciones técnicamente imposibilitadas de cumplir
con una o más de las disposiciones establecidas en el Anexo. En el caso de que la Comisión rechace
la imposibilidad técnica, la instalación deberá ser incorporada por el Coordinador al cronograma de
modiﬁcaciones mencionado en el inciso tercero anterior.

Artículo 7-6

Requisitos de Información adicional para una IBR GFM

Mientras el Anexo Técnico “Información Técnica de Instalaciones y Equipamiento” de la NTSyCS no
incorpore  expresamente  los  antecedentes  técnicos  exigibles  a  las  IBR  GFM,  los  propietarios,
arrendatarios, usufructuarios o quienes operen, a cualquier título, las instalaciones indicadas en el
Título  3,  deberán  proporcionar  al  Coordinador,  previo  a  su  entrada  en  operación,  al  menos,  la
siguiente información:

a)  Diagrama de impedancia en función de la frecuencia.

b)  Diagrama de Nichols.

c)  Esquema de arquitectura y su diagrama de bloques en Laplace.

d)  Documentación técnica asociada al modelo EMT.

e)  El tipo de IBR GFM (UGBC, SAE, compensación dinámica reactiva, CRCA, entre otros).

f)  Límite de salto de fase en Estado Normal, en grados.

g)  Límite de salto de fase durante contingencias, en grados.

h)  Potencia por Salto de Fase, para una variación de ángulo igual a 10 grados, en [MW].

i)  Potencia de Amortiguamiento Activa para una variación u oscilación de frecuencia del sistema

entre 0,05 [Hz] y 1 [Hz].

j)  Constante de inercia H, determinado mediante:

Donde,

𝐻𝐻 =

𝑀𝑀𝑀𝑀𝑀𝑀 Instalados
𝑀𝑀𝑀𝑀𝑀𝑀 Nominales instalados

: constante de inercia, en [MWs/MVA].

MWs Instalados: capacidad de respuesta inercial de la instalación, en [MWs].
𝐻𝐻

MVA Nominales instalados: capacidad total de la IBR, en [MVA].

k)

 Constante de inercia efectiva

, determinado mediante:

Donde,

𝐻𝐻𝐻𝐻

𝐻𝐻𝐻𝐻 =

𝑆𝑆𝐻𝐻𝑀𝑀𝑅𝑅𝑅𝑅𝐻𝐻𝑀𝑀𝑅𝑅𝑅𝑅 𝑆𝑆𝑅𝑅𝑆𝑆𝑅𝑅𝐹𝐹 ∗ 𝑓𝑓
2 ∗ 𝑆𝑆

Comisión Nacional de Energía

 29 de 30

—–——–

Título 7 Disposiciones Transitorias

: constante de inercia efectiva en [MWs/MVA].

𝐻𝐻𝐻𝐻
Frecuencia de la instalación igual a 2, en [Hz/s].
𝑆𝑆𝐻𝐻𝑀𝑀𝑅𝑅𝑅𝑅𝐻𝐻𝑀𝑀𝑅𝑅𝑅𝑅 𝑆𝑆𝑅𝑅𝑆𝑆𝑅𝑅𝐹𝐹

:  potencia  entregada  o  absorbida  en  respuesta  a  la  Tasa  de  Cambio  de

: frecuencia del SEN, en [Hz].

: capacidad nominal de la instalación, en [MVA].

𝑓𝑓

Sin perjuicio de lo anterior, el Coordinador deberá especiﬁcar la metodología de cálculo en el
𝑆𝑆
Estudio de Análisis de Robustez del SEN vigente.

l)  Capacidad de sobrecorriente de la instalación, en por unidad.

m)  Peak de corriente nominal, en por unidad.

n)  Tensión nominal en el Punto de Conexión, en [kV].

o)  Máxima tensión de la FIV del convertidor para la peor condición, en por unidad (por ejemplo, en
el  punto  de  conexión,  máxima  inyección  de  potencia  reactiva  con  la  tensión  en  el  umbral
superior de acuerdo con el artículo 5-19 de la NTSyCS).

p)  Máximo aporte de cortocircuito trifásico al Punto de Conexión al SI, en [kA].

q)  Máximo aporte de cortocircuito monofásico al Punto de Conexión al SI, en [kA].

r)  Máximo aporte de corriente de secuencia negativa, en [kA].

s)  Factor Equivalente de Amortiguamiento (z).

Comisión Nacional de Energía

 30 de 30

