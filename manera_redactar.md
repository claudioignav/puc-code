SISTEMA DE INFORMACIÓN PARA EMPRESA MINERA Propuesta técnica 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

## **Tabla de contenido** 

|**1.**<br>**RESUMEN EJECUTIVO**|**5**|
|---|---|
|**2.**<br>**EMPRESA**|**7**|
|2.1.<br>¿QUIÉNES SOMOS?|7|
|2.2.<br>NUESTRA MISIÓN|7|
|2.3.<br>NUESTRAVISIÓN|7|
|2.4.<br>TRAYECTORIA|7|
|2.5.<br>NUESTRO EQUIPO|8|
|2.6.<br>NUESTROS SERVICIOS|9|
|**3.**<br>**PROBLEMA**|**10**|
|3.1.<br>DESGLOSE DE LA PROBLEMÁTICA|10|
|_3.1.1._ _Prospecto_|_11_|
|_3.1.2._ _Seguridad_|_13_|
|_3.1.3._ _Recursos Humanos_|_14_|
|_3.1.4._ _Gestión de Proyectos_|_14_|
|_3.1.5._ _Gestión de Usuarios_|_15_|
|3.2.<br>SUPUESTOS DELPROBLEMA|15|
|**4.**<br>**ESQUEMA DE LA SOLUCIÓN**|**17**|
|4.1.<br>ACTORES|17|
|_4.1.1._ _Módulo de Gestión de Proyectos_|_17_|
|_4.1.2._ _Módulo de Recursos Humanos_|_17_|
|_4.1.3._ _Módulo de Finanzas_|_18_|
|_4.1.4._ _Módulo de Seguridad_|_18_|
|_4.1.5._ _Módulo de Soporte_|_18_|
|4.2.<br>DIAGRAMA GENERAL DE LASOLUCIÓN|19|
|_4.2.1._ _Diagrama específico: Módulo de Seguridad_|_20_|
|_4.2.2._ _Diagrama específico: Módulo de Recursos Humanos_|_21_|
|_4.2.3._ _Diagrama específico: Módulo de Finanzas_|_22_|
|_4.2.4._ _Diagrama específico: Módulo de Gestión de Proyectos_|_23_|
|_4.2.5._ _Diagrama específico: Módulo de Soporte_|_24_|
|**5.**<br>**ALCANCE DE LA SOLUCIÓN**|**25**|
|5.1.<br>MÓDULOS DELSISTEMA|25|
|_5.1.1._ _Módulo de Seguridad_|_25_|
|_5.1.2._ _Módulo de Finanzas_|_26_|
|_5.1.3._ _Módulo de Gestión de Proyectos_|_26_|
|_5.1.4._ _Módulo de Soporte_|_27_|
|_5.1.5._ _Módulo de Recursos Humanos_|_28_|
|5.2.<br>REQUERIMIENTOS|29|
|_5.2.1._ _Requerimientos Funcionales_|_30_|
|5.2.1.1.<br>Módulo de Gestión de Proyectos|30|
|5.2.1.2.<br>Módulo de Recursos Humanos|30|
|5.2.1.3.<br>Módulo de Finanzas|31|



1 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

|5.2.1.4.<br>Módulo de Seguridad|31|
|---|---|
|5.2.1.5.<br>Módulo de Soporte|31|
|_5.2.2._ _Requerimientos No Funcionales_|_31_|
|5.3.<br>METODOLOGÍACASCADA|32|
|**6.**<br>**ARQUITECTURA LÓGICA**|**33**|
|6.1.<br>ARQUITECTURALÓGICAMÓDULOGESTIÓN DEPROYECTOS|35|
|6.2.<br>ARQUITECTURALÓGICAMÓDULORRHH|36|
|6.3.<br>ARQUITECTURALÓGICAMÓDULOFINANZAS|37|
|6.4.<br>ARQUITECTURALÓGICAMÓDULOSEGURIDAD|38|
|6.5.<br>ARQUITECTURALÓGICAAPLICACIÓNWEBHELPDESKMÓDULOSOPORTE|39|
|**7.**<br>**ARQUITECTURA FÍSICA**|**40**|
|7.1.<br>INSTALACIONES DE LA OBRA|41|
|7.2.<br>SERVIDOR PARA APLICACIÓN WEB DE RECURSOS HUMANOS Y FINANZAS|42|
|7.3.<br>SERVIDOR DE MICROSERVICIOS|42|
|_7.3.1._ _Módulos, autenticación y orquestador_|_44_|
|7.4.<br>HELPDESK PARA SOPORTE NIVEL1Y2|47|
|7.5.<br>REDUNDANCIA PARA ALTA DISPONIBILIDAD|48|
|7.6.<br>SERVIDOR DE BASE DE DATOS DEL PROVEEDOR|48|
|7.7.<br>TOPOLOGÍA DE RED DE LAOBRA|49|
|_7.7.1._ _Sección de la obra_|_51_|
|_7.7.2._ _Datacenter local de la obra_|_52_|
|7.8.<br>ARQUITECTURA FÍSICA BASADA ENAWS|52|
|_7.8.1._ _Amazon Route 53_|_53_|
|_7.8.2._ _AWS Amplify_|_55_|
|7.8.2.1.<br>AWS Amplify producción|56|
|7.8.2.2.<br>AWS Amplify QA|57|
|_7.8.3._ _AWS S3 Buckets_|_57_|
|7.8.3.1.<br>AWS S3 Bucket producción|58|
|7.8.3.2.<br>AWS S3 Bucket QA|59|
|_7.8.4._ _Amazon API Gateway_|_60_|
|7.8.4.1.<br>AWS API Gateway producción|61|
|7.8.4.2.<br>AWS API Gateway QA|61|
|_7.8.5._ _AWS Lambda_|_62_|
|7.8.5.1.<br>AWS Lambda producción|63|
|7.8.5.2.<br>AWS Lambda QA|63|
|_7.8.6._ _AWS DynamoDB_|_64_|
|7.8.6.1.<br>AWS DynamoDB producción|65|
|7.8.6.2.<br>AWS DynamoDB QA|65|
|_7.8.7._ _Elastic Load Balancing_|_65_|
|_7.8.8._ _Instancia EC2 para servidor de microservicios_|_67_|
|7.8.8.1.<br>AWS EC2 producción|68|
|7.8.8.2.<br>AWS EC2 QA|68|
|_7.8.9._ _Backend web Help Desk (instancia EC2)_|_69_|
|7.8.9.1.<br>AWS EC2 backend Help Desk producción|70|
|7.8.9.2.<br>AWS EC2 backend Help Desk QA|70|



2 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

|_7.8.10._<br>_Amazon Aurora_|_70_|
|---|---|
|_7.8.11._<br>_Amazon ElastiCache_|_72_|
|7.8.11.1.<br>AWS ElastiCache producción|73|
|7.8.11.2.<br>AWS ElastiCache QA|73|
|_7.8.12._<br>_Amazon Elastic Container Registry (Amazon ECR)_|_74_|
|**8.**<br>**PLAN DE IMPLANTACIÓN**|**75**|
|8.1.<br>PROVISIÓN DE DISPOSITIVOS E INFRAESTRUCTURA|75|
|8.2.<br>MARCHA BLANCA|75|
|8.3.<br>PUESTA EN MARCHA|77|
|8.4.<br>CAPACITACIONES|77|
|**9.**<br>**INNOVACIONES**|**78**|
|**10.**<br>**GESTIÓN DEL RIESGO**|**79**|
|10.1.<br>ANÁLISIS DE RIESGO DE LA SOLUCIÓN|79|
|10.2.<br>ANÁLISIS DE RIESGO DE DESARROLLO|81|
|10.3.<br>ANÁLISIS DE RIESGO DE IMPLANTACIÓN|84|
|10.4.<br>ANÁLISIS CUALITATIVO DE RIESGOS|86|
|10.5.<br>EVALUACIÓN DE RIESGOS|87|
|10.6.<br>EQUIPO|93|
|10.7.<br>PLAN DE ACCIÓN|95|
|10.8.<br>PLAN DE RESPUESTA|97|
|**11.**<br>**EDT**|**102**|
|11.1.<br>DICCIONARIO DEEDT|102|
|**12.**<br>**PLANIFICACIÓN DEL PROYECTO**|**119**|
|12.1.<br>HITOS|119|
|12.2.<br>CARTAGANTT|120|
|_12.2.1._<br>_Carta Gantt expandida_|_120_|
|_12.2.2._<br>_Carta Gantt general sin expandir_|_121_|
|_12.2.3._<br>_Carta Gantt con Requerimientos de Producto expandido_|_122_|
|_12.2.4._<br>_Carta Gantt con Administración de proyecto expandido_|_122_|
|_12.2.5._<br>_Carta Gantt con Diseño del sistema de software expandido_|_123_|
|_12.2.6._<br>_Carta Gantt con Desarrollo del sistema de software expandido_|_124_|
|_12.2.7._<br>_Carta Gantt con Pruebas del sistema expandido_|_124_|
|_12.2.8._<br>_Carta Gantt con Implantación expandido_|_125_|
|_12.2.9._<br>_Carta Gantt con Mantención expandido_|_125_|
|**ANEXO 1: REQUERIMIENTOS FUNCIONALES**|**127**|
|**ANEXO 2: REQUERIMIENTOS NO FUNCIONALES**|**136**|
|**ANEXO 3: DIAGRAMA ARQUITECTURA LÓGICA**|**139**|
|**ANEXO 4: DIAGRAMA ARQUITECTURA FÍSICA**|**140**|
|**ANEXO 5: TOPOLOGÍA DE RED DE LA OBRA**|**141**|
|**ANEXO 6: ARQUITECTURA FÍSICA BASADA EN AWS**|**142**|



3 

**ANEXO 7: EDT 143 ANEXO 8: CARTA GANTT EXPANDIDA 144** 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

4 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 1. Resumen ejecutivo 

A lo largo de este documento se revisará y entenderá el desafío del caso Minera, el cual como empresa Digital Dreams nos emociona tomar para así aprender del rubro y toda la experiencia que este nos puede entregar. La primera parte del documento corresponde a la problemática presentada por el cliente, en el cual se desglosa la misma para así entender de mejor manera el cómo este afecta al funcionamiento de la empresa, para luego dar paso al modelo de solución presentado mediante un esquema de fácil entendimiento para quienes lean. 

Como propuesta técnica, y para ahondar más en lo específico, se presenta la sección del alcance de la solución, en donde se desglosa de mejor manera tanto los módulos del sistema con sus subsecciones para explicar cada uno. Dentro del alcance también encontraremos tanto el hardware a adquirir como los requerimientos, tanto funcionales como no funcionales, que se desprenden del esquema de solución presentado. 

Siguiendo en la línea de la solución, se presentarán las arquitecturas lógicas, haciendo énfasis en cada una de las capas que se desarrollarán para lograr que la solución funcione de manera correcta. Por otro lado, se presentará la arquitectura física del proyecto, que contiene, como su nombre lo indica, la infraestructura que dará solución a los módulos, como también la topología de la red necesaria para el correcto funcionamiento de las obras. 

Se presentarán también todas las innovaciones planeadas para implementar en el proyecto, dejando así el sello de calidad que caracteriza a la empresa en cada una de las soluciones aportadas, esperando que estas sean de gran utilidad y cumpliendo con las expectativas de nuestro cliente. 

Por último, se describirán los planes de cómo nuestro equipo planea enfocar el trabajo, empezando por una detallada descripción de los riesgos que se pueden encontrar durante el desarrollo con su análisis, y cómo se tratarán estos riesgos para darle una solución adecuada y pronta en cada caso. Se sigue inmediatamente con el EDT, el cual repasará las etapas en base a los entregables planificados que además cuenta con su propio diccionario para entender el mismo. 

5 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Finalmente, en la sección de la planificación del proyecto se abordarán los hitos de este, ordenados mediante una carta Gantt. 

Sin mucha más explicación, esperamos que encuentre este documento claro y que despeje todas las dudas que tenga acerca del proyecto. 

6 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 2. Empresa 

En esta sección se darán a conocer las principales características de nuestra empresa. 

2.1. ¿Quiénes somos? 

Digital Dreams es una empresa de desarrollo de software creada el 2019 y ubicada en Viña del Mar. Con gran experiencia en proyectos de software de alto impacto e innovación, entregando asesoría a las empresas sobre las nuevas tecnologías y posibilidades en sus proyectos. Contamos con un equipo especializado en distintas áreas, pudiendo entregar soluciones complejas desde aristas variadas. 

### 2.2. Nuestra misión 

Es entregar un software en base a la necesidad del cliente, que funcione bajo los estándares de más alta calidad, entregando un producto especializado, útil y con soporte, diseñado a la medida del problema. Se busca ser la empresa número uno en el desarrollo de software en la región, estableciendo conexiones con el resto de los proveedores para poder dar siempre el mejor producto posible para nuestros clientes. Se quiere llegar a conseguir el prestigio gracias a la calidad de nuestras soluciones y atención al detalle que nos caracterizan. 

### 2.3. Nuestra Visión 

Nuestra visión se basa en las soluciones que podemos entregar a diversas empresas, sean del ámbito que sean, para así generar un estándar de calidad que nos diferencia de cualquier otra empresa proveedora de software, dejando así una marca en todos los clientes que hayan requerido de nuestros servicios, y, por qué no, en el mundo de las soluciones e innovaciones informáticas. 

2.4. Trayectoria 

Digital Dreams nace como un proyecto de un grupo de estudiantes de la Pontificia Universidad Católica de Valparaíso en el año 2018, de la escuela de Ingeniería Informática. Desde entonces hemos brindado diversas soluciones tecnológicas a distintos proyectos a lo largo del país. 

A lo largo de estos años, y gracias a la confianza depositada en nosotros, hemos adquirido experiencia, ampliando nuestro horizonte de capacidades y perfeccionando las habilidades y manejo de herramientas de nuestro equipo. 

7 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

2.5. Nuestro equipo 

Contamos con un amplio equipo capaz de desarrollar las soluciones que el cliente necesite, el cual está compuesto por: 

- Felipe Barja Cárcamo: **Soporte** , es el encargado de dar soporte respecto al desarrollo de la organización, seleccionar y adquirir herramientas y entrenar al personal. 

- Diego Catalán Marchese: **Jefe de proyecto,** es el encargado de gestionar el buen funcionamiento del proyecto, quien supervisa y controla al equipo. 

- Manuel Encina Muñoz: **Analista** , es el responsable de la planificación y coordinación de los trabajos de análisis de los sistemas nuevos y existentes, para luego dar paso a su desarrollo. 

- Amanda Flores Aravena: **Documentador** , es el encargado de diseñar y construir un repositorio de información compartida, donde se almacenará la documentación del proyecto. 

- Felipe Inostroza Órdenes: **Ingeniero de sistemas** , es el encargado de investigar, evaluar y sintetizar información técnica para diseñar, desarrollar y probar sistemas. 

- Sebastián Lillo Acosta: **Coordinador** , es el encargado de la organización del equipo y de la correcta distribución del trabajo. 

- Diego Muñoz Muñoz: **Seguridad** , es el encargado de dictar las políticas de seguridad y protección que deberán seguirse en el diseño, implementación e implantación del sistema. 

- Ignacio Valdebenito Cáceres: **Diseñador** , es el encargado de generar el diseño arquitectónico y diseño detallado del sistema, basándose en los requerimientos. 

- Sebastián Orellana Reyes: **Programador** , es el encargado de implementar en código específico del sistema el software a realizar. 

8 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

- Francisco Mercado Lizana: **Programador** , es el encargado de implementar en código específico del sistema el software a realizar. 

- Pablo Vidal Avalos: **Programador** , es el encargado de implementar en código específico del sistema el software a realizar. 

### 2.6. Nuestros servicios 

Como proveedores, préstamos diferentes servicios que se pueden ajustar a las necesidades de los clientes. Dentro de las posibilidades de desarrollo para nuestros clientes tenemos: 

● Soporte, administración y diseño de sistemas informáticos:  Contamos con personal capacitado para diseñar tus ideas para sistemas informáticos, y así poder poner en orden las ideas informáticas que tenga el cliente en mente. 

● Programación de software: El personal está capacitado para llevar a cabo la programación de diversos proyectos que ya estén diseñados, respaldados por un sello de calidad único que nos caracteriza. 

9 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 3. Problema 

La problemática planteada consiste en la falta de un sistema que permita realizar un correcto seguimiento de las obras. Todo esto se requiere para la implementación de un proyecto minero y operación de la faena: desde la etapa de prospecto, con la gestión de documentos en el análisis del terreno a adquirir; los permisos y estudios de suelo relacionados, hasta la finalización de la obra. También se plantea la necesidad de gestionar el personal que ha sido contratado para la realización de la obra, realizando un correcto seguimiento de estos, tanto de sus contratos como de su seguridad e ingreso a los recintos. Para entender de mejor manera la problemática, es necesario contextualizar el caso. En principio, se trabajará para una empresa consolidada y que maneja un gran número de personal, además de un gran flujo económico. Es por esto, que la solución debe estar a la altura de una empresa de este calibre. También se entiende que la empresa está en una fase de digitalización de sus documentos, por lo que estos se presentan en formato físico. 

### 3.1. Desglose de la problemática 

El problema se plantea en dos partes: En primera instancia se trata el tema del flujo de trabajo de la obra, con sus etapas y procesos; mientras que en la segunda parte se tratará el sistema gestor de recursos humanos. Para un mejor desglose de los problemas que tiene actualmente la empresa, se analizará el flujo de trabajo de los procesos que debe completar la obra para ser aceptada, separando así dos ideas de flujo de trabajo, siendo tratada la primera como prospecto de obra y la segunda como gestión del proyecto. 

10 



<!-- Start of picture text -->
ZO DIGITAL<br><!-- End of picture text -->



<!-- Start of picture text -->
1<br>a<br>.GP<br><!-- End of picture text -->



<!-- Start of picture text -->
Ilustración 1<br><!-- End of picture text -->

3.1.1. Prospecto 

Se entiende como prospecto a la idea de un proyecto en cierta zona del país. Para esto, se analizan posibles terrenos a adquirir, el proceso de saneamiento, el proceso de adquisición y obtención de permisos, tanto medioambientales como los de extracción y de producción. En base a lo anterior, se evalúa la adquisición del sitio. Finalmente, se continúa con el estudio de suelo, informes y el diseño final de la obra. 

11 





<!-- Start of picture text -->
Analisis de terreno a adquirir<br>© Estudio de suelos, andlisis de calidad porcentual de minerales.<br>© Analisis viabilidad de extraccion de minerales.<br>Proceso de adquisicion<br>e Inicio de proyectos de estudio de suelos para construccién.<br>« Realizacion de informes y disefio de obra.<br>e Proceso de disefio de planos del proyecto.<br>Proceso de saneamiento del terreno<br>« Disefio de proyecto plan para saneamiento al cierre de Faenas.<br>© Identificacion de riesgos e impactos ambientales.<br>© Identificacion de criterios ambientales y medidas minimas<br>Proceso de adquisicion de permisos medioambientales<br>e Ingreso solicitud evaluacion y autorizacion del proyecto para permiso sanitario a las entidades<br>correspondientes.<br>© Ingreso de solicitud de evaluacién y autorizacin de proyecto de plan para saneamiento.<br>e Evaluacion de resultados ante respuesta a solicitudes ingresadas:<br>© Caso parcialmente rechazado: Se corrige hasta su aprobacion.<br>© Caso rechazo total: Se inicia una nueva obra, dando inicio a nuevos estudios e informes para<br>su posterior evaluacion.<br>Proceso de adquisicion de permisos de extraccion<br>© Analisis y disefio de proyecto de métodos de explotacion.<br>e Ingreso solicitud de aprobacion de proyecto de método de explotacion<br>« Evaluacion de resultados ante respuesta solicitada:<br>© Caso parcialmente rechazado: Se corrige hasta su aprobacion.<br>Caso rechazo total: Se inicia nueva obra dando inicio a nuevos estudios e informes para su<br>posterior evaluacion.<br>Proceso de adquisicion de permisos de produccion<br>Proyecto gestion de plantas de procesamiento de minerales<br> Evaluaci6n de resultados ante respuesta solicitada:<br>© Caso parcialmente rechazado: Se corrige hasta su aprobacion.<br>¢ Caso rechazo total: Se inicia nueva obra dando inicio a nuevos estudios e informes para su<br>posterior evaluacion.<br><!-- End of picture text -->

_Ilustración 2_ 

12 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Los problemas asociados a esta fase, conforme con el sistema que se debe desarrollar se pueden resumir en: 

● La inexistencia de un sistema que reúna los documentos y permisos necesarios, concedidos para una gestión organizacional eficaz, control y resguardo de estos. 

● La inexistencia de un sistema que gestione el flujo de trabajo del prospecto y los estados de las etapas mencionadas anteriormente, como también sus resultados. 

3.1.2. Seguridad 

Al ser una empresa que trabaja en proyectos con información sensible, gran cantidad de personal y también proveedores, la seguridad debe ser una prioridad para controlar los accesos y el resguardo de la infraestructura. Para este caso, en donde no existe sistema alguno, se identifican y analizan los siguientes puntos: 

● No existen identificaciones, algo primordial para la trazabilidad del personal en la obra. 

● No existe digitalización de la información de los contratos del personal externo, esto para verificar que los contratos estén vigentes. 

● No existen respaldos distribuidos estratégicamente del sistema en caso de contingencias. 

● No existe la protección ante pérdidas o robos de los dispositivos del personal. 

● No existe un control de acceso con las normativas de seguridad adecuadas. 

13 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### 3.1.3. Recursos Humanos 

En el caso de recursos humanos, pese al gran volumen de personas que se tiene que manejar y la gran cantidad de rotaciones que se presentan entre estos, no existe un sistema que permita facilitar su administración, identificando las siguientes debilidades: 

● La falta de una correcta gestión del personal y sus correspondientes remuneraciones. 

- La ineficiencia a la hora de distribuir y planificar los turnos. 

- La ineficacia en las evaluaciones de desempeño del personal. 

- La falta de controles de asistencia. 

En este punto, se presenta otro problema, ya que no existe actualmente un 100% de digitalización de documentos y contratos. Por ende, no se tiene control y supervisión correcta de estos mismos, pudiendo existir pérdidas de información y de legibilidad afectando la integridad propia de la documentación tratada. También, a pesar de que la empresa trabaja con múltiples proveedores, no posee un método eficaz para distinguir si el personal, que circula por las obras, corresponde a empleados de la propia compañía o de algún proveedor en específico con su contrato vigente. Tampoco se verifica si este personal cumple con los cursos y equipamientos apropiados para realizar el trabajo. 

#### 3.1.4. Gestión de Proyectos 

En el caso de la gestión del proyecto presentado, debido a la inexistencia de un sistema que trabaje por encima de toda la información de la minera, es vital reconocer todas las deficiencias asociadas al tráfico de información y la disposición de ésta. Actualmente, no se responde eficazmente a todas las necesidades administrativas. También, faltan herramientas que permitan ordenar y jerarquizar todas las solicitudes, automatizando las interacciones de éstas. A raíz de esto, se pueden identificar las siguientes problemáticas: 

● La falta de control para gestionar, administrar y controlar los documentos ya sea planos, permisos o informes en un sistema centralizado. 

14 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

● No existe la posibilidad de gestionar un flujo de trabajo en los proyectos y sus tareas respectivas. 

● No existen herramientas de comunicación que permitan notificar, alertar o advertir a sobre el estado de las tareas y/o situaciones ocurridas en el proyecto. 

● Los documentos no poseen un código identificador, tampoco registro de las fechas, ya sea de subida o de actualización. 

● No hay herramientas efectivas para la elaboración y almacenamiento de bitácoras, notas e imágenes satelitales. 

3.1.5. Gestión de Usuarios 

Es un hecho que el sistema en la actualidad no cuenta con ninguna infraestructura que les permita a los usuarios identificarse al momento de realizar cualquier solicitud. Ante esta enorme problemática, para poder traspasar la documentación de manera precisa y segura podemos recalcar: 

● La falta de un sistema que gestione cuentas de usuarios, de manera de tener un control y resguardo del trazado de la información en el sistema. 

3.2. Supuestos del Problema 

En esta sección, se revisarán los supuestos de la problemática. Se asumirá que: 

- La empresa no cuenta con ninguna obra en la actualidad y solo cuenta con proyectos en sus etapas de investigación. 

- Un trabajador solo tiene acceso y permisos para la obra en la que fue contratado. 

- La empresa comenzará a usar el nuevo sistema desde el inicio de un nuevo prospecto. 

- La empresa maneja alrededor de 2000 y 5000 trabajadores, distribuidos en todas las obras. 

15 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

- La empresa cuenta con personal de finanzas que no tiene ningún software especializado que facilite la realización de su trabajo. 

- Los trabajadores en terreno de cada obra cuentan con un mecanismo de comunicación con una estación central de la empresa. 

- La empresa contará con las adquisiciones necesarias relacionadas a los módulos de finanzas y de recursos humanos, dentro de los cuales se encuentran oficinas, computadores compatibles con el sistema a implementar y proveedores de internet. 

16 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 4. Esquema de la Solución 

A continuación, se presenta el esquema de la solución planteada, la cual se va a encontrar dividida en varios módulos que, a su vez, solucionan los problemas específicos de su área con el objetivo de responder de manera efectiva a las necesidades de la empresa, también se toma en cuenta que la fragmentación de la solución en módulos permite priorizar las áreas que sean de mayor interés, y que, por tanto, necesiten más enfoque y revisión. 

### 4.1. Actores 

En esta sección, se especificarán los actores que interactúan con el sistema planteado como solución. 

4.1.1. Módulo de Gestión de Proyectos 

● **Administrador de módulo de gestión de proyectos** : encargado de administrar el módulo de gestión de proyectos y sus usuarios. 

● **Jefe de proyecto** : encargado de gestionar el proyecto del cual esté a cargo y a sus participantes. Debe controlar los plazos y costos del proyecto. 

● **Participante de proyecto** : encargado de subir documentos necesarios con el fin de validar el estado en el que se encuentre la obra. 

● **Empleado de proveedor:** empleado de un proveedor que tiene acceso a las instalaciones. 

4.1.2. Módulo de Recursos Humanos 

● **Administrador de módulo de recursos humanos** : encargado de administrar el módulo de RRHH. 

● **Trabajador RRHH** : encargado de gestionar trabajadores del sistema, sus contratos, de la compañía o de proveedores; sus remuneraciones, planificación de turnos, evaluaciones de desempeño, todo de manera digital. 

17 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

4.1.3. Módulo de Finanzas 

● **Administrador de Módulo de finanzas** : encargado de administrar trabajadores del módulo de finanzas. 

● **Trabajador de finanzas** : encargado de hacer seguimiento de gastos en general, tales como, remuneraciones de trabajadores, pagos y facturas de la minera y flujos de cualquier tipo. 

4.1.4. Módulo de Seguridad 

● **Administrador de Módulo de seguridad** : encargado de administrar el módulo de seguridad. 

● **Trabajador de seguridad** : encargado de verificar que las condiciones de seguridad de los trabajadores se cumplan y validar su identidad. 

4.1.5. Módulo de Soporte 

● **Administrador:** encargado de gestionar roles de administradores del resto de los módulos, ya sea de gestión de proyectos, de recursos humanos, de finanzas y de seguridad. 

● **Trabajador:** corresponde a trabajador de la empresa el cual enviará una solicitud al módulo de soporte. 

● **Operario de soporte nivel 1:** encargado de atender solicitudes de problemas técnicos básicos recibidas en el respectivo módulo. Además, este puede derivar solicitudes, si es requerido debido al nivel de complejidad, a operario de soporte de nivel 2. 

● **Operario de soporte nivel 2:** especializado en software encargado de atender solicitudes de problemas específicos recibidas en el respectivo módulo. 

18 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

### 4.2. Diagrama general de la Solución 

El software que se plantea como solución se basa en un sistema conectado a un servidor central, el cual recibe y envía datos entre diferentes módulos, siendo el más importante el módulo de gestión proyectos, donde se llevará registro de todas las obras en general. Por otro lado, también se encuentran los módulos de finanzas, de recursos humanos, de seguridad y de soporte, siendo este último en donde se gestionan los roles de administradores independientes de todos los módulos ya mencionados. 



<!-- Start of picture text -->
2<br>eae= Sistema Central MéduloRRHHde<br>proyectos |<br>Médulode<br>Seguridad<br><!-- End of picture text -->

_Ilustración 3_ 

19 



<!-- Start of picture text -->
DDIGITALDREAMS<br><!-- End of picture text -->

4.2.1. Diagrama específico: Módulo de Seguridad 

Dentro del módulo de seguridad, encontramos la existencia de una tarjeta de identificación física, la cual indicará claramente el rol que alguien desempeña en el lugar de trabajo (proveedor, trabajador de la faena, etc.). Cada trabajador de la empresa perteneciente a cualquier área y/o módulo y empleado de algún proveedor contará sí o sí con este elemento. Así también, quién deja registro en el software de todo el personal que entra al área de trabajo es el trabajador de seguridad. Esto se realizará vía laptop entregada. Todo el personal que va a trabajar a terreno tiene que cumplir con las medidas de seguridad, esto también quedará registrado en el software ingresado manualmente por este trabajador. La persona encargada de verificar que todo esto se cumpla de manera correcta, tanto al momento de ingresar datos en el software como en el mismo lugar de trabajo (entrega de tarjetas de identificación, laptop para el trabajador de seguridad, etc.) es el Administrador de módulo de seguridad. También será el encargado de gestionar a los trabajadores de este módulo. 



<!-- Start of picture text -->
i- —_<br>/ TMédulo de Visualizacept aci é6 n  y<br>mma<br>equipamientoy<br>Administrador£ | g eersy=e<br>médulo de Identificacionpor tarjeta TrabajaSeguri d ador “2ueeruen<br>seguridad<br>tas<br>Participantede proyecto —_Empleado proveedorde<br><!-- End of picture text -->

_Ilustración 4_ 

20 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

4.2.2. Diagrama específico: Módulo de Recursos Humanos 

Dentro del módulo de recursos humanos, encontramos cuatro grandes categorías de las que se encargan los trabajadores de esta área, siendo estas: contratos, planificación de turnos laborales, evaluación de desempeño a los trabajadores de la empresa y finalmente una recolección de opinión por parte de los empleados. Además, todos los trabajadores de la empresa pasarán por un control de asistencia biométrico mediante huella dactilar, el cual enviará el registro directamente al módulo. La función en el software de los trabajadores de RR.HH. será subir los documentos relacionados a las categorías mencionadas anteriormente. Existirá un administrador de recursos humanos, quien será el encargado de gestionar a los trabajadores y que todo el flujo de trabajo dentro del mismo módulo funcione correctamente. 



<!-- Start of picture text -->
m—aN  2<br>g — 6<br>Admini: dor<br>-—— 1<br>Contratos Mir eect — main Seguro<br>L—1—____f#—___1____J<br>‘Trabajador<br><!-- End of picture text -->

_Ilustración 5_ 

21 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

4.2.3. Diagrama específico: Módulo de Finanzas 

Al igual que en los demás módulos, está la presencia de un Administrador de módulo de finanzas, esta es la persona encargada de gestionar a los trabajadores del módulo y verificar que todo esté funcionando correctamente, tanto a nivel de personal como dentro del mismo software. La función de los trabajadores de finanzas es subir los documentos necesarios que tengan que ver con el área (informes, cuentas de cada proyecto). 



<!-- Start of picture text -->
Informes de Cuentas de<br>finanzas proyecto<br>Trabajador<br>Finanzas<br><!-- End of picture text -->

_Ilustración 6_ 

22 



4.2.4. Diagrama específico: Módulo de Gestión de Proyectos 

En el módulo de gestión de proyectos se encuentra todo el proceso por el que pasa una obra, desde la adquisición de terreno hasta la finalización de esta. Para controlar cada etapa del proyecto, el software usará un sistema tipo workflow. En el siguiente diagrama, se muestra la lógica de cómo funcionará a nivel general este sistema en el cual, un participante del proyecto podrá recibir documentos y validar que estos estén correctos, para luego comenzar con su etapa del workflow y subir sus documentos correspondientes. Además, es importante mencionar que algunos documentos a subir en el software son permisos que otorga alguna institución gubernamental (municipalidad, ministerio del medio ambiente, etc.). El encargado de chequear que todo el flujo de trabajo esté libre de errores o irrupciones, será un jefe asignado a cada proyecto. 



<!-- Start of picture text -->
Administrador<br>De Médulo de<br>Gestion de<br>Participante visualiza<br>ysube documentos<br>méduloPertinentesa su etapaal<br>— «> — = «—<br>7) de gestién de proyectos.<br>ed : 2 >— i<br>Médulo de Documentos 7<br>Gestion de Participante Permisos Institucién<br>proyectos \ J de proyecto Gubernamental<br>Participante La ignada Servicio de<br>de proyecto said[ Geolocalizacion<br>2 ra ;<br>Participante Inventario<br>de proyecto<br><!-- End of picture text -->

_Ilustración 7_ 

23 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

4.2.5. Diagrama específico: Módulo de Soporte 

Inicialmente, en este módulo podemos encontrar a un administrador, el cual será el encargado de gestionar las cuentas de administradores del resto de los módulos existentes en el sistema, es decir, asignará los roles a quienes se encargarán de llevar el correcto funcionamiento de los respectivos módulos. Por otro lado, podemos encontrar operarios de soporte de nivel 1 y de nivel 2, los cuales estarán encargados de atender solicitudes de soporte enviadas por los trabajadores de los mismos módulos ya mencionados, ya sean de clasificación presencial o remota. Además, las solicitudes también serán asignadas a los operarios dependiendo del nivel de complejidad y especificación del problema. 



<!-- Start of picture text -->
g—<br>Trabajador Solicitud<br>£—9-®<br>Administrador epore Sontnnied ,<br>‘solicitud operario de nivel 2<br>\ ‘Operario de nivel! puede escalar<br>Operario<br>Soporte nivel 2<br><!-- End of picture text -->

_Ilustración 8_ 

24 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 5. Alcance de la solución 

A continuación, en el alcance de la solución se aborda la creación de un sistema que permite agilizar procesos tanto administrativos como de gestión, además integra desde la identificación de usuarios hasta al seguimiento de los recursos financieros. En esta etapa también se encuentran detallados los diversos dispositivos hardware a utilizar en cuestión. 

### 5.1. Módulos del Sistema 

A continuación, se describirán los módulos considerados para el sistema como parte del alcance de la solución. 

#### 5.1.1. Módulo de Seguridad 

Con lo importante que es la seguridad en la industria minera, en especial en las faenas, se requiere implementar un sistema de seguridad que verifique a los empleados que entran y salen de las instalaciones. Esto debido a la posibilidad de robo de materiales y al alto riesgo de accidentes en las instalaciones. Tomando en cuenta la i _lustración 4_ se tienen los siguientes procesos: 

Verificación de entrada: 

- Se verificará la tarjeta de identificación del usuario. 

- Se revisará que el empleado tenga toda la indumentaria de seguridad correspondiente. 

- El empleado de seguridad deja registro en su equipo. 

Verificación de salida: 

- Se verificará la tarjeta de identificación. 

- Se revisará que el empleado tenga toda la indumentaria de seguridad correspondiente. 

25 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

- El empleado de seguridad deja registro en su equipo. 

5.1.2. Módulo de Finanzas 

El módulo de finanzas es sumamente importante para la empresa, ya que se encarga de la gestión de dineros de esta, además es imprescindible hacer un seguimiento de todos los movimientos del presupuesto, para que todo el proceso sea lo más transparente posible. 

El responsable directo es el administrador de finanzas, bajo su dirección se encuentra el empleado de finanzas y son los principales actores del guardado de toda la información económica. Entre sus tareas se encuentran: 

- El empleado de finanzas revisará los **informes** de facturas de la minera. 

- El empleado de finanzas revisará los flujos de dinero en **cuentas** de proyectos. 

- El empleado de finanzas administra cualquier otro tipo de caso no previsto para efectos de adquisición de recursos. 

- El administrador de finanzas verificará los informes y cuentas del empleado de finanzas. 

5.1.3. Módulo de Gestión de Proyectos 

En este módulo, para efectos de control de los eventos de la minera, tiene asociada a sí toda la información de los participantes en el proyecto, en consecuencia, el jefe que dirija el proyecto podrá administrar las responsabilidades, conociendo el panorama general de la empresa. Podemos destacar: 

- **Documentos:** Todos los documentos nuevos y antiguos se traspasan al sistema, delegando la responsabilidad al jefe de proyecto para consultarlo y editarlo según estime conveniente. Además, todos los permisos que estén relacionados a la viabilidad del proyecto también serán almacenados y podrán ser consultados. 

26 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

- **Proyectos:** Cada dato nuevo, asociado a un proyecto específico, estará disponible en conjunto de los documentos y permisos necesarios, para que el jefe de proyecto lo administre directamente, es decir, podrá modificar, eliminar elementos, añadir nuevos proyectos y todo el detalle de los movimientos y estados. 

- **Permisos** : Los permisos que sean otorgados por la institución externa al participante del proyecto deben ser traspasados a la plataforma virtual; una vez se encuentren en el sistema el jefe de proyecto una vez compruebe la integridad de la información, procederá a traspasar los nuevos datos. 

- **Servicio de Geolocalización** : Cada laptop asignada desde el jefe al participante del proyecto pasará por una verificación de ubicación, con el propósito de evitar que algún tercero no autorizado pueda tener acceso a información delicada o importante sobre los proyectos. Además, el jefe tendrá la facultad de distribuir las laptops según las prioridades de cualquier tarea a ejecutar. 

#### 5.1.4. Módulo de Soporte 

El módulo de soporte tiene como principal tarea recibir las solicitudes de problemas que tengan los trabajadores del resto de los módulos, ya sea, que requieran asistencia remota o presencial y específica o general. Este módulo cuenta con dos niveles de soporte, el de nivel 1 y el de nivel 2. En el caso del primero, se encuentra enfocado en atender problemas de nivel técnico y de menor complejidad. Por otro lado, se encuentra el soporte de nivel 2, el cual también está encargado de atender problemas técnicos, pero de una complejidad superior en comparación a las de nivel 1. Para ello, en este módulo se cuenta con actores respectivos para cada nivel, y dentro de los operarios de soporte de nivel 1, estos pueden derivar solicitudes a operarios de nivel 2 si consideran que la solicitud es de una complejidad no acorde a sus funciones. Finalmente, este módulo también cuenta con otra función, la cual corresponde a la asignación de roles de administradores de los otros módulos ya mencionados. Para ello, el administrador será quién realizará esta tarea. 

27 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### 5.1.5. Módulo de Recursos Humanos 

En este módulo se gestiona principalmente al personal y las remuneraciones de los empleados de la empresa, además de hacer control de asistencia de sus trabajadores, gestionar sus contratos y planificar los turnos de los empleados. El actor que tendrá mayor injerencia en este módulo es el administrador de recursos humanos. Dentro de la información que se maneja dentro de este módulo, se puede encontrar: 

- Empleados: 

   - RUT. 

   - Nombres. 

   - Apellidos. 

   - Huella dactilar asociada. 

   - Información de contacto: 

      - Fono. 

      - E-mail. 

   - Tipo de empleado: Interno o externo. 

   - Estado: activo, inactivo o desvinculado. 

- Contratos: registro de contratos del empleado. 

   - Número de documento. 

   - Datos del empleado. 

   - Sueldo base. 

- Horarios: horarios de trabajo del empleado 

   - Número de documento. 

   - Datos del empleado. 

   - Tiempo de validez horario. 

- Horas extras: registro de las horas extras realizadas por el empleado. 

   - Datos del empleado. 

   - Número de documento. 

   - Fecha: corresponde a los días y cantidad de horas extra. 

28 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

- Liquidaciones: registro de liquidaciones. 

   - Número de documento. 

   - Datos del empleado. 

   - Liquidación y fecha de esta 

- Descuentos: descuentos de impuesto a la renta, AFP, Isapre y seguros. 

   - Datos del empleado. 

   - Número de documento. 

   - Porcentaje de descuento 

- Asistencias: registro de asistencia del empleado. 

   - Datos del empleado. 

   - Número de documento. 

   - Hora entrada. 

   - Hora de salida. 

Con esos datos se podrá: 

- Asignación de horarios: el sistema dejará ingresar los horarios de los empleados por parte de empleados de RRHH. 

- Control de asistencia manual: los empleados de RRHH ingresarán de manera manual las asistencias registradas en caso de que falle el dispositivo de control de asistencia biométrico. 

- Control de remuneraciones: a partir de los registros anteriores. Finalizado el periodo de trabajo, mensual o quincenal se determinarán los pagos a el empleado, sueldo, bonos, descuentos que correspondan a el empleado. 

### 5.2. Requerimientos 

En la siguiente sección, se presentan los requerimientos funcionales y no funcionales identificados a partir de la propuesta realizada. 

29 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### 5.2.1. Requerimientos Funcionales 

A continuación, se presentan los requerimientos funcionales del inicio de sesión y de los demás módulos del proyecto. Para verlos en detalle, revisar Anexo 1. 

● Iniciar sesión (RF01-01). 

_5.2.1.1. Módulo de Gestión de Proyectos_ 

En este apartado se expresan los requerimientos funcionales del módulo de gestión de proyecto. 

- Gestionar proyectos (RF02-01). 

- Gestionar recordatorio predeterminado (RF02-02). 

- Gestionar Actividades (RF02-03). 

- Gestionar Participantes por especialidad de proyectos (RF02-04). 

- Realizar actividad (RF02-05). 

- Evaluar tarea recibida (RF02-06). 

- Gestionar los documentos (RF02-07). 

- Controlar costos de etapas y tareas de un proyecto (RF02-08). 

- Controlar plazos de etapas y tareas de un proyecto (RF02-09). 

#### _5.2.1.2. Módulo de Recursos Humanos_ 

En este apartado se expresan los requerimientos funcionales del Módulo de Recursos Humanos. 

- Gestión de credenciales para trabajadores de recursos humanos (RF03-01). 

- Gestión de contratos (RF03-02). 

- Gestión de turnos (RF03-03). 

- Control de remuneraciones (RF03-04). 

- Evaluación de desempeño (RF03-05). 

- Firmar un contrato de trabajo (RF03-06). 

- Gestión de seguros (RF03-07). 

30 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### _5.2.1.3. Módulo de Finanzas_ 

En este apartado se expresan los requerimientos funcionales del Módulo de Finanzas. 

- Gestionar proveedores (RF04-01). 

- Gestionar cuentas de gastos (RF04-02). 

#### _5.2.1.4. Módulo de Seguridad_ 

En este apartado se expresan los requerimientos funcionales del Módulo de Seguridad. 

- Verificación de acceso (RF05-01). 

- Verificar cursos y equipamiento (RF05-02). 

- Creación de tarjeta de identificación (RF05-03). 

#### _5.2.1.5. Módulo de Soporte_ 

En este apartado se expresan los requerimientos funcionales del Módulo de Soporte. 

- Gestionar trabajadores de soporte (RF06-01). 

- Crear solicitud de soporte (RF06-02). 

- Gestionar solicitud de soporte (RF06-03). 

- Escalar solicitud de soporte (RF06-04). 

- Marcar solicitud como resuelta (RF06-05). 

   - 5.2.2. Requerimientos No Funcionales 

A continuación, se presentan los requerimientos no funcionales del sistema. 

- Seguridad por Geolocalización (RNF01-01). 

- Alta disponibilidad (RNF01-02). 

- Soporte remoto (RNF01-03). 

31 



<!-- Start of picture text -->
ZDDIGITALDREAMS<br><!-- End of picture text -->

- Alta portabilidad (RNF01-04). 

- Interfaz gráfica intuitiva (RNF01-05). 

- Sistema de alertas (RNF01-06). 

- Datacenter primario (RNF01-07). 

- Datacenter secundario (RNF01-08). 

- Funcionamiento off line (RNF01-09). 

### 5.3. Metodología Cascada 

Con respecto a la metodología de desarrollo a utilizar, esta será la metodología en cascada, debido a que, como empresa tradicional, se lleva trabajando con esta desde sus inicios. Esto significa que se utilizará un modelo iterativo en el cual cada una de sus fases se basará en la anterior y se verificarán los resultados de esta. 



<!-- Start of picture text -->
Definicion de<br>Requerimientos<br>Diseiio del Software|<br>y del Sistema<br>Implementacion y<br>Prueba de unidades<br>del Sistema<br>Operacién y<br>Mantenimiento<br><!-- End of picture text -->

_Ilustración 9_ 

32 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 6. Arquitectura Lógica 

A continuación, se presentará la arquitectura lógica para el sistema a desarrollar. En la _ilustración 9_ , se aprecia una arquitectura de 3 capas, las cuales son: Capa de presentación, Capa de Negocios y Capa de Datos. 

En la primera capa, de presentación, se encuentran las aplicaciones y servicios que interactúan directamente con el usuario, recibiendo y mostrando la información correspondiente a cada una. En la segunda capa, de Negocios, se gestionan las funciones principales de cada aplicación o servicio, procesando los datos y permitiendo su correcta administración para luego ser almacenados y/o mostrados al usuario. Finalmente, en la tercera capa, de datos, está conformada por los servicios que proporcionan los datos persistentes a los módulos que necesiten acceder a los datos, tantos documentos, información de trabajadores, identificación de personal, gestión de cuentas, entre otros; que estarán disponibles para ser gestionados en las capas superiores. 

33 





<!-- Start of picture text -->
Ee=RRHHY Cliente para<br>Aplicacion control de<br>\SDE=D Aplicacién de escritorio Vv acceso de<br>phases Médulo Gestion de Proyectos Médulo deFinanzas Médulo deRRHH. médulo deseguridad<br>= anVv g 4} nNVv<br>a > 4<br>Capa Presentacion = Vv| & ServicioVvZ para | ServicioV7» para VY4 oe<br>Servicio para|| Servicio Servicio para Servicio para<br>‘gestion de para gestionde _gestién de cuentasgestion dede ‘contratosgestion de Serviciogestion para de<br>‘cuentas || gestionde actividades documentos gastos t identficacion<br>\____] archivos ‘Servicio eepara<br>local Servicio paragestion de -Setviciode. Nace<br>Servicio de inventario desempetio<br>gestionSolicitudclientesparade seoctontie,  Seectortae, _ BroveedoresServiciogestion para de Servicio‘controlo  para de<br>permisos mensajeria_ seietenicin<br>, Servicio para Servicio para<br>Serviciopara “gestion de gestion de<br>nestor | Parnas Feeunerecones<br>Servicio para<br>gestion de firma<br>digital<br>ServicioCargasegurosdepara<br>Capa de Negocios erihees A4S: a> oa ———| ><br>| Base de<br>| Datos |<br>Local | |<br>Vv Vv V v Vv<br>Base de<br>datos<br>Capa de Datos eobel<br><!-- End of picture text -->

_Ilustración 10_ 

34 



6.1. Arquitectura Lógica Módulo Gestión de Proyectos 

El esquema lógico del Módulo de Gestión de proyectos consta de una aplicación en la capa de presentación que interactúa directamente con el servicio para gestión de archivos local y su base de datos correspondiente en la capa de datos. Esto permite al usuario almacenar la información y documentos mientras la aplicación no tenga internet. Además, puede conectarse a los demás servicios de la nube a través del API GATEWAY, gestionando toda transacción relacionada al módulo, almacenando y/o mostrando la información en la aplicación, por ejemplo, notificaciones y mensajes. 

_Ilustración 11_ 

35 



6.2. Arquitectura Lógica Módulo RRHH 

El módulo de RR.HH. tiene la finalidad de facilitar la gestión de contratos, evaluación de desempeño, remuneraciones, firmas digitales y, además, el control de asistencia, información que es capturada por el lector biométrico y enviada hacia el servicio para el control de asistencia, para ser verificada y almacenada posteriormente en la base de datos global. 



<!-- Start of picture text -->
‘Aplicaci6n Web RR.HH y Finanzas<br>———<br>Vv<br>‘Médulo de RR.HH.<br>Capa Presentacién | APIGATEMMAY<br>i<br>Servicio para gestién de contratos<br>aed pr nl ene<br>Seni para cone dase<br>Servicio para gestion de remuneraciones<br>Servet pa ges de mata<br>Seri pra capa ops<br>“N<br>Capa de Negocios J.<br>Base de<br>datos<br>Capa de Datos global<br><!-- End of picture text -->

_Ilustración 12_ 

36 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

6.3. Arquitectura Lógica Módulo Finanzas 

El módulo de Finanzas permite gestionar la contabilidad general de la empresa minera, permitiendo la gestión de proveedores, administración y gestión de cuentas de gastos. Este módulo es accedido directamente desde la aplicación web de RR.HH. y Finanzas. 

_Ilustración 13_ 

37 



<!-- Start of picture text -->
ZDDIGITALDREAMS<br><!-- End of picture text -->

### 6.4. Arquitectura Lógica Módulo Seguridad 

El módulo de seguridad tiene por objetivo manejar el control de acceso a las secciones de las obras y obtener la información necesaria para realizar el control de identidad mediante la aplicación móvil instalada en el Handheld. Ambos son representados como un cliente que envía la información de la tarjeta RFID utilizando el API Gateway como puerta de enlace hacia el servicio de gestión de identificación. Los propósitos de este servicio son principalmente dos: el primero confirma la identidad del dueño de la tarjeta y envía una señal al cliente para que este desactive el torniquete y le permita pasar; el segundo permite obtener información de la persona mediante la lectura de su tarjeta RFID, retornando información sobre la identidad del empleado junto a su contrato. Todas estas funciones son realizadas utilizando los datos de la capa de datos, mediante la base de datos global. 

_Ilustración 14_ 

38 



<!-- Start of picture text -->
ZDDIGITALDREAMS<br><!-- End of picture text -->

6.5. Arquitectura Lógica Aplicación Web Help Desk Módulo Soporte 

Se dispone de una aplicación web en la capa de presentación que permite a los empleados de la obra y a los de soporte TI nivel 1 y 2 conectarse a los servicios de soporte proporcionados por la capa de negocios. El primer servicio corresponde al de gestión de cuentas, que permite a los administradores crear nuevos usuarios con roles específicos. El servicio de gestión de solicitudes permite a los empleados de las obras enviar solicitudes a los empleados de soporte, y a estos últimos les permite gestionarlas, resolviendo los problemas o derivando a un nivel superior de soporte. Todas estas funciones son realizadas utilizando los datos de la capa de datos, mediante la base de datos global. 

_Ilustración 15_ 

39 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 7. Arquitectura Física 

A continuación, se presenta la arquitectura física, cuyo objetivo es modelar con detalle la infraestructura diseñada para dar solución a los módulos. Además, se presenta la topología de red necesaria para que los empleados de la obra puedan realizar sus funciones. Esta podrá apreciarse de mejor manera en el Anexo 4. 



<!-- Start of picture text -->
y<br>i _ =]. se 7 es<br>1]<br><!-- End of picture text -->

_Ilustración 16_ 

40 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

7.1. Instalaciones de la obra 

En este diagrama se identifican las interfaces que harán uso de los servicios del servidor principal, poniendo como caso de uso las computadoras correspondientes a los actores de la solución. La aplicación de escritorio contendrá una base de datos local para continuar las operaciones offline. 



_Ilustración 17_ 

41 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

7.2. Servidor para aplicación web de recursos humanos y finanzas 

Es necesario contar con un servidor para alojar la aplicación web de RR.HH. y finanzas, con el objetivo de separarla del servidor que contiene los microservicios para así realizar un escalador vertical u horizontal dependiendo de lo que se necesite. 



<!-- Start of picture text -->
cmpleado RR.HH<br>Gente del<br>t= | Servidor<br><!-- End of picture text -->

_Ilustración 18_ 

### 7.3. Servidor de microservicios 

Se considera la contratación de un servicio de virtualización en la nube de un proveedor bajo una arquitectura de microservicios, donde se implementará un API gateway que funcionará como puerta de enlace y control de acceso, conectando los microservicios al servicio de autenticación y exponiendo sus servicios. 

Los módulos de gestión de proyectos, recursos humanos y finanzas contarán con un balanceador de carga de capa de aplicación dedicado configurado con algoritmo least connection, redirigiendo el tráfico hacia el microservicio con menor cantidad de conexiones activas, logrando una alta disponibilidad frente a una alta demanda. Los servicios correspondientes al módulo de soporte y seguridad no utilizarán balanceadores de carga inicialmente debido a que proveen funcionalidades que no serán utilizadas con demasiada frecuencia. A pesar de esto, se dispone como un servicio en un contenedor para un escalado efectivo en caso de requerir un microservicio. 

42 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

Adicionalmente, se incorpora el uso de un orquestador de contenedores que estará encargado de gestionarlos, permitiendo replicar nuevos contenedores y así mismo los microservicios, esto dependiendo del análisis del tráfico de la red, sesiones activas y demás. 



<!-- Start of picture text -->
.<br>/<br>/F=/J<br>=<br>\ a<br>act<br><!-- End of picture text -->

_Ilustración 19_ 

43 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

7.3.1. Módulos, autenticación y orquestador 

Cada módulo fue diseñado como un conjunto de microservicios junto a un balanceador de carga. De esta manera, se mantendrá una alta disponibilidad dividiendo la carga en dos o más contenedores simultáneamente. Los servicios proveídos serán expuestos por el API Gateway que a su vez hará uso de la autenticación ante una solicitud que requiera autorización. Además, se contará con un orquestador que permitirá gestionar de manera automática el escalado de los microservicios. 

A continuación, se listan los módulos para su visualización junto al apartado de autenticación y orquestación. 



_Ilustración 20_ 

44 





<!-- Start of picture text -->
poe eee eee eee ~ ooo,<br>'H Médulo de recursos humanos ;<br>ZF '<br>H Contenedor API '<br>"H<br>"<br>'<br>1 -———— '<br>H Contenedor API |<br>b<br>7, '<br>'0 Balanceador de Carga '<br>1 1<br>ic Lo '<br>| odee y Contenedor API i'<br>= 0 Oram> Desempeno | 0<br>H<br>'<br>' -———— H<br>H Contenedor API |<br>H<br>Hb<br>H4<br>1<br>b<br>H 1<br>Uo --- eee eee eee eee eee eee eee oo<br><!-- End of picture text -->

_Ilustración 21_ 

45 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
' Médulo de finanzas '<br>' LG '<br>i Contenedor API ;<br>|:<br>:Balanceadorde Carga '<br>01 Sse\ ~——————— ‘<br>1 Contenedor API ‘<br><!-- End of picture text -->

_Ilustración 22_ 



<!-- Start of picture text -->
' Médulo de Seguridad '<br>i Lo ;<br>' Contenedor Control '<br>! de Acesso 4<br><!-- End of picture text -->

_Ilustración 23_ 

46 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
Ca Sn SSS SS<br>' Autenticaci6n '<br>' LY ———y '<br>' Contenedor Contenedor API '<br>Balanceador de Carga '<br>''<br>UC) servicio de =) '<br>''<br>''<br><!-- End of picture text -->

_Ilustración 24_ 



<!-- Start of picture text -->
; Orquestador ;<br>'<br>i LYContenedor 1'<br>' Orquestador '<br>1orquestaci6n de '<br>1 ( contenedores 1<br>;'<br><!-- End of picture text -->

_Ilustración 25_ 

7.4. Help Desk para soporte nivel 1 y 2 

Para proveer los servicios de soporte de nivel 1 y 2 se utilizará un servidor para alojar la aplicación web Help desk y además un servidor exclusivo para el backend. 



<!-- Start of picture text -->
4<br>Spe ewe ;<br>web Help Desk ‘Médulo<br>fal de Soporte<br><!-- End of picture text -->

_Ilustración 26_ 

47 

7.5. Redundancia para alta disponibilidad 



<!-- Start of picture text -->
ZDDIGITALDREAMS<br><!-- End of picture text -->

Además del servidor principal, se tendrá un servidor secundario en caso de que el principal presente algún problema y se caiga. El balanceador de carga de capa de transporte redirigirá el tráfico hacia el servidor secundario si esto ocurre, manteniendo los servicios arriba. 



<!-- Start of picture text -->
|<br>'Redundancia para alta disponibilidad !<br>11<br>1i<br>!<br>1‘del proveedor 1<br>| Jocctp<br>1 se tanapore — !<br>|g<br>S40 1<br>7S 7 ‘Servidor secundario uo !<br>i —— ==<br>1<br>1!<br>Ree ewe ee ew ew ewe ew ewe ew ew ewe ew ew ewe ew ew ew ee ew ew ee ee ee<br><!-- End of picture text -->

_Ilustración 27_ 

7.6. Servidor de base de datos del proveedor 

El servidor de base de datos utilizado por el datacenter será suministrado por el proveedor. Se considera la utilización de una base de datos principal para lectura y escritura y, además, dos bases de datos “hot standby” de solo lectura. Los balanceadores de carga estarán configurados para alta disponibilidad, permitiendo redirigir las peticiones hacía una réplica en caso de que la base de datos principal presente problemas y no esté disponible. En caso de que la base de datos principal esté sobrecargada por tareas en cola, se podrán utilizar las otras réplicas para lectura. 

48 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
| Fa] fy]<br>\ =<br>_ Fr<br>><br>=<br>Fe J]<br><!-- End of picture text -->

_Ilustración 28_ 

7.7. Topología de red de la Obra 

El siguiente diagrama representa la topología de red de las instalaciones del proyecto minero. De manera general, cada proyecto tendrá 3 secciones y 1 datacenter central, con sus respectivos dispositivos que luego serán explicados de manera más detallada. 

49 





<!-- Start of picture text -->
Topologia de red de la<br>obra<br>i Seccién de la obra |<br>: Urovo :<br>:: Handheld ‘TS-2000 H|<br>i | torniquetes |<br>H «> con lector |<br>H RFID!<br>: Wavlink N300 :<br>H punto de aceso {J H<br>H WiFi :<br>H ZKTEKO H<br>|: “Usuarios dispositvedeMB360 :<br>H: asistenciacontrol de H:<br>: TEFLIZ6P-24-250W H<br>| “Usuarios seteh i<br>po" """secci6ndelaobra sf = \X DattacenterLocalObra<br>: TEFII26P-24-250W : ‘TEFLIZ6P-24-250W i ‘Modem |<br>switch : switch Linksys :<br>| Usuarios ui firewall 1<br>Gp) tomiquetes | HPE ProLiant :<br>: RFID hi:: servidorMicroserverGent0 Plusde la :Hi<br>: Wavtink N00 ut obra :<br>H punto de aceso_— [J {iepeeeeeeeeennnennnn USEEOSESESSSSEEEEISEEESSSSEEESSSEEOEINS<br>H wir ZKTEKO | | Secci6n de la obra H<br>H MB360 | H<br>Usuarios dispositive | | i<br>de H TEFLI26P-24-250W H<br>H control | ‘switch Usuarios<br>H: ono asistenciade |||} ::<br>: Tsou hy :<br>: Handheld He i<br>:: @»\ 6 / torniqueteslector RFIDcon<br>H Wavlink N300 i<br>H aceso WIFI A ne<br>: MB360 i<br>Usuarios dspostvo<br>: de :<br>: control H<br>: ge :<br>H Urovo asistencia. |<br>H DTS0U H<br>: Handheld :<br><!-- End of picture text -->

_Ilustración 29_ 

50 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### 7.7.1. Sección de la obra 

Cada sección de la obra tendrá un grupo de usuarios locales (Computadores de escritorio) que serán conectados a un switch **TEF1126P-24-250W** , permitiendo su enrutamiento hacia el punto de acceso **WAVLINK N300.** Los usuarios también podrán conectarse a este punto de acceso a través de Wi-FI. Por otro lado, los dispositivos **HANDHELD UROVO DT50U** con lector RFID **,** el dispositivo de control de asistencia **ZKTECO MB360** y los torniquetes **TS-2000** , también estarán conectados al punto de acceso para enviar la respectiva información al servidor central en la nube. 



<!-- Start of picture text -->
; Secciéndelaobra<br>‘|—<br>:<br>| L_ |= TEF1126P-24-250Wswitch ''<br>' Usuarios ‘<br>' TS-2000 '<br>H torniquetes H<br>| a con lector |<br>' kL RFID '<br>‘ Wavlink N300 '<br>: punto de aceso_—__{J H<br>' WiFi ZKTEKO '<br>'<br>: ; MB360 H<br>Usuarios dispositivo '<br>‘ control '<br>H de H<br>' Urovo asistencia '<br>: DT50U :<br>| Handheld '<br><!-- End of picture text -->

_Ilustración 30_ 

51 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

7.7.2. Datacenter local de la obra 

El Data center local de la obra consta de un servidor principal **HPE PROLIANT MICROSERVER GEN10 PLUS** , sirviendo como controlador para el control de acceso en la obra a partir de los torniquetes **TS-2000** con lector RFID. Además, el datacenter consta de un firewall gestionado por un router **Linksys LRT214** que controla el tráfico de información de entrada y salida de la obra por motivos de seguridad. Finalmente, el módem corresponde al equipo suministrado por el proveedor de internet y estará encargado de conectarse a internet para acceder a los servicios del datacenter central en la nube. 



<!-- Start of picture text -->
po aacenter LocalObra<br>switch Linksys Modem<br>i E firewall<br>: HPEMicroserverProLiant ''<br>:: servidorGen10 Plusde la '<br>H obra<br><!-- End of picture text -->



<!-- Start of picture text -->
Ilustración 31<br><!-- End of picture text -->

7.8. Arquitectura física basada en AWS 

A continuación, se presenta la arquitectura física desde una perspectiva que considera el proveedor de la nube (Amazon Web Services), además de las tecnologías como lenguajes, frameworks, gestores de base de datos, entre otros. Así mismo, se detallan los modelos de los dispositivos físicos y las especificaciones de los servicios a contratar de AWS. También se presentan los recursos destinados a cada máquina utilizada en la nube y la interacción con los dispositivos de las obras, separados por ambiente de producción y QA. 

52 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
; 4 ae<br>g as eee ONE<br>7 7 ‘on wo go 88<br><!-- End of picture text -->

_Ilustración 32_ 

7.8.1. Amazon Route 53 

Todo el sistema relacionado a la empresa de trabajo; ya sea en su versión de aplicación de RR.HH. y Finanzas, aplicación de gestión de proyectos, la aplicación web Help Desk o la aplicación móvil de lectura de RFID, estarán conectadas a Amazon Route 53, el cual es un servicio web de DNS escalable y de alta disponibilidad y que se usará para direccionar el tráfico a los recursos del dominio. Este servicio es compartido por los ambientes de producción y QA. 

53 





<!-- Start of picture text -->
ZKTEKO MB360<br>dlspostivos de contol de asistencia<br>x \<br>HPE ProLiant<br>TS-2000 Se)<br>tomiquetes con lector RFID HPe Protiant<br>Gen10 Plus<br>servi dea bra<br>—<br>Aplicacion<br>escritorio<br>‘gestion<br>‘de<br>proyectos<br>—<br>computador<br>personalFinanzasRRHHy<br>Movil<br>Lectura<br>RFID<br>< ay<br>—_—<br>computadora<br>personal<br>soporte<br>Ilustración 33<br><!-- End of picture text -->

54 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|**Característica**|**Valor**|
|---|---|
|Consultas estándar|1 millón por mes|
|Consultas<br>de<br>direccionamiento<br>basado en la latencia|1 millón por mes|
|Consultas de DNS geográfico|1 millón por mes|
|Consultas de enrutamiento basado en<br>IP|1 millón por mes|
|Número de dominios almacenados|1|
|Consultas de DNS|10 millones por mes|



#### 7.8.2. AWS Amplify 

Se utilizará AWS Amplify para alojar las aplicaciones web de los módulos de recursos humanos, finanzas y soporte y sus contenidos estáticos. Cada aplicación web se implementará con las tecnologías TypeScript y el framework VueJS. 

55 



<!-- Start of picture text -->
DIGITAL<br><!-- End of picture text -->



<!-- Start of picture text -->
=><br><!-- End of picture text -->



<!-- Start of picture text -->
Ilustración 34<br><!-- End of picture text -->



<!-- Start of picture text -->
7.8.2.1. AWS Amplify producción<br><!-- End of picture text -->

Aquí se detallan los costos de AWS Amplify y sus valores en producción. 

|**Característica**||**Valor**|
|---|---|---|
|Datos almacenados al mes|20 GB||
|Datos servidos al mes|200 GB||



_Tabla de recursos asignados al servicio AWS Amplify para aplicación web módulo de RRHH y Finanzas._ 

56 





<!-- Start of picture text -->
Característica  Valor<br>Datos almacenados al mes 10 GB<br>Datos servidos al mes  100 GB<br><!-- End of picture text -->

_Tabla de recursos asignados al servicio AWS Amplify para aplicación web help desk para módulo de soporte._ 

#### _7.8.2.2. AWS Amplify QA_ 

Aquí se detallan las características del servicio de AWS Amplify en QA. 



<!-- Start of picture text -->
Característica  Valor<br>Datos almacenados al mes 5 GB<br>Datos servidos al mes  50 GB<br>OS<br>Tabla de recursos asignados al servicio AWS Amplify para aplicación web help desk para módulo de<br>soporte.<br>Característica  Valor<br>Datos almacenados al mes 5 GB<br>Datos servidos al mes  50 GB<br>a<br>Tabla de recursos asignados al servicio AWS Amplify para aplicación Web Help Desk QA.<br><!-- End of picture text -->

7.8.3. AWS S3 Buckets 

Se utilizará S3 Bucket para el almacenamiento de contenido estático y almacenamiento de archivos para las aplicaciones web de los módulos de recursos humanos y finanzas. 

57 



<!-- Start of picture text -->
ODIGITAL<br><!-- End of picture text -->



<!-- Start of picture text -->
ro ~~ “servidorde rf ~~ “Servidorde<br>! Aplicacién Web ! ! Aplicacion Web Help Desk!<br>I RR.HH y Finanzas 1 ! 1<br>II<br>II I I<br>1I<br>I<br>1 I I [t I<br>VX I I I<br>II AWS Amplify II II AWS Amplify: II<br>1 I Ces eeeeee a|aq7<br>me ee ee ee -_-J<br>as<br>AWS S3 AWS S3<br>Bucket Bucket<br><!-- End of picture text -->

_Ilustración 35_ 

#### _7.8.3.1. AWS S3 Bucket producción_ 

A continuación, se detalla sobre las características del servicio AWS Bucker y su valor correspondiente en producción. 

|**Característica**||**Valor**|
|---|---|---|
|Almacenamiento de S3 Estándar|2 TB por mes||
|Solicitudes PUT, COPY, POST y LIST a S3|100||
|Estándar|||
|Solicitudes GET, SELECT y todas las|100||
|demás desde S3 Estándar|||
|Datos devueltos por S3 Select|3 TB por mes||



_Tabla de recursos asignados al servicio AWS S3 Bucket para aplicación web RR.HH. y Finanzas producción._ 

58 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|**Característica**|**Valor**|
|---|---|
|Almacenamiento de S3 Estándar|32 GB por mes|
|Solicitudes PUT, COPY, POST y LIST a S3<br>Estándar|100|
|Solicitudes GET, SELECT y todas las|100|
|demás desde S3 Estándar||
|Datos devueltos por S3 Select|32 GB por mes|



_Tabla de recursos asignados al servicio AWS S3 Bucket para aplicación web Help Desk para módulo de soporte producción._ 

#### _7.8.3.2. AWS S3 Bucket QA_ 

A continuación, se detalla sobre las características del servicio AWS S3 Bucket y su valor correspondiente en el ambiente QA. 

|**Característica**||**Valor**|
|---|---|---|
|Almacenamiento de S3 Estándar|1 TB por mes||
|Solicitudes PUT, COPY, POST y LIST a S3<br>Estándar|33||
|Solicitudes GET, SELECT y todas las|33||
|demás desde S3 Estándar|||
|Datos devueltos por S3 Select|1 TB por mes||



_Tabla de recursos asignados al servicio AWS S3 Bucket para aplicación web RR.HH y Finanzas QA._ 

59 



|**Característica**|**Valor**|
|---|---|
|Almacenamiento de S3 Estándar|8 GB por mes|
|Solicitudes PUT, COPY, POST y LIST a S3<br>Estándar|33|
|Solicitudes GET, SELECT y todas las|33|
|demás desde S3 Estándar||
|Datos devueltos por S3 Select|16 GB por mes|



_Tabla de recursos asignados al servicio AWS S3 Bucket para aplicación web Help Desk para módulo de soporte QA._ 

#### 7.8.4. Amazon API Gateway 

Se utilizará Amazon API Gateway para el redireccionamiento y protección de las API Rest de los microservicios del sistema. 

_Ilustración 36_ 

60 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

_7.8.4.1. AWS API Gateway producción_ 

A continuación, se detalla sobre las características del servicio AWS API Gateway y su valor correspondiente en producción. 

|**Característica**||**Valor**|
|---|---|---|
|API de HTTP: solicitudes por día|108000||
|API WebSocket: solicitudes por día|15000||



_Tabla de recursos asignados al servicio AWS API Gateway producción._ 

#### _7.8.4.2. AWS API Gateway QA_ 

A continuación, se detalla sobre las características del servicio AWS API Gateway y su valor correspondiente en el ambiente QA. 

|**Característica**||**Valor**|
|---|---|---|
|API de HTTP: solicitudes por día|27000||
|API WebSocket: solicitudes por día|3750||



_Tabla de recursos asignados al servicio AWS API Gateway QA._ 

61 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

#### 7.8.5. AWS Lambda 

Se configurará el API Gateway para que haga uso de la funcionalidad AWS Lambda authorizer, utilizando una función de AWS Lambda para realizar la autenticación y autorización de los usuarios. 

_Ilustración 37_ 

62 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

#### _7.8.5.1. AWS Lambda producción_ 

A continuación, se detalla sobre las características del servicio AWS API Lambda y su valor correspondiente a producción. 

|**Característica**||**Valor**|
|---|---|---|
|Arquitectura|x86||
|Cantidad de solicitudes|4000 por día||
|Duración de cada solicitud (en ms)|1||
|Cantidad de memoria asignada|1000 MB||



_Tabla de recursos asignados al servicio AWS Lambda producción._ 

#### _7.8.5.2. AWS Lambda QA_ 

A continuación, se detalla sobre las características del servicio AWS Lambda y su valor correspondiente en el ambiente QA. 

|**Característica**||**Valor**|
|---|---|---|
|Arquitectura|x86||
|Cantidad de solicitudes|1000 por día||
|Duración de cada solicitud (en ms)|1||
|Cantidad de memoria asignada|250 MB||



_Tabla de recursos asignados al servicio AWS Lambda QA._ 

63 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

#### 7.8.6. AWS DynamoDB 

Se dispondrá de una base de datos en DynamoDB exclusiva para guardar la información referente a los usuarios del sistema. Esta base de datos será utilizada junto a AWS Lambda para realizar la autenticación y autorización. 



<!-- Start of picture text -->
Amazon<br>DynamoDB<br>AWS Lambda<br>Authentication<br>Amazon API Application<br>Gateway oat<br>Balancer<br><!-- End of picture text -->

_Ilustración 38_ 

64 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

_7.8.6.1. AWS DynamoDB producción_ 

A continuación, se detalla sobre las características del servicio AWS DynamoDB producción y su valor correspondiente a producción. 

|**Característica**||**Valor**|
|---|---|---|
|Tamaño<br>del<br>almacenamiento<br>de|16 GB||
|datos|||
|Escrituras no transaccionales|50 %||
|Escrituras transaccionales|50 %||



_Tabla de recursos asignados al servicio AWS DynamoDB producción._ 

#### _7.8.6.2. AWS DynamoDB QA_ 

A continuación se detalla sobre las características del servicio AWS DynamoDB producción y su valor correspondiente en el ambiente QA. 

|**Característica**||**Valor**|
|---|---|---|
|Tamaño<br>del<br>almacenamiento<br>de|4 GB||
|datos|||
|Escrituras no transaccionales|50 %||
|Escrituras transaccionales|50 %||



_Tabla de recursos asignados al servicio AWS DynamoDB QA._ 

#### 7.8.7. Elastic Load Balancing 

Se utilizará Elastic Load Balancing para la distribución automática del tráfico entrante para los distintos servicios que están alojados en el contenedor AWS EC2. En este caso se dispondrá el balanceo de carga solamente para el ambiente de producción. 

65 



_Ilustración 39_ 

|**Característica**||**Valor**|
|---|---|---|
|Número de balanceadores de carga|1||
|de aplicaciones|||
|Bytes procesados (instancias EC2 y|1 GB por hora||
|direcciones IP como objetivos)|||
|Duración promedio de conexión|1 segundo||



_Tabla de recursos asignados al servicio Elastic Load Balancing_ 

66 



7.8.8. Instancia EC2 para servidor de microservicios 

Como se puede observar en la ilustración 39 el contenedor EC2 representa una instancia (entorno virtual informático), la cual tendrá asociada las configuraciones de los _task_ para la asignación de los recursos hardware, cantidad de memoria RAM y número de núcleos CPU, para los módulos de finanzas, recursos humanos y gestión de proyectos. Cada _task_ representa una definición en formato json que describe uno o más contenedores docker, los cuales tendrán el registro de las configuraciones para ejecutar los módulos mencionados anteriormente. Por otra parte, cada servicio representa un microservicio, los cuales se implementarán con las tecnologías Python, framework Django, Redis y Celery para la gestión de tareas asíncronas. 



<!-- Start of picture text -->
MecacontaneR = ———ss—<“—s—sSsSSSSSSSC<br>H1<br>1<br>topenne ----. ----§(@U----.:Q 1<br>iol 4 ' 1 = my<br>mo ECS Task 1 1 ECS Task ro<br>1 Medulo RR.HH j ‘modulo it<br>toy ' Finanzas 1<br>not ' 1 in)<br>io| 1, Setvicio de Servicio-  de ' 1| __ Servicio Servicio 45 |<br>ro Remuneraciones Asistenciay Contabilidad Reporteria<br>iol Turnos 1' '1 m yt<br>ho ' 1 in)<br>11!i 1 EvaluacionServiciodede Serviciode '| '1 myin)1<br>1 1 Desempefio Firma Digital | 1 fn)<br>ftene-------ees eee ees |<br>11<br>1' Q Q 1'<br>roetcst --- 4 eo---f SB----4<br>toomy ECS Taska 1bog' ECS Taska 1!i<br>oy Modulo de i ‘Modulo '<br>' gestion de ' Seguridad mo<br>roa Proyectos ' 1 ot<br>routy UII THIN '' 1 moi<br>st| | Seviciode = Servictode = ' ' [im i!mo<br>ro ‘workflow P ‘Serviciode<br>ro {nventariado 1 identificacion 1}<br>AIM]iolitmy1 Serviciomensajeria de notificaciones(UNServicio de '1|!1 !1'ee----- esm4inni '1<br>roa ' 1<br>11<br>1<br>it ‘Amazon ' 1<br>rot Elasticache ' ‘<br>hoy for Redis 1 1<br>1<br>|te-------eee es<br>11<br>11<br><!-- End of picture text -->

_Ilustración 40_ 

67 



#### _7.8.8.1. AWS EC2 producción_ 

A continuación, se detalla sobre las características del servicio AWS EC2 producción y su valor correspondiente a producción. 

|**Servicio**<br>|**N° de núcleos CPU**<br><br>|**Cantidad de Memoria**<br>|
|---|---|---|
|EC2<br>_Tabla de_<br> <br>|64<br>_recursos para la instancia EC2 d_<br> <br><br>~~ee~~|256<br>_e producción._<br>|
|**Nombre Módulo**|**N° de núcleos CPU**|**Cantidad de Memoria**|
|Módulo RRHH|26|128|
|Módulo de Finanzas|4|16|
|Módulo de Gestión de<br>Proyectos|32|112|
|Módulo de Seguridad|1|1|



_Tabla de recursos asignados para cada servicio ECS Task de producción._ 

#### _7.8.8.2. AWS EC2 QA_ 

A continuación, se detalla sobre las características del servicio AWS EC2 producción y su valor correspondiente a QA. 

**Servicio N° de núcleos CPU Cantidad de Memoria** EC2 16 32 ~~—~~ _Tabla de recursos para la instancia EC2 de QA._ ~~a~~ 

68 



|**Nombre Módulo**|**N° de núcleos CPU**|**Cantidad de Memoria**|
|---|---|---|
|Módulo RRHH|4|8|
|Módulo de Finanzas|2|4|
|Módulo de Gestión de|8|16|
|Proyectos|||
|Módulo de Seguridad|2|4|



_Tabla de recursos asignados para cada servicio ECS Task de QA._ 

#### 7.8.9. Backend web Help Desk (instancia EC2) 

Se dispone una instancia de EC2 como servidor para el backend de la aplicación web Help Desk, que incluye la lógica de negocio de este sistema. A continuación, se detallan las características necesarias para dicho servicio tanto para el ambiente de producción como para el de QA. 



<!-- Start of picture text -->
Virtual Private Cloud<br>ro ~~ “Servidorde ~~ ~ 7<br>'Aplicacion Web Help Desk!<br>iI<br>II<br>fi<br>i i =]<br>|<br>f Def i<br>' ' ‘Amazon EC2,<br>' ‘AWS Amplipity ' backend<br>ae hee Help Desk<br>AWS S3<br><!-- End of picture text -->

_Ilustración 41_ 

69 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

_7.8.9.1. AWS EC2 backend Help Desk producción_ 

A continuación, se detalla sobre las características del servicio AWS EC2 backend Help Desk y su valor correspondiente a producción. 

|**Característica**||**Valor**|
|---|---|---|
|Sistema operativo|Linux||
|N° de núcleos|8||
|Memoria|32 GB||



_Tabla de recursos asignados a instancia EC2 para backend web help desk producción._ 

_7.8.9.2. AWS EC2 backend Help Desk QA_ 

A continuación, se detallan las características y valor del servicio de AWS EC2 backend Help Desk QA y su valor en QA 

|**Característica**||**Valor**|
|---|---|---|
|Sistema operativo|Linux||
|N° de núcleos|4||
|Memoria|16 GB||



_Tabla de recursos asignados a instancia EC2 para backend web help desk QA._ 

#### 7.8.10. Amazon Aurora 

Con respecto al almacenamiento de datos se optó por Amazon Aurora PostgreSQL-Compatible DB, la cual consta de una instancia como base de datos principal, la cual tiene las funciones de lectura y escritura, mientras las dos últimas tiene solo las funciones de lectura. 

70 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
HamazonAuroraDBClusterH == = =  tstSt~CSH<br>H'<br>''<br>''<br>H' po--- n-ne ---4 pore ----4 H<br>1 1! Availability Zone 1! 11 Availability Zone 1! 'i<br>tf11<br>t'i!<br>1! ! 1 1<br>t111<br>H1 1 1 1 '<br>H 1 Principal 1 S51 Replica Replica 1 t<br>'!!<br>H1 w = 1 w o ! H<br>' 1 3 = I I 3 3 ' i<br>i'2s11<br>1<br>' 1a o , | a \ '1<br>H' ' ' ' ' H'<br>roo 1<br>, | 1 ot<br>' 1 Data Copies Data Copies ' '<br>'to1 'of<br>'11'<br>!v------- ees U--------eeeeeee es H<br>' '<br>(on ee eee en eee e eee eeeeee<br><!-- End of picture text -->

_Ilustración 42_ 

|**Característica**||**Valor**|
|---|---|---|
|N° de instancias + réplicas|3||
|N° de núcleos|2||
|Memoria|16 GB||
|Almacenamiento|2 TB||



_Tabla de recursos asignados para cada instancia de Amazon Aurora producción._ 

71 



#### 7.8.11. Amazon ElastiCache 

Para los servicios de mensajería y notificaciones pertenecientes al módulo de gestión de proyectos, es necesario contar con un mecanismo de caché en memoria que permite encolar los mensajes o las notificaciones enviadas y recibidas desde y hacia los websockets configurados en el API Gateway hacia las aplicaciones. A continuación, se detallan las características necesarias para dicho servicio, tanto para producción como para el ambiente de QA. 

_Ilustración 43_ 

72 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

#### _7.8.11.1. AWS ElastiCache producción_ 

A continuación, se detallan las características y valor del servicio de AWS ElastiCache y su valor en producción. 

|**Característica**||**Valor**|
|---|---|---|
|Nodos|2||
|N° de núcleos|4||
|Memoria|12.93 GB||
|Utilización|70%||
|Motor|Redis||



_Tabla de recursos asignados para el servicio de AWS ElastiCache Producción._ 

#### _7.8.11.2. AWS ElastiCache QA_ 

A continuación, se detalla sobre las características del servicio AWS ElastiCache y su valor correspondiente a QA. 

|**Característica**||**Valor**|
|---|---|---|
|Nodos|2||
|N° de núcleos|2||
|Memoria|6.38 GB||
|Utilización|40%||
|Motor|Redis||



_Tabla de recursos asignados para el servicio de AWS ElastiCache QA._ 

73 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

#### 7.8.12. Amazon Elastic Container Registry (Amazon ECR) 

Debido a que se está utilizando una arquitectura basada en microservicios, es necesario poder gestionar y mantener almacenadas las versiones de las imágenes docker correspondientes a cada uno, es por ello por lo que se hace uso de AWS ECR, servicio utilizado por ambos ambientes. A continuación, se especifican las características escogidas para el servicio. 

|**Característica**||**Valor**|
|---|---|---|
|Cantidad de datos almacenados|16 GB por mes||
|Transferencia de datos de entrada|1 TB al mes||
|Transferencia de datos de salida|1 TB al mes||



_Tabla de recursos asignados para el servicio de AWS ECR._ 

74 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 8. Plan de implantación 

A continuación, se detalla de qué manera y cuándo se implementará todo el software en la empresa. 

### 8.1. Provisión de dispositivos e infraestructura 

Primero se realizarán las compras de todas las tecnologías necesarias para poner en marcha la solución, tanto a lo que se refiere como equipamiento de los trabajadores como a implementos físicos necesarios, como, por ejemplo, computadores, lectores RFID, dispositivos de control de asistencia biométricos, servidores, routers, switches, etc. Una vez adquiridos los dispositivos y servicios, se llevará a cabo la distribución del equipamiento hacia las obras mineras, de esto se encargará una empresa externa con experiencia en procesos similares. 

Una vez el equipamiento esté en el lugar de la obra, se procederá a realizar las instalaciones correspondientes para que nuestra solución pueda llevarse a cabo, es decir, se instalarán los servicios eléctricos, servicios de internet y racks de servidores. Una vez terminado esto, estará todo listo para que el sistema inicie su marcha blanca. 

### 8.2. Marcha blanca 

Para la implantación del software primero se considerará una marcha blanca en donde se verá cómo responde el sistema a las solicitudes y a las interacciones del usuario. La idea de esto es ver si a los usuarios finales se les hace muy difícil usar el software, ver si el sistema sufre fallas o si el hardware que compramos no responde de manera correcta. La implantación de la marcha blanca se dividirá según los módulos, primero se implantará el módulo de gestión de proyecto, luego el de RR.HH. y finanzas (simultáneamente), después el módulo de seguridad, y finalmente el módulo de soporte, entonces, cada módulo contará con su propia marcha blanca. 

75 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Estas se llevarán a cabo a medida que los módulos terminen sus etapas de desarrollo, vale decir, una vez terminé de desarrollarse el módulo de gestión de proyectos, se comenzará con su marcha blanca, mientras ocurre esto, se estarán desarrollando los módulos de RRHH y finanzas, para luego iniciar su marcha blanca correspondiente, este proceso se repite para los módulos de seguridad y soporte respectivamente. 

Para el comienzo de la marcha blanca correspondiente al módulo de gestión de proyecto, se le pedirá al cliente que seleccione una de sus obras para ser una especie de sujeto de prueba, en donde se implementará la primera marcha blanca, como participantes de esta, se considerará a todos los usuarios que interactúen directamente con la aplicación de escritorio. Con respecto a los participantes de los otros módulos, el sistema se implementará solo con un 20% de los usuarios que interactúen con el sistema por módulo, es decir, 20% de trabajadores de finanzas, 20% de trabajadores de RRHH, y así sucesivamente. Se le hará entrega del equipo necesario para desarrollar su trabajo y usar el software a todos los empleados seleccionados, independiente del módulo al que pertenezca. 

Para ayudar con el entendimiento del nuevo sistema se desarrollará un manual de usuario, el cual indicará las funcionalidades y el correcto uso de estas dependiendo del tipo de empleado. Este se entregará a todas las personas que vayan a ocupar el sistema en la fecha que inicie cada marcha blanca. 

La marcha blanca durará un total de 20 días por módulo, terminado los primeros 10 días, los usuarios que hicieron uso del sistema, deberán rellenar una encuesta de satisfacción de producto y entregar el equipo que se les facilitó inicialmente. Tras un análisis de los resultados que se obtengan en la encuesta, se contará con otro plazo de 10 días para realizar cambios y últimos refinamientos del sistema del módulo. En el caso de que se encuentre algún fallo crítico, se volverá al análisis de la solución y se reprogramará otra marcha blanca. Una vez finalicen las marchas blancas de todos los módulos, comenzará la puesta en marcha real de la solución. 

76 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

### 8.3. Puesta en marcha 

Al igual que en la marcha blanca, la puesta en marcha “real” se realizará gradualmente. Después de terminar el proceso de marcha blanca de un módulo, se comenzará con la puesta en marcha “real” del software del módulo, mientras esto ocurre, simultáneamente, se inicia la marcha blanca del siguiente módulo, este proceso se repite hasta que todos los módulos estén implementados. Primero se implementará el módulo de gestión de proyectos, luego el de RRHH y finanzas, después el de seguridad y finalmente el de soporte. Se considerarán 10 días para que se ejecuten todos los preparativos para la puesta en marcha “real” de cada módulo (entrega de tarjetas de seguridad en el caso de módulo de seguridad, instalación de software, etc.). 

### 8.4. Capacitaciones 

Se realizarán capacitaciones de cómo usar el software a todos los usuarios finales, esto en paralelo a que se vayan iniciando sus respectivas puestas en marchas reales, capacitaciones que tienen como objetivo enseñar de una manera correcta al usuario a cómo usar la aplicación y no perderse en ella, esto sumado al manual de usuario entregado, será un apoyo considerable para todos los trabajadores con el objetivo de que tengan una grata experiencia al momento de trabajar con nuestro software. Este proceso será realizado por el analista de soporte de la empresa. 

77 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 9. Innovaciones 

En esta sección se revisarán las innovaciones propuestas por nuestra empresa que entregan un valor fundamental a la propuesta realizada. 

- **Módulo de finanzas:** El software a desarrollar cuenta con un módulo de finanzas, para que el mismo personal de la empresa del área pueda hacer uso de este. De esta manera, la digitalización de esta parte de la empresa tendrá una manera ordenada y segura de llevar sus finanzas al día. 

- **Calendario de hitos de la empresa:** El software presentará un calendario que presentará tanto los _deadlines_ o fechas de entrega de cada avance en el proyecto, como también los diferentes eventos que ocurran en la obra, ya sean accidentes, denegaciones o puesta en marcha de cualquier proyecto. También se implementará en el caso de cualquier atraso con los plazos de entrega y fechas importantes. 

- **Sistema de inventariado:** El software contará con un sistema de inventario que permita a los participantes del proyecto gestionar las herramientas y maquinarias de la obra, manteniendo además un historial de los costos de dichos artefactos visible por el jefe de proyecto y jefes de especialidad. 

- **Carga y visualización de seguros:** La falta de una correcta forma de manejar seguros y la digitalización de la información de estos de cada trabajador es una implementación que se llevará a cabo como innovación dentro del módulo de recursos humanos, para así tener una manera más organizada de gestionar estos recursos. Toda la información que esté relacionada a los seguros de cada trabajador se visualizará en una pestaña del módulo de recursos humanos, lo cual el operario de recursos humanos podrá cargar la información relacionada para cada seguro asociado a un trabajador. 

- **Sistema de recopilación de opinión de los trabajadores de forma anónima (encuesta):** El sistema contará con una sección en donde los trabajadores podrán realizar opiniones o realizar sugerencias sobre su experiencia al momento de trabajar en la empresa. Se espera que con estos comentarios la empresa pueda tener claridad necesaria para que tome esos datos y le sean de utilidad para integrarlos a la manera en que se trabaja. 

78 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

# 10. Gestión del riesgo 

A continuación, se presentarán los análisis de riesgos de la solución, los análisis de riesgos de desarrollo y el análisis de riesgos de implantación. Además, se realizarán los análisis cualitativos de estos, finalizando con los planes de acción y respuesta para cada uno de los riesgos identificados. 

### 10.1. Análisis de riesgo de la solución 

Los siguientes riesgos están ligados a la propuesta para dar solución a todos los problemas, cada uno de ellos puede afectar la implementación del sistema. A continuación, la tabla se presenta con un ID de riesgo y su nombre, consideramos dos efectos del riesgo, positivo, que son aquellos riesgos que se pueden explotar para que se mejore el proyecto, mientras que los riesgos negativos son riesgos que pueden afectar a un correcto desarrollo del proyecto. 

|**ID**|**Nombre del riesgo**|**Efecto**|**Descripción**||
|---|---|---|---|---|
|RS-01|Añadir<br>nuevas<br>funcionalidades<br>al<br>sistema.|Positivo|Añadir<br>funcionalidade<br>previstas<br>al<br>sistema<br>hacer más útil al sistema<br>cliente entregando así u<br>producto.|s<br>no<br>puede<br>para el<br>n mejor|
|RS-02|Insuficientes<br>reuniones<br>con<br>el<br>Cliente<br>y<br>Stakeholders.|Negativo|Dado que no se desar<br>suficientes<br>reuniones<br>generan<br>requisitos<br>pulidos, derivando en<br>funcionalidades del siste|rollaron<br>,<br>se<br>poco<br>malas<br>ma.|



79 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RS-03|Mal entendimiento de<br>las<br>jerarquías<br>internas<br>con<br>relación<br>a<br>los<br>actores.|Negativo|Dado que los actores de la<br>solución<br>deben<br>estar<br>claramente jerarquizados para<br>poder distribuir correctamente<br>las<br>responsabilidades<br>y<br>funcionalidades del sistema, un<br>mal entendimiento provocaría<br>pérdidas de tiempo.|
|---|---|---|---|
|RS-04|Incumplimiento<br>de<br>plazos.|Negativo|Dado que el proyecto se realiza<br>entre varias personas y en un<br>periodo<br>de<br>tiempo<br>determinado, si el proyecto no<br>sigue un correcto flujo y no se<br>coordinan todas las partes para<br>cumplir los plazos acordados, el<br>proyecto se puede retrasar.|
|RS-05|Incorrecto<br>análisis<br>de<br>requerimientos.|Negativo|Dado<br>que<br>faltarían<br>requerimientos claves para el<br>desarrollo del sistema se podría<br>volver a fases de análisis de<br>requerimientos, retrasando el<br>proyecto.|
|RS-06|Cambio repentino de<br>requerimientos.|Negativo|Dado que el proyecto tendrá<br>una larga duración, entonces<br>es probable que en algún<br>momento de la elaboración se<br>cambien<br>los<br>requerimientos,<br>teniendo<br>que<br>cambiar<br>la<br>estructura del sistema.|



80 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RS-07|Falla en la distribución<br>Negativo|Dado que la solución se hará|
|---|---|---|
||de<br>responsabilidades|por<br>un<br>gran<br>número<br>de|
||del equipo.|personas, entonces es posible|
|||que los integrantes del equipo|
|||no reciban las tareas que más|
|||se<br>ajustan<br>a<br>su<br>cargo<br>y|
|||especialidad, provocando un|
|||bajo rendimiento en las tareas.|



### 10.2. Análisis de riesgo de desarrollo 

En relación con la implementación de respuestas, existen riesgos operacionales en el desarrollo, como también riesgos técnicos en toda la puesta del sistema. Al igual que en el anexo anterior, se separa entre ID, Nombre del riesgo y sus efectos. 

|**ID**|**Nombre del riesgo**|**Efecto**|**Descripción**|
|---|---|---|---|
|RD-01|Fallas de fábrica en el<br>hardware.|Negativo|Dado que hay que enviar los<br>dispositivos<br>a<br>la<br>faena,<br>entonces, algunos pueden venir<br>con problemas o fallas, y en<br>consecuencia<br>habría<br>que<br>tomar medidas para responder.|
|RD-02|Capacidades<br>de<br>Hardware<br>mal<br>dimensionadas.|Negativo|Dado<br>que<br>se<br>puede<br>sobreestimar o subestimar las<br>necesidades<br>del<br>hardware,<br>concluyendo<br>en<br>gastos<br>mayores si se subestima o gastos<br>imprevistos si se sobrestima.|



81 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-03|No<br>conocer<br>las<br>capacidades<br>tecnológicas del usuario<br>final.|Negativo|Dado que el usuario puede no<br>estar<br>familiarizado<br>con<br>un<br>sistema de este tipo, entonces,<br>pueden llegar más solicitudes<br>de ayuda y mejoras, teniendo<br>como consecuencia un mayor<br>gasto<br>en<br>capacitaciones,<br>manuales de uso y mejoras de<br>usabilidad<br>durante<br>la<br>mantención perfectiva.|
|---|---|---|---|
|RD-04|Estado deteriorado de<br>un documento físico al<br>realizar migración.|Negativo|Dado que al momento de<br>realizar la migración física a<br>digital puede existir uno o más<br>documentos en mal estado,<br>significa la pérdida de datos<br>relevantes<br>en<br>el<br>contexto<br>trabajado,<br>teniendo<br>como<br>consecuencia, la pérdida de<br>integridad de estos mismos.|
|RD-05|Daños al Hardware por<br>transporte a la faena.|Negativo|Dado<br>que<br>los<br>dispositivos<br>electrónicos transportados a la<br>faena pueden sufrir daños en el<br>trayecto (transporte realizado<br>por<br>una<br>empresa<br>externa),<br>existe el caso en que lleguen a<br>la instalación en mal estado o<br>incluso inutilizables.|



82 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-06|Problemas<br>de<br>integración<br>con<br>software externo.|Negativo|Dado que el software externo<br>puede que no se integre como<br>se esperaba al sistema, en<br>consecuencia, se tendrá que<br>aplicar un mayor esfuerzo de lo<br>esperado.|
|---|---|---|---|
|RD-07|Problemas<br>de<br>instalación<br>del<br>Hardware en las obras.|Negativo|Dado que las obras pueden<br>tener problemas de corriente,<br>voltaje, cableado, ventilación<br>y/o espacio puede significar<br>dificultades al momento de<br>realizar las instalaciones del<br>hardware,<br>teniendo<br>por<br>consecuencia el impedimento<br>de la instalación.|
|RD-08|Revisión de Firmware,<br>controladores<br>y<br>actualizaciones para los<br>dispositivos y software.|Positivo|Dado que los dispositivos y<br>software no están en su última<br>versión estable, entonces se<br>deben<br>actualizar,<br>para<br>en<br>consecuencia<br>alcanzar<br>el<br>objetivo<br>de<br>mantener<br>la<br>seguridad de los sistemas y sus<br>funcionalidades al día.|
|RD-09|Atrasos de envío de<br>dispositivos o entrega de<br>Hardware.|Negativo|Dado<br>que<br>cuando<br>los<br>dispositivos<br>y<br>hardware<br>no<br>llegan en los tiempos requeridos<br>por los proveedores, entonces<br>puede provocar retrasos en la<br>implementación.|



83 

10.3. Análisis de riesgo de implantación 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

Estos, al igual que los anexos anteriores cuentan con los mismos contenidos, ID, Nombre del riesgo, efecto y descripción. Aquí se describirán los riesgos que ocurren en la puesta en marcha del proyecto, fase que llamaremos implantación, ya que aquí entrarán todos los que tengan que ver con la implementación del proyecto. 

|**ID**|**Nombre del riesgo**|**Efecto**|**Descripción**|
|---|---|---|---|
|RI-01|No cumplimiento de los<br>tiempos de soporte.|Negativo|Dado que el soporte tiene<br>que cumplir<br>con un tiempo máximo de<br>respuesta<br>ante<br>un<br>inconveniente con el sistema,<br>esto puede implicar multas<br>estipuladas por contrato.|
|RI-02|No disponibilidad del ISP|Negativo|Dado que la disponibilidad<br>del servicio tiene que ser de<br>tiempo completo, una caída<br>eventual del servicio de red<br>afectaría notablemente.|
|RI-03|No disponibilidad de los<br>servicios cloud.|Negativo|Dado que la disponibilidad<br>de la nube se puede ver<br>afectada,<br>entonces<br>el<br>servicio del sistema puede<br>quedar paralizado.|
|RI-04|Fallo en la lectura RFID|Negativo|Dado que no se puede<br>controlar los accesos a las<br>obras<br>por<br>parte<br>de<br>trabajadores o externos, esto<br>afectaría<br>el<br>flujo<br>de<br>los<br>trabajadores en la obra.|



84 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RI-05|Fallo<br>en<br>lectura<br>biométrica|Negativo|Dado que no se puede<br>controlar<br>las<br>entradas<br>y<br>salidas de trabajadores en<br>consecuencia<br>en<br>consecuencia no es posible<br>llevar un registro durante el<br>fallo.|
|---|---|---|---|
|RI-06|Fallo<br>de<br>envío<br>de<br>notificación|Negativo|Dado el error del sistema, si<br>una notificación no llega<br>correctamente<br>a<br>su<br>destinatario, el workflow no se<br>ejecutará<br>correctamente,<br>generando<br>un<br>producto<br>defectuoso.|
|RI-07|Fallos de usabilidad no<br>previstos|Negativo|Dado que puede existir un<br>error de usabilidad en la<br>aplicación,<br>esto<br>puede<br>provocar el descontento del<br>usuario final.|
|RI-08|Pérdida<br>o<br>robo<br>del<br>equipo de trabajador|Negativo|Dado que no se puede<br>eliminar la posibilidad de una<br>sustracción ilegal de equipos,<br>entonces se puede perder<br>información<br>valiosa<br>almacenada<br>en<br>ordenadores de interés.|



85 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

10.4. Análisis cualitativo de riesgos 

A continuación, se presentan los criterios para evaluar el nivel de prioridad de riesgos. 

#### ● Impacto 

En la siguiente tabla se presenta el daño o impacto que posee cada riesgo, esto se representará con un valor numérico del 1 al 5 que irá en dependencia del impacto económico y temporal del riesgo. 

|**Nivel**|**Impacto**|**Valor**|
|---|---|---|
|Despreciable|No existen efectos perceptibles si el<br>riesgo ocurre.|1|
|Menores|Aumentará los costos (dinero/tiempo)<br>en un máximo de un 10%.|2|
|Moderados|Aumentará los costos (dinero/tiempo)<br>en un máximo de un 20%.|3|
|Mayores|Aumentará los costos (dinero/tiempo)<br>entre un 20% y un 40%.|4|
|Catastrófico|Aumentará los costos (dinero/tiempo)<br>más de un 40%.|5|



#### ● Probabilidad 

Se describen 5 niveles de probabilidad de un riesgo, que irán escalando desde improbable hasta casi seguro. 

86 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|**Nivel**|**Probabilidad**|**Valor**|
|---|---|---|
|Improbable|De 1% a 20%.|1|
|Poco probable|De 20 a 40%.|2|
|Probable|De 40 a 60%.|3|
|Muy probable|De 60 a 80%.|4|
|Casi seguro|De 80 a 100%.|5|



#### ● Prioridad 

En base a los dos criterios anteriores se puede construir una tabla de criterios para darle prioridad a los diferentes riesgos que varían desde Baja hasta Muy Alto. 

|**Criterios**|**Improbable**|**Poco**<br>**probable**|**Probable**|**Muy probable**|**Casi**<br>**seguro**|
|---|---|---|---|---|---|
|**Despreciable**|Bajo|Bajo|Bajo|Medio|Medio|
|**Menores**|Bajo|Bajo|Medio|Medio|Alto|
|**Moderados**|Bajo|Medio|Medio|Alto|Alto|
|**Mayores**|Medio|Medio|Alto|Alto|Muy Alto|
|**Catastrófico**|Medio|Alto|Alto|Muy alto|Muy alto|



### 10.5. Evaluación de riesgos 

Finalmente, para evaluar los riesgos y darle prioridad se genera una tabla con su ID, probabilidad, impacto y su exposición que se obtiene multiplicando la probabilidad con el impacto, obteniendo la exposición. Sigue la prioridad dada por la tabla anteriormente nombrada y se justifica explicando la elección de probabilidad y su impacto. 

87 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|**ID**|**Probabilidad**|**Impacto**|**Exposición**|**Prioridad**|**Justificación**|
|---|---|---|---|---|---|
|RS-01|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|El añadir funcionalidades extras al<br>sistema que el equipo considere<br>útiles<br>puede<br>impactar<br>directamente en el desarrollo del<br>software como tal (dependiendo<br>de la funcionalidad), por lo que se<br>considera un impacto mayor.|
|RS-02|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|Se considera que al ser una<br>empresa interesada en el proyecto<br>y consolidada es poco probable<br>que suceda, sin embargo, de no<br>realizarse suficientes reuniones el<br>producto se podría ver seriamente<br>afectado.|
|RS-03|Improbable<br>(1)|Mayores<br>(4)|4|Bajo|Dado que el proyecto contempla<br>el<br>trabajo<br>de<br>profesionales<br>experimentados, la probabilidad<br>de<br>un<br>mal<br>entendimiento<br>y<br>comprensión del proyecto es baja.|
|RS-04|Poco<br>probable<br>(2)|Catastrófico<br>(5)|10|Alto|Todo atraso significa un gran<br>problema<br>que<br>afecta<br>directamente a los costos y plazos<br>estimados,<br>por<br>esta<br>razón, la<br>correcta planeación previa es<br>clave<br>para<br>evitar<br>pérdidas<br>cuantiosas.|
|RS-05|Poco<br>probable<br>(2)|Catastrófico<br>(5)|10|Alto|Un mal análisis de requerimientos<br>impactaría directamente en el<br>trabajo realizado, pudiendo llegar<br>hasta a reiniciar el proyecto. Sin<br>embargo, se considera que es baja<br>la probabilidad debido a que se<br>considera que el equipo de trabajo<br>realiza bien sus funciones.|



88 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RS-06|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|Al ser un proyecto bien definido, se<br>considera que es poco probable<br>que los requerimientos lleguen a<br>cambiar de manera súbita, sin<br>embargo, un pequeño cambio<br>atrasaría al equipo de desarrollo, y<br>por consecuencia, aumentaría el<br>costo de este.|
|---|---|---|---|---|---|
|RS-07|Improbable<br>(1)|Mayores<br>(4)|4|Medio|Es improbable que esto ocurra<br>debido a que el equipo está bien<br>organizado, sin embargo, una falla<br>de este calibre sería un error<br>importante que atrasaría en gran<br>medida el desarrollo debido al<br>replanteo que tendría que hacer.|
|RD-01|Poco<br>probable<br>(2)|Menores<br>(2)|4|Bajo|Considerando que se realizó una<br>investigación sobre qué hardware<br>es el mejor en todo ámbito, se<br>espera que sea poco probable<br>que se presenten fallas de fábrica<br>al trabajar con marcas empresas<br>tecnológicas confiables. Se espera<br>que sean casos puntuales los<br>equipos con problemas por lo que<br>no<br>representaría<br>un<br>mayor<br>impacto.|
|RD-02|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|Si<br>sucede<br>el<br>caso<br>que<br>se<br>sobreestime sería una pérdida de<br>dinero en el caso que no se termine<br>usando, si se subestima se deberán<br>comprar equipos extras.|



89 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-03|Poco<br>probable<br>(2)|Despreciable<br>(1)|2|Bajo|No<br>conocer<br>la<br>capacidad<br>tecnológica<br>del<br>usuario<br>es<br>improbable que ocurra porque se<br>tienen esos datos desde el inicio, sin<br>embargo, en caso de que este<br>punto pase más allá no condiciona<br>un impacto demasiado grande<br>debido a las capacitaciones que<br>se pueden implementar.|
|---|---|---|---|---|---|
|RD-04|Improbable<br>(1)|Menores<br>(2)|2|Bajo|Es poco probable que esté lo<br>suficientemente dañado para no<br>ser entendible para migrar y si es así<br>se asume que es un documento<br>poco importante para la empresa.|
|RD-05|Poco<br>probable<br>(2)|Menores<br>(2)|4|Bajo|Se puede reemplazar el hardware<br>dañado sin mucho problema, pero<br>sí supondrá un retraso más en el<br>tiempo que en el presupuesto.|
|RD-06|Muy probable<br>(4)|Menores<br>(2)|8|Medio|Rara vez la implementación de<br>software funciona por primera vez,<br>sin embargo, con el personal<br>capacitado con el que se cuenta,<br>se puede aminorar los riesgos<br>asociados a este punto.|
|RD-07|Muy probable<br>(4)|Menores<br>(2)|8|Medio|Al<br>momento<br>de<br>instalar<br>el<br>hardware en las obras, debido a la<br>ubicación, se puede considerar<br>probable que se presente algún<br>problema menor, se asume que<br>son<br>problemas<br>que<br>serán<br>relativamente<br>sencillos<br>de<br>solucionar.|



90 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-08|Casi seguro<br>(5)|Menores<br>(2)|10|Alto|El<br>uso<br>de<br>tecnologías<br>con<br>firmwares, controladores o software<br>desactualizado<br>puede<br>causar<br>fallos<br>y/o<br>errores<br>en<br>el<br>funcionamiento de los sistemas,<br>además de agujeros de seguridad.|
|---|---|---|---|---|---|
|RD-09|Poco<br>probable<br>(2)|Menores<br>(2)|4|Bajo|Hoy en día, la logística de los<br>distribuidores es suficientemente<br>eficiente para que los productos no<br>se atrasen. A raíz de esto si se<br>atrasan no serán por tantos días.|
|RI-01|Improbable<br>(1)|Catastrófico<br>(5)|5|Medio|Un<br>incumplimiento<br>en<br>las<br>respuestas del tiempo de soporte<br>es un error grave, sin embargo, se<br>espera que sea poco probable<br>que<br>ocurra,<br>debido<br>a<br>la<br>preparación de este ante las<br>eventualidades.|
|RI-02|Improbable<br>(1)|Menores (2)|2|Bajo|Si bien en la mayoría de los casos,<br>una caída o no disponibilidad de la<br>ISP que provee de conexión a la<br>localidad podría ser catastrófica,<br>se considera que el sistema podrá<br>trabajar de manera offline|
|RI-03|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|A diferencia del caso RI-02, este es<br>un poco más probable que ocurra<br>y tiene más urgencia, debido a que<br>un fallo en la nube sería grave no se<br>tendría ni respaldo de datos ni<br>donde subir información.|
|RI-04|Muy probable<br>(4)|Despreciable<br>(1)|4|Medio|Es muy común que la tarjeta no<br>pase de manera correcta, pero<br>esto no supone una amenaza o<br>impacto demasiado alto mientras<br>que no suponga un aumento en el<br>tiempo de más de 5 minutos.|



91 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RI-05|Improbable<br>(1)|Mayores<br>(4)|4|Medio|A diferencia del torniquete con<br>lector RFID, la lectura biométrica no<br>debería<br>presentar<br>fallos<br>constantes, por lo que un solo fallo<br>requiere una moderada urgencia<br>porque significa un error en el<br>hardware.|
|---|---|---|---|---|---|
|RI-06|Poco<br>probable<br>(2)|Mayores<br>(4)|8|Medio|El fallo de envío de notificación es<br>un riesgo de impacto catastrófico,<br>conlleva el estancamiento de todo<br>el flujo de trabajo lo que podría<br>traer<br>consecuencias<br>como<br>incumplimiento<br>de<br>plazos,<br>no<br>avance de la obra, etc. Sin<br>embargo, se considera que es<br>poco probable que esto ocurra en<br>el software.|
|RI-07|Muy probable<br>(4)|Despreciable<br>(1)|4|Medio|Al trabajar con la metodología de<br>cascada, es probable que el<br>cliente<br>presente<br>algunos<br>descontentos relacionados con la<br>usabilidad, sin embargo, mientras<br>estos sean menores y no dificulten<br>significativamente<br>el<br>uso<br>del<br>software<br>no<br>tendrían<br>mayor<br>impacto.|
|RI-08|Poco<br>probable<br>(2)|Menores<br>(2)|4|Bajo|El sufrir la pérdida o el robo de un<br>equipo<br>puede<br>comprometer<br>información sensible con respecto<br>a los proyectos de la empresa,<br>pero no a su vez perderla. Por ello<br>se debe realizar la respectiva<br>búsqueda mediante el dispositivo<br>de geolocalización que posea,<br>quitando<br>tiempo<br>en<br>ello,<br>y<br>aumentando el costo ya que se<br>debe adquirir un nuevo equipo.|



92 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

### 10.6. Equipo 

A continuación, se detallarán los cargos de la empresa, en conjunto con su descripción y las etapas de las que será partícipe, esto para posteriormente especificar los responsables en el apartado de plan de acción. 

|**Cargo**|**Descripción**|**Etapa**|
|---|---|---|
|Jefe de Proyecto|Encargado de gestionar todo el<br>proyecto y los trabajadores que<br>se encuentren en este.|Todo el proyecto|
|Jefe de análisis y<br>diseño|Encargado<br>de<br>gestionar<br>y<br>administrar el equipo de análisis y<br>diseño, junto a las tareas de este<br>equipo.|Implementación e<br>implantación|
|Analista<br>Diseñador Senior|Se encarga de dar forma e<br>implementar<br>la<br>arquitectura<br>lógica y física del proyecto.|Implementación e<br>implantación|
|Analista<br>Diseñador Junior|Apoya al diseñador senior en sus<br>tareas y labores.|Implementación e<br>implantación|
|Jefe<br>de<br>Desarrollo|Encargado de gestionar todo el<br>personal que trabajará en el<br>desarrollo del software.|Implementación|
|Ingeniero<br>Programador<br>Senior|Encargado<br>para<br>liderar<br>el<br>desarrollo de un módulo de la<br>solución y de guiar el trabajo de<br>los<br>ingenieros<br>programadores<br>junior que lo acompañan.|Implementación|



93 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|Ingeniero<br>Programador<br>Junior|Encargado del desarrollo de un<br>módulo de la solución, creando<br>el código necesario para cumplir<br>con<br>cada<br>una<br>de<br>las<br>funcionalidades requeridas por<br>dicho módulo.|Implementación|
|---|---|---|
|Jefe de UI/UX|Encargado de gestionar a los<br>Diseñadores UI/UX y verificar que<br>su<br>trabajo<br>responda<br>correctamente las necesidades<br>del usuario.|Implantación.|
|Diseñador UI/UX|Encargado de diseñar las vistas<br>del sistema de software.|Implantación.|
|Jefe TIC|Encargado<br>de<br>realizar<br>una<br>correcta<br>instalación<br>del<br>Hardware<br>y<br>Software.<br>Responsable de los técnicos de<br>electricidad,<br>informática<br>y<br>telecomunicaciones y redes.|Implantación.|
|Técnico<br>en<br>telecomunicaci<br>ones y redes|Encargado<br>de<br>realizar<br>una<br>correcta instalación de la parte<br>de telecomunicaciones y redes<br>del sistema.|Implantación.|
|Técnico<br>en<br>electricidad|Encargado<br>de<br>realizar<br>una<br>correcta<br>instalación<br>de<br>la<br>electricidad del sistema.|Implantación.|
|Técnico<br>en<br>informática|Encargado<br>de<br>realizar<br>una<br>correcta instalación del software<br>del sistema.|Implantación.|
|Analista<br>QA<br>Senior|Encargado de realizar y generar<br>los planes de prueba.|Implantación.|



94 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|Analista<br>QA<br>Junior|Se encarga de llevar a cabo los<br>planes de prueba y encontrar<br>errores en los mismos.|Implantación.|
|---|---|---|
|Analista Soporte|Encargado de presentar soporte<br>al cliente, respondiendo dudas y<br>resolviendo problemas.|Operación.|
|Encargado<br>de|Encargado de la seguridad de|Todo el proyecto.|
|Seguridad TI|todos los softwares.||



### 10.7. Plan de acción 

El plan de acción se obtiene analizando cada tipo de riesgo, clasificando según el tipo de acción que se tomará, siendo positivo una acción de respuesta que aprovechará el problema para mejorar el sistema, mientras que un tipo de acción negativa serán respuestas para solucionar el problema como tal. Las acciones de respuesta variarán según el tipo de acción a tomar. A continuación, se presentarán los planes de acción ordenados según exposición. 

|**ID**|**Exposición**|**Tipo de**<br>**acción**|**Acción de**<br>**respuesta**|**Responsable**|
|---|---|---|---|---|
|RS-04|10|Negativo|Mitigar|Jefe de proyecto|
|RS-05|10|Negativo|Mitigar|Jefe de análisis y diseño|
|RI-06|10|Negativo|Mitigar|Ingeniero Programador<br>senior|
|RS-01|8|Positivo|Aceptar|Jefe de proyecto|
|RS-06|8|Negativo|Mitigar|Ingeniero de<br>requerimientos|
|RD-02|8|Negativo|Mitigar|Jefe de tecnologías de la<br>información y la<br>comunicación|



95 



<!-- Start of picture text -->
ODIGITAL<br><!-- End of picture text -->

|RD-03<br>|8<br>|Negativo<br>|Mitigar<br>|Jefe de UI/UX<br>~~e~~|
|---|---|---|---|---|
|RD-07<br><br>~~e~~<br>|8<br><br>~~e~~<br>|Negativo<br><br><br>|Mitigar<br><br>|Jefe TIC<br><br>~~ee~~<br>|
|RD-08<br><br><br>|8<br><br><br>|Positivo<br><br>~~e~~<br>|Favorecer<br><br>|Técnico en informática<br><br>~~ee~~<br>|
|RI-04<br><br>~~e~~|8<br><br>|Negativo<br><br>~~e ~~|Mitigar<br>|Técnico en informática<br><br>~~ee~~|
|RI-07<br>|8<br>|Negativo<br>|Mitigar<br>|Diseñador UI/UX<br>|
|RI-02<br><br>|5<br><br>|Negativo<br><br>|Mitigar<br><br>|Técnico en<br>telecomunicaciones y<br>redes<br>~~e~~<br>|
|RS-03<br><br>~~e~~<br>|4<br><br>~~e~~<br>|Negativo<br><br><br>|Mitigar<br><br><br>|Jefe de análisis y diseño<br><br>~~ee~~<br>|
|RS-07<br><br><br>|4<br><br><br>|Negativo<br><br><br>|Mitigar<br><br><br>|Jefe de proyecto<br><br>~~e~~<br>|
|RD-06<br><br>|4<br><br>|Negativo<br><br>|Mitigar<br><br>|Analista DevOps<br>~~e~~<br>|
|RD-09<br>|4<br>|Negativo<br>|Transferir<br>|Jefe TIC<br>~~e~~|
|RI-01<br><br>|4<br><br>|Negativo<br><br>|Mitigar<br><br>|Analista Soporte<br>~~e~~<br>|
|RI-05<br>|4<br>|Negativo<br>|Mitigar<br>|Técnico en informática<br>|
|RI-08<br>|4<br>|Negativo<br>|Mitigar<br>|Jefe TIC<br>|
|RS-02<br><br>|2<br><br>|Negativo<br> <br>|Mitigar<br> <br>|Jefe de proyecto<br><br>~~e~~|
|RD-01<br><br>|2<br><br>|Negativo<br><br>|Transferir<br><br>~~e~~|Jefe TIC<br><br>~~e~~|
|RD-04<br><br>|2<br><br>|Negativo<br><br>|Aceptar<br><br>|Jefe de proyecto<br><br>~~e~~|
|RD-05<br><br><br>|2<br><br><br>|Negativo<br><br><br>|Transferir<br><br><br>|Jefe TIC<br><br>~~e~~<br>|
|RI-03<br>|2<br>|Negativo<br>|Mitigar<br>|Jefe de análisis y diseño<br>~~e~~|



96 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

### 10.8. Plan de respuesta 

En lo que respecta al plan de respuesta, se explicará mediante una tabla, ordenada por prioridad, con el ID de cada riesgo y se explicará tanto el plan de mitigación, que es la forma de evitar que el riesgo ocurra, como también se su plan de contingencia, que es lo que ocurrirá una vez se del riesgo. 

|**ID**|**Prioridad**|**Plan de Mitigación**|**Plan de Contingencia**|
|---|---|---|---|
|RS-04|Alto|Estimación con margen de<br>error del tiempo de cada<br>actividad y realización de<br>entregables.|Subdividir el área que<br>provoque más problemas<br>entre los grupos que estén<br>más capacitados.|
|RS-05|Alto|Reuniones<br>constantes<br>de<br>toma<br>y<br>aceptación<br>de<br>requerimientos en conjunto<br>con la empresa.|Reunión de emergencia<br>de forma extraordinaria<br>para<br>poder<br>definir<br>correctamente<br>requerimientos<br>deficientes.|
|RD-08|Alto|Estudio las versiones óptimas<br>en cada caso.|Revisión<br>de<br>todos<br>los<br>equipos y software para<br>actualizarlos<br>si<br>es<br>necesario.|
|RS-02|Medio|Calendarizar<br>reuniones<br>periódicas con revisión de<br>documentos,<br>avances<br>y<br>estado del proyecto.|Reunión de emergencia<br>de forma extraordinaria<br>con<br>los<br>ejecutivos<br>y<br>encargados<br>de<br>la<br>empresa.|



97 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RS-06|Medio|Reuniones<br>constantes<br>de<br>toma<br>y<br>aceptación<br>de<br>requerimientos en conjunto<br>con la empresa.|Cláusula del contrato que<br>especifique que tantos<br>cambios<br>se<br>pueden<br>hacer<br>determinados<br>también<br>por<br>una<br>evaluación<br>de<br>este<br>cambio si es factible o no.|
|---|---|---|---|
|RS-07|Medio|Subdivisión en grupos en<br>donde un jefe de grupo<br>divida<br>las<br>tareas<br>con<br>conocimiento<br>de<br>las<br>habilidades del grupo.|Transferencia de tarea a<br>otro<br>participante<br>más<br>capacitado.|
|RD-02|Medio|Estudio de las capacidades<br>del Hardware a adquirir y los<br>usos del software en cargas<br>altas.|En caso de ser necesario,<br>cambiar el hardware a<br>uno que sí cumpla con lo<br>requerido<br>para<br>poder<br>utilizar<br>el<br>software<br>de<br>manera cómoda.|
|RD-06|Medio|Pruebas de integración con<br>los softwares a revisar.|Ver todas las maneras<br>posibles<br>para<br>poder<br>realizar la integración de<br>software<br>externo<br>sin<br>problemas,<br>de<br>no<br>encontrar<br>solución,<br>incorporar al sistema otro<br>software que cumpla una<br>función similar.|



98 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-07|Medio|Estudio de espacio en las<br>faenas y oficinas. Envío de<br>especificaciones<br>técnicas<br>de habitación a la empresa<br>para<br>próximas<br>construcciones.|Personal encargado de ir<br>físicamente<br>al<br>lugar<br>donde se realizarán las<br>instalaciones, para poder<br>dictar un juicio del por<br>qué<br>ocurren<br>los<br>problemas de instalación<br>y su respectiva solución.|
|---|---|---|---|
|RI-01|Medio|Personal<br>del<br>módulo<br>de<br>soporte<br>encargado<br>de<br>responder<br>dentro<br>de<br>un<br>horario establecido.|Intentar<br>contactar<br>lo<br>antes posible al personal<br>del módulo de soporte,<br>de no tener respuesta, el<br>problema lo abordará la<br>empresa directamente.|
|RI-03|Medio|Se realizarán averiguaciones<br>e investigaciones pertinentes<br>para trabajar con el servicio<br>cloud más estable posible.|Realizar un estudio sobre<br>qué tan recurrentes son<br>los<br>inconvenientes<br>relacionados<br>con<br>el<br>servicio cloud con el que<br>se trabaje, en base a ese<br>estudio concluir si es que<br>es necesario optar por<br>otro servicio cloud.|
|RI-04|Medio|Realización de pruebas con<br>las tarjetas RFID y los lectores.|Ingreso con el guardia de<br>seguridad, junto con el rut<br>y<br>otras<br>formas<br>de<br>autentificación<br>como<br>fotos<br>del<br>supuesto<br>trabajador<br>que<br>quiere<br>entrar.|



99 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RI-05|Medio|Pruebas del dispositivo de<br>control de asistencia.|Ingreso con otros recursos<br>como fotos del supuesto y<br>que se ingrese de forma<br>manual la asistencia.|
|---|---|---|---|
|RI-06|Medio|Antes de realizar la entrega,<br>realizar<br>las<br>pruebas<br>correspondientes<br>para<br>corroborar que siempre las<br>notificaciones se entreguen<br>de forma correcta a quienes<br>les tenga que llegar.|Contactar directamente<br>al personal del workflow<br>perteneciente a la etapa<br>en la que se produjo el<br>fallo<br>de<br>envío<br>de<br>notificación.|
|RI-07|Medio|Antes de realizar la entrega<br>final, se pedirá a un usuario<br>final según sea el caso, que<br>use el software y nos de sus<br>impresiones.|Tomando en cuenta las<br>opiniones de los usuarios<br>finales, se evaluará si es<br>necesario,<br>realizar<br>cambios en el software<br>para mejorar los aspectos<br>de usabilidad de este.|
|RS-03|Bajo|Actividades de estudio del<br>negocio junto con directorio<br>de la empresa y jefes de<br>proyecto.|Visita a la empresa para<br>recopilar la información<br>de manera directa.|
|RD-01|Bajo|Se revisarán y se testean<br>los equipos apenas lleguen y<br>se<br>asegura<br>de<br>comprar<br>dispositivos que puedan ser<br>devueltos. Además, se piden<br>los dispositivos con tiempo<br>antes de la utilización de<br>estos por si se pierde tiempo<br>con el reemplazo.|Se<br>devuelven<br>a<br>la<br>empresa por fallas y se<br>esperan los retornos.|



100 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|RD-03|Bajo|Actividades de exploración<br>de usuarios finales y sus<br>habilidades tecnológicas.|Realizar<br>mayores<br>capacitaciones<br>a<br>personal que no haya<br>logrado<br>adaptarse<br>al<br>software.|
|---|---|---|---|
|RD-05|Bajo|Transferencia<br>de<br>responsabilidad a empresa<br>transportista<br>que<br>firme<br>seguro.|Cobro a la empresa por<br>los dispositivos y compra<br>de unos nuevos.|
|RD-09|Bajo|Se pedirán con tiempo los<br>equipos.|Se<br>reclamará<br>con<br>la<br>empresa proveedora por<br>el retraso.|
|RI-02|Bajo|Se<br>trabajará<br>con<br>dos<br>proveedores<br>de<br>internet,<br>uno principal y uno en caso<br>de que el principal falle.|En caso de que los 2<br>proveedores<br>fallen,<br>se<br>cambiará al menos<br>uno de estos.|
|RI-08|Bajo|Los dispositivos contarán con<br>geolocalización para poder<br>ser encontrados de forma<br>rápida en caso de robo o<br>pérdida.|Se hará el seguimiento<br>correspondiente de el o<br>los dispositivos perdidos o<br>robados,<br>hasta<br>recuperarlos.|



101 



<!-- Start of picture text -->
DDIGITALDREAMS<br><!-- End of picture text -->

# 11. EDT 

El propósito de la presente sección es exponer las etapas y subetapas en base a los entregables y trabajos que se implementarán para el desarrollo del sistema, por lo cual la elaboración del EDT es la base para la planificación del cronograma del proyecto. En base a la ilustración 43, se puede observar la estructura global del EDT, la cual considera 7 grandes etapas. 



<!-- Start of picture text -->
- =<br>“| FE FL - b=] =]<br>[a Ea=) SL| RS= Fa]SE[=a]<br>Ce] ) [es el ey) el<br>fe=  =|=)| | He=) SyBe) [“escras”es|<br>| _ Ee P|<br>=| =]<br>ial ka<br>[aa] =]<br>P|<br><!-- End of picture text -->

_Ilustración 44_ 

11.1. Diccionario de EDT 

Para tener un mejor entendimiento del EDT encontrado en el anexo, se genera un diccionario que contará con la explicación de cada tabla en donde se dará una descripción de lo que contiene, su criterio de aceptación, sus entregables y los supuestos, como también los hitos que contendrán. 

102 



**ID # 1.1 Cuenta Control # 1 Descripción:** Administración del proyecto, explicación de cómo se trabajará y sus documentos. ~~<u>a</u>~~ **ID # 1.1.1 Cuenta Control # 1.1 Descripción:** Se realizan los estudios acordes para definir como tal el alcance del proyecto. ~~<u>a</u>~~ **ID # 1.1.1.1 Cuenta Control # 1.1 Descripción:** Se analiza de manera cualitativa y cuantitativa los factores de riesgo. ~~<u>a</u>~~ **ID # 1.1.1.2 Cuenta Control # 1.1 Descripción:** Se especifica la exposición, tipo de acción, acción de respuesta y responsable de cada factor de riesgo. ~~<u>a</u>~~ **ID # 1.1.1.3 Cuenta Control # 1.1 Descripción:** Se especifica prioridad, plan Mitigación y plan de Contingencia de los riesgos. ~~—~~ 

103 



#### **ID # 1.1.2 Cuenta Control # 1.1 Descripción:** Se realizará la EDT y la carta gantt. 

**ID # 1.1.2.1 Cuenta Control # 1.1 Descripción:** Se escriben los sucesos a superar en el proyecto con fecha estimada. ~~<u>a</u>~~ **ID # 1.1.3 Cuenta Control # 1.1 Descripción:** Se identifican los requisitos, riesgos, casos de prueba y entornos de prueba que hay que probar. ~~<u><mark>———</mark></u>~~ **ID # 1.1.4 Cuenta Control # 1.1 Descripción:** Se definen los procesos por los cuales las empresas planifican, organizan y administran las tareas y activos relacionados con las personas que conforman la organización. ~~<u>—</u>~~ **ID # 1.1.5 Cuenta Control # 1.1 Descripción:** realizar seguimiento de los procesos mediante programas, herramientas o técnicas con el objetivo de mejorar la calidad del producto o servicio. ~~a~~ ~~<u><mark>_</mark></u>~~ 

104 



**ID # 1.1.6 Cuenta Control # 1.1 Descripción:** realizar estudios sobre la rentabilidad con la que cuenta el proyecto. ~~<u>a</u>~~ **ID # 1.1.7 Cuenta Control # 1.1 Descripción:** realizar registros de los ingresos y gastos de la empresa. ~~<u><mark>———</mark></u>~~ **ID # 1.2 Cuenta Control # 1 Descripción:** Se realizan todos los estudios pertinentes respecto a los requerimientos funcionales y no funcionales de todo el proyecto. ~~<u>a</u>~~ **ID # 1.2.1 Cuenta Control # 1.2 Descripción:** Se realizan los estudios acordes para definir como tal el alcance del proyecto, se deja un documento como registro de esto. ~~<u><mark>———</mark></u>~~ **ID # 1.2.2 Cuenta Control # 1.2 Descripción:** Se tiene una reseña de las reuniones con el cliente. ~~<u>—d</u>~~ **ID # 1.2.3 Cuenta Control # 1.2 Descripción:** Se tiene un documento con todos los requerimientos funcionales bien especificados y explicados cada uno. ~~——~~ 

105 



**ID # 1.2.4 Cuenta Control # 1.2 Descripción:** Se tiene un documento con todos los requerimientos no funcionales bien especificados y explicados cada uno. **ID # 1.3 Cuenta Control # 1 Descripción:** Creación de diagramas e informes de diseño. ~~<u><mark>———</mark></u>~~ **ID # 1.3.1 Cuenta Control # 1.3 Descripción:** Arquitectura de la solución, aquí se ven tanto las arquitecturas lógica y física como la topología de la red. ~~<u>a</u>~~ **ID # 1.3.1.1 Cuenta Control # 1.3 Descripción:** Arquitectura física, documento que describe cómo se estructura la arquitectura física del sistema en forma de diagrama. Esta cuenta con las diferentes capas del sistema. ~~<u>—</u>~~ **ID # 1.3.1.2 Cuenta Control # 1.3 Descripción:** Arquitectura lógica, documento que describe cómo se estructura la arquitectura lógica del sistema en forma de diagrama. Esta cuenta con la estructuración de las instalaciones y el servidor del proveedor. ~~a.~~ 

106 



**ID # 1.3.1.3 Cuenta Control # 1.3 Descripción:** Topología de la red, documento que describe cómo se estructura la topología de la red en forma de diagrama. **ID # 1.3.2 Cuenta Control # 1.3 Descripción:** Diseño de base de datos, aquí se diagrama y se explica cómo estará estructurada la base de datos a utilizar. ~~<u>a</u>~~ **ID # 1.3.3 Cuenta Control # 1.3 Descripción:** En el diseño de la interfaz del usuario se verá todo lo que tenga que ver con las interfaces a utilizar. ~~<u>a</u>~~ **ID # 1.3.3.1 Cuenta Control # 1.3 Descripción:** Diseño de aplicación de escritorio, aquí se integrarán las vistas necesarias para dicha aplicación con sus funcionalidades. En la aplicación se encuentra todo el proceso por el que pasa una obra, desde la adquisición de terreno hasta la finalización de esta. ~~a~~ 

107 



#### **ID # 1.3.3.2** 

#### **Cuenta Control # 1.3** 

**Descripción:** Diseño de aplicación web de recursos humanos y finanzas, aquí se integrarán las vistas necesarias para dicha aplicación con sus funcionalidades. La función en el software de los trabajadores de RR.HH. será subir los documentos relacionados a las categorías mencionadas anteriormente y la función de los trabajadores de finanzas es subir los documentos necesarios que tengan que ver con el área. **ID # 1.3.3.3 Cuenta Control # 1.3 Descripción:** Diseño de aplicación web Help Desk, aquí se integrarán las vistas necesarias para dicha aplicación con sus funcionalidades. En la aplicación se encuentran las funcionalidades del módulo de soporte. ~~<u>a</u>~~ 

**ID # 1.3.3.4 Cuenta Control # 1.3** 

**Descripción:** Diseño de la aplicación móvil, aquí se integrarán las vistas necesarias para dicha aplicación con sus funcionalidades. Dentro del sistema de seguridad, encontramos la existencia de una tarjeta de identificación física, la cual indicará claramente el rol que alguien desempeña en el lugar de trabajo (proveedor, trabajador de la faena, etc.). Cada trabajador de la empresa perteneciente a cualquier área y/o módulo y empleado de algún proveedor contará sí o sí con este elemento. Así también, quién deja registro en el software de todo el personal que entra al área de trabajo es el trabajador de seguridad. 

108 



**ID # 1.4 Cuenta Control # 1 Descripción:** Desarrollo del sistema de software, aquí entra el desarrollo y puesta en marcha de todos los microservicios asociados como también la implementación de la base de datos. ~~<u>a</u>~~ **ID # 1.4.1 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla y da forma a todos los microservicios vinculados con el sistema de software y cada uno de sus módulos. ~~<u><mark>———</mark></u>~~ **ID # 1.4.1.1 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla el microservicio del módulo de gestión de proyectos. ~~<u><mark>———</mark></u>~~ **ID # 1.4.1.2 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla el microservicio del módulo de RR.HH. ~~<u><mark>———</mark></u>~~ **ID # 1.4.1.3 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla el microservicio del módulo de seguridad. ~~—~~ 

109 



**ID # 1.4.1.4 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla el microservicio del módulo de finanzas. ~~<u><mark>———</mark></u>~~ **ID # 1.4.1.5 Cuenta Control # 1.4 Descripción:** En esta etapa se desarrolla el microservicio del módulo de soporte. ~~<u>a</u>~~ **ID # 1.4.2 Cuenta Control # 1.4 Descripción:** Se desarrollarán las interfaces previamente diseñadas. ~~<u><mark>———</mark></u>~~ **ID # 1.4.2.1 Cuenta Control # 1.4 Descripción:** Se desarrollarán las interfaces previamente diseñadas para el módulo de gestión de proyecto y de inventariado enfocado para aplicación de escritorio. ~~<u>—</u>~~ **ID # 1.4.2.2 Cuenta Control # 1.4 Descripción:** Se desarrollarán las interfaces previamente diseñadas para el módulo de gestión de recursos humanos y el módulo de finanzas enfocado para aplicación web. ~~—~~ 

110 



#### **ID # 1.4.2.3 Cuenta Control # 1.4** 

**Descripción:** Se desarrollarán las interfaces previamente diseñadas para el módulo de soporte enfocado para aplicación web. **ID # 1.4.2.4 Cuenta Control # 1.4 Descripción:** Se desarrollarán las interfaces previamente diseñadas para el módulo de seguridad enfocado para la aplicación de web. ~~<u><mark>———</mark></u>~~ 

**ID # 1.4.3 Cuenta Control # 1.4** 

**Descripción:** En esta fase se llevará a cabo la implementación de la base de datos central en el software, se evaluará el correcto funcionamiento y que los datos se estén guardando correctamente, así también la correcta sincronización de las bases de datos locales generadas offline con la central. **ID # 1.5 Cuenta Control # 1 Descripción:** Se testea y prueba la efectividad de respuesta a las solicitudes por parte del software. ~~<u><mark>———</mark></u>~~ **ID # 1.5.1 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas de que cada procedimiento de manera independiente cumpla con lo planificado. ~~——~~ 

111 



**ID # 1.5.2 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas de que la solución cumpla con los requerimientos y necesidades. ~~<u>a</u>~~ **ID # 1.5.3 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas de que cada función realiza lo diseñado. ~~<u>a</u>~~ **ID # 1.5.4 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas de que las funciones de manera conjunta cumplan con lo planificado. ~~<u><mark>———</mark></u>~~ **ID # 1.5.5 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas para ver si la seguridad de la solución cumple con lo acordado. ~~<u>a</u>~~ **ID # 1.5.6 Cuenta Control # 1.5 Descripción:** Se realizarán pruebas para ver si la solución cumple con un nivel de usabilidad acorde al ambiente. ~~—~~ 

112 



**ID # 1.6 Cuenta Control # 1 Descripción:** Se realizarán todas las tareas correspondientes para que la solución desarrollada pueda empezar a utilizarse. ~~<u>a</u>~~ **ID # 1.6.1 Cuenta Control # 1.6 Descripción:** Se hace la entrega de todo el equipo necesario. ~~<u><mark>———</mark></u>~~ **ID # 1.6.1.1 Cuenta Control # 1.6 Descripción:** Se estimará cuánto se gastará en el equipamiento. ~~<u><mark>———</mark></u>~~ **ID # 1.6.1.2 Cuenta Control # 1.6 Descripción:** Se realizará registro de las compras realizadas. ~~<u><mark>————</mark></u>~~ **ID # 1.6.1.3 Cuenta Control # 1.6 Descripción:** Se realizará control de la distribución del equipamiento. ~~<u><mark>———</mark></u>~~ **ID # 1.6.2 Cuenta Control # 1.6 Descripción:** Provisión de infraestructura, se informa acerca de las cotizaciones y construcción acerca de la infraestructura. ~~<mark>———?</mark>~~ 

113 



#### **ID # 1.6.2.1 Cuenta Control # 1.6** 

**Descripción:** Se realizarán estimaciones de los gastos enfocados en la infraestructura. **ID # 1.6.2.2 Cuenta Control # 1.6 Descripción:** Se realizarán informes de la supervisión de la construcción. ~~<u><mark>———</mark></u>~~ 

**ID # 1.6.3 Cuenta Control # 1.6** 

**Descripción:** Plan de Marcha blanca. Por cada módulo del sistema se realizará una marcha blanca para ir probando los sistemas, darle familiaridad a los clientes y detectar si es que aparecen problemas. Para una marcha blanca se utilizará una selección de alrededor de un 20% de los usuarios finales. **ID # 1.6.3.1 Cuenta Control # 1.6 Descripción:** Se seleccionará un grupo de individuos para realizar pruebas en el módulo de gestión de proyectos. ~~<u><mark>————</mark></u>~~ **ID # 1.6.3.2 Cuenta Control # 1.6 Descripción:** Se seleccionará un grupo de individuos para realizar pruebas en el módulo de gestión de finanzas. ~~<mark>——_—</mark>~~ 

114 



**ID # 1.6.3.3 Cuenta Control # 1.6 Descripción:** Se seleccionará un grupo de individuos para realizar pruebas en el módulo de RR.HH. **ID # 1.6.3.4 Cuenta Control # 1.6 Descripción:** Se seleccionará un grupo de individuos para realizar pruebas en el módulo de seguridad. ~~<u>a</u>~~ **ID # 1.6.3.5 Cuenta Control # 1.6 Descripción:** Se seleccionará un grupo de individuos para realizar pruebas en el módulo de soporte. ~~<u>a</u>~~ **ID # 1.6.4 Cuenta Control # 1.6 Descripción:** Plan de puesta en marcha, se basa que al terminar una marcha blanca exitosa se comienza a utilizar los sistemas para todos los usuarios, trabajando de forma gradual hasta llegar un 100% de los usuarios objetivos. ~~<u>a</u>~~ **ID # 1.6.4.1 Cuenta Control # 1.6 Descripción:** Se trabajará de forma gradual para que el 100% de los usuarios utilicen el módulo de gestión de proyectos. ~~<mark>——-</mark>~~ 

115 



**ID # 1.6.4.2 Cuenta Control # 1.6 Descripción:** Se trabajará de forma gradual para que el 100% de los usuarios utilicen el módulo de finanzas. ~~<u>a</u>~~ **ID # 1.6.4.3 Cuenta Control # 1.6 Descripción:** Se trabajará de forma gradual para que el 100% de los usuarios utilicen el módulo de RR.HH.. ~~<u><mark>———</mark></u>~~ **ID # 1.6.4.4 Cuenta Control # 1.6 Descripción:** Se trabajará de forma gradual para que el 100% de los usuarios utilicen el módulo de seguridad. ~~<u><mark>———</mark></u>~~ **ID # 1.6.4.5 Cuenta Control # 1.6 Descripción:** Se trabajará de forma gradual para que el 100% de los usuarios utilicen el módulo de soporte. ~~<u>a</u>~~ **ID # 1.6.5 Cuenta Control # 1.6 Descripción:** Se realizarán medidas para que los nuevos usuarios aprendan a utilizar y se familiaricen con el nuevo sistema, las cuales tienen que estar debidamente documentadas. ~~—~~ 

116 



**ID # 1.6.5.1 Cuenta Control # 1.6 Descripción:** Se realiza la inducción a los usuarios respectivos. ~~<u>a</u>~~ **ID # 1.6.5.2 Cuenta Control # 1.6 Descripción:** Se creará y entregará al cliente un manual que indique detalladamente como usar el software desde la perspectiva de un usuario. ~~<u>a</u>~~ **ID # 1.7 Cuenta Control # 1 Descripción:** Registro para la gestión y apoyo de los clientes, y la metodología adoptada para las mantenciones. ~~<u>oo</u>~~ **ID # 1.7.1 Cuenta Control # 1.7 Descripción:** Se observarán y corregirán defectos en los dispositivos entregados e instalaciones en caso de ser necesario. ~~<u>a</u>~~ **ID # 1.7.2 Cuenta Control # 1.7 Descripción:** El software se adaptará a ciertos cambios de ser necesario, esto para para hacer frente a los cambios ocurridos en el entorno (cambios en las condiciones e influencias que actúan desde el exterior). ~~—~~ 

117 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

**ID # 1.7.3 Cuenta Control # 1.7** 

**Descripción:** Se desarrollará un soporte para que en caso de cualquier duda o problema que tenga el cliente, pueda contactarse con la empresa para encontrar una solución. 

|**ID # 1.7.4**<br>**Cuenta Control # 1.7**|
|---|



**Descripción:** Se crearán las primeras cuentas dentro del software. 

118 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# 12. Planificación del proyecto 

En la siguiente sección se presentará toda la planificación realizada para este proyecto. Esto con el fin de contextualizar el orden y temporalidad de las tareas a realizar que implican tanto a la empresa minera como a Digital Dreams. Primero se presentarán los hitos de la empresa y luego se presentará la carta gantt. 

### 12.1. Hitos 

A continuación, se presentarán los hitos del proyecto estipulados en la planificación. 

#### ● **Entrega de documentos de requerimientos y alcance** 

Este hito hace referencia al momento en el que todos los documentos relacionados a los requerimientos se encuentren finalizados, entregados y aceptados y a la definición del alcance del proyecto. Este se llevará a cabo el 26/07/2022. 

#### ● **Entrega de documento de riesgos y plan de calidad** 

En este hito se hace la entrega de toda la información en base al estudio de riesgos y de documentos respectivos sobre el control de calidad del producto, en donde todos los documentos respectivos han sido aprobados para su entrega. Este se llevará a cabo el 05/08/2022. 

#### ● **Diseño de interfaces entregado** 

Este hito hace referencias al momento en que se terminan de diseñar las interfaces de la aplicación de escritorio, la aplicación web, la aplicación móvil y la aplicación web Help Desk. Este se llevará a cabo el 17/03/2023. 

#### ● **Entrega de desarrollo** 

Este hito hace referencia a cuando se terminan las entregas del desarrollo del sistema de software, es decir, las aplicaciones y los módulos requeridos. Este se llevará a cabo el 06/06/2023. 

119 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

#### ● **Entrega de resultados de pruebas** 

Hace referencia a las pruebas y aprobaciones que validan el correcto funcionamiento del software en todos sus aspectos. Este se llevará a cabo el 06/06/2023. 

#### ● **Fin del primer año** 

Este hito hace referencia a la finalización del desarrollo del sistema completo, la provisión del equipamiento y plataformas y el inicio de la etapa de proveer la infraestructura y etapa de mantención. Este se llevará a cabo el 03/07/2023. 

### 12.2. Carta Gantt 

En este apartado se presentará la carta Gantt en su versión tanto expandida como en todas sus demás versiones. La carta Gantt abarca desde el inicio del proyecto en julio del 2022 hasta junio del 2025. Se expande en cada uno de los procesos del producto para dar una vista más detallada de las fechas y sus componentes. 

#### 12.2.1. Carta Gantt expandida 

En esta imagen se ve toda la Carta Gantt expandida, se aprecian a grandes rasgos los trabajos, sus relaciones y sus hitos. Esta imagen tiene como objetivo dimensionar la escala de todo el proyecto. Además, existen unas relaciones que no se logra ver en las otras imágenes ya que se encuentran en dos tareas principales. Esta es que al terminar el desarrollo de cada módulo se inicia la marcha blanca de este módulo en particular. 

120 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



_Ilustración 45_ 

12.2.2. Carta Gantt general sin expandir 

En la ilustración 46 se aprecian las relaciones en las tareas principales. La primera es que no se puede iniciar el diseño del sistema de software sin terminar los Requerimientos de Producto. La siguiente relación indica que el desarrollo del sistema de software va a terminar en conjunto con las pruebas del sistema. 



_Ilustración 46_ 

121 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

12.2.3. Carta Gantt con Requerimientos de Producto expandido 

En la tarea Requerimientos de Producto se estipulan veinte días para realizar un refinamiento de los requisitos y el alcance de la solución. Los procesos son cortos ya que se presentaron los requerimientos y solo se van a mejorar. 



<!-- Start of picture text -->
Nombrede tarea Fecha de inicio Fecha final Duracién Jon rT] Tao<br>01-07-2022 0... 03-07-20251... 785d —<br>1 © Total estimate 01-07-2022 0... 03-07-2025 1... 785d ‘Total estipate 101-07<br>11 © _Requerimientosde Producto 01-07-2022 0... 28-07-2022 1... 204 Requerimientos de P<br>aaa Capiura de nuevos requerimientos 01-07-2022... 14-07-2022... 10d<br>112 Refinacion de documento<br>113 de requerimientos f... 1507-20220... 21-07-2022 1... 5d ‘a<br>Refinacion de doctimento de requerimientosn... 15-07-2020... 21-07-20221... 5d<br>114 Definicion del alcance del proyecto 22-07-20220... 28-07-2022 1... 8d<br>115 Entregadedocumentosde requerimientos y a... 26-07-2220... 26-07-2020...<br>12 Administracién de proyecto 21-07-2022 0... 05-08-2022 0... ud inistracié<br>13 Disefio del sistema de software 29-07-2022 0... 16-03-20230... 164d PPtselio del<br>14 Desarrollo del sistema de software 01-08-2022 0... 01-06-20230... 218d Desarrolic<br>15 Pruebas del sistema 06-10-2022 0... 01-06-2023 0... 170d<br>16 Implantacion 03-10-2022 0... 12-07-20231... 203d<br>17 Fin del primer afto 03-07-2020... 03-07-20230...<br>18 Mantencion 03-07-2023 0... 03-07-2021... 524d<br><!-- End of picture text -->

_Ilustración 47_ 

12.2.4. Carta Gantt con Administración de proyecto expandido 

Al igual que el punto anterior, al tener los riesgos ya estipulados antes del inicio del proyecto se realizarán pequeñas modificaciones y refinamientos solo si son necesarios. Además, se realizará el plan de pruebas y el plan de control de calidad simultáneamente. Esta tarea finaliza entregando el documento de riesgos y los planes. 

122 





<!-- Start of picture text -->
Nombre de tarea Fecha de inicio Fecha final Duracién } rn Tor re<br>01-07-2020... 03-07-20251... 785d ed<br>1 &) Total estimate 01-07-20220... 03-07-2025 1... 785d Total estimate| 01-07-<br>11 Requerimientos de Producto 01-07-20220... 28-07-2022 1... 20d Requerimientosde Pr:<br>12 ©) Administracionde proyecto 21-07-20220... 05-08-20220... ud inistracior<br>121 Refinacion de Riesgos 21-07-2020... 27-07-2022 1... 5d<br>122 Plan de control de calidad 21-07-2020... 03-08-2022 1... tod<br>123 Plan de pruebas, 22-07-2020... 04-08-20221... tod<br>124 Entrega de documento de riesgosy plan de cal... 05-08-20220... 05-08-20220...<br>13 Disefio del sistema de software 29-07-20220... 16-03-20230... 1644 Disefiodel<br>14 Desarrollo<br>del sistemade software 01-08-20220... 01-06-20230... 218d Desarrolig<br>15 Pruebas del sistema 06-10-20220... 01-06-20230... 170d<br>16 Implantacion 03-10-20220... 12-07-2023 1... 203d<br>7 Fin del primer afo 03-07-20230... 03-07-20230...<br>18 Mantencion 03-07-20230... 03-07-20251... 524d<br><!-- End of picture text -->

_Ilustración 48_ 

12.2.5. Carta Gantt con Diseño del sistema de software expandido 

Al igual que los dos puntos anteriores, se aprecian pequeños refinamientos en las arquitecturas, luego de un diseño de la base de datos. Lo que toma más tiempo es el diseño gráfico de las interfaces de usuario módulos en donde el equipo de diseño UI/UX se encargará trabajando en dos módulos simultáneamente.  Esta tarea principal termina con el diseño de interfaces entregados. 



<!-- Start of picture text -->
cvoraene.. moran. Te ——<br>2B ames cvoraem0.. moras. Te Tet entiata 01.7.2 2805<br>11 Requtinienos  oa crane. moran. — 2 RegerininicseProtatesoioraa woraea=~—~*~S<br>12 Admin<br>de proyscte aamne.. wouaae. ud con Ge proyca 237.222- 008.222<br>12 Dla star de sotare morzene. worse. ss Deh dsm ese 357-222-16032023<br>waia ooDn ba sos coosmaze..Barconoszeet.. "i108 | Lee=<br>waa Doe erga gee momo. nome. G<br>be mtn ran a oh<br>1a Dea ce poga re cemmn0, imei. a og<br>123 Diatotrces<br>deuaio cimame. seize. une Diet macs de ure 01.08-222- 35032023<br>1221 Beato deapeacon et evonsen0. caizze21. 908 Dastoceapiaconme ooeaezoisae<br>raat ean oer omanoe emmne, wom. 49 ==<br>waa ead raeas comme, ez. 4 a<br>1222)aaazi Datouadeapeacon6 gesin geproyectos seta cvonsen0..ovoeaez0.. seszz021.163220221.. 10081008 [Dao———woawete splcahn pesonceporcos de nero 008- 02‘i-3612.022<br>1232 Bio deapensionmt ceumne. maze. a a penclonmov 042202-2.012008<br>ast nea geseen cezeme, raze, 1<br>1224 Dato deapeaconmebhap<br>desk ——aanamRze.. ssonmaa1.. 6d Dee de aptcacln web lp ek 30122022 15052028,<br>1341 oat go spat roizz0z20.. 150320031...<br>1s Det ete ep reso, 1eonmso L}®<br><!-- End of picture text -->

_Ilustración 49_ 

123 

12.2.6. Carta Gantt con Desarrollo del sistema de software expandido 



En la ilustración 50 se presentan los desarrollos del sistema de software. La metodología serán 4 grupos de ingenieros desarrolladores que se dividen en partes iguales entre la creación de microservicios y la creación de las vistas de las aplicaciones. 



<!-- Start of picture text -->
—— =| ——————<br>—- evs csraems. ra) 3-00 8<br>rn cenmae. marae. we| [RepeatPenns oleae<br>8 nealigeree noma omy a or in<br>a8 cage gerne meane wegetly wu Ponts ieeer ne pg ssn<br>raeebnctige<br>re comme. ewig Rage ‘inl Ogg ocean]<br>7 ———sa7- SaaS Se a ——<br>1s Desoto deacon web np dost cmosas0.. S105. sod prea apcaconweb]<br>Los baamdenenensemiasesp, onda. atest ws<br><!-- End of picture text -->

_Ilustración 50_ 

12.2.7. Carta Gantt con Pruebas del sistema expandido 

En la ilustración 51 se presentan las pruebas que se realizarán. Estas se realizan a la par que el desarrollo del sistema de software para tener cerciorarse de que todo lo realizado cumpla con las calidades de funcionalidad, seguridad, usabilidad y aceptación. Todas terminan cuando el desarrollo termina. 



<!-- Start of picture text -->
— = ————— OO<br>oo ee<br>a Ear iaraaae. menaeai. a) Remini<br>Pe OTE OTE<br>12La omaoe pagese mercene. werane wae cn<br>cman comer meetin yet erat atone oe CERO<br>1G mene cena wee’, rr<br>1s pn cesos0. steams. 4 _<br>552 tpn iomme, neimm1. ver<br>137 wae. wane. ww<br>a eeas0, stosae as =<br>sate ouosa0. aioe lo<br><!-- End of picture text -->

_Ilustración 51_ 

124 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->

12.2.8. Carta Gantt con Implantación expandido 

En la ilustración 52 se presenta el plan de implantación, el cual parte con la compra de todos los productos necesarios, luego de esto se distribuyen. Por consiguiente, se construye la infraestructura. Luego del fin del desarrollo de cada módulo comienza con su marcha blanca y finalizado esto la puesta en marcha. Antes de cualquier marcha blanca se realiza el manual de usuario, los analistas diseñador participan en la capacitación del personal, el cual se hará durante las marchas blancas y puestas en marcha. 



<!-- Start of picture text -->
a onan beg eal Onansrs nes<br><!-- End of picture text -->



<!-- Start of picture text -->
Ilustración 52<br><!-- End of picture text -->

12.2.9. Carta Gantt con Mantención expandido 

La mantención durará dos años e iniciará al inicio del segundo año del proyecto. En esta trabajarán los analistas de soporte y participarán en la gestión de cuentas de alto nivel, estos se encargarán de gestionar la mantención correctiva y adaptativa y su principal trabajó será el soporte al cliente. 

125 



<!-- Start of picture text -->
ZODIGITALDREAMS<br><!-- End of picture text -->



<!-- Start of picture text -->
Ilustración 53<br><!-- End of picture text -->

126 



Anexo 1: Requerimientos Funcionales 

|Id|RF01-01|
|---|---|
|Nombre|Iniciar sesión|
|Descripción|Un usuario del sistema puede ingresar a la aplicación con sus<br>credenciales. Tanto como los trabajadores, los participantes del<br>proyecto, los administradores de módulo y jefes de proyecto se<br>redirigen al módulo correspondiente.|
|Id<br>|RF02-01<br>|
|Nombre<br>|Gestionar proyectos<br>|
|Descripción<br>|El jefe de proyecto a través del sistema puede:<br>● Crear proyecto<br>● Eliminar proyecto existente<br>● Editar características del proyecto, tales como:<br>`o` Nombre del proyecto.<br>`o` Costo general del proyecto.<br>`o` Pre-deadline.<br>`o` Plazos.<br>~~_~~|
|Id<br>|RF02-02<br>|
|Nombre<br>|Gestionar recordatorio predeterminado<br>|
|Descripción<br>|El jefe de proyecto puede seleccionar un recordatorio<br>personalizado para las etapas del proyecto. Estas pueden ser<br>hasta cinco veces y se puede configurar en los siguientes<br>tiempos:<br>● El día del deadline.<br>● X días antes del deadline.<br>● Un periodo para la ejecución de cada tarea.<br>~~=~~|



127 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|Id|RF02-03|
|---|---|
|Nombre|Gestionar Actividades|
|Descripción|El jefe de especialidad a través del sistema puede:<br>● Agregar actividad.<br>● Eliminar actividad existente.<br>● Editar<br>características<br>de<br>una<br>actividad<br>(nombre,<br>descripción, plazo).<br>● Asignar participantes del proyecto a una actividad.<br>● Asignar recordatorio personalizado a una actividad.<br>● Asignar deadline de cada actividad.<br>● Asignar estado de la actividad.<br>● Asignar costos asociados de cada actividad.<br>● Asignar prioridad de la actividad.|



|Id|RF02-04|
|---|---|
|Nombre|Gestionar Participantes por especialidad de proyectos|
|Descripción|El jefe de especialidad, a través del sistema puede:<br>● Configurar accesos para diferentes tipos de cuentas de<br>trabajador.|
||● Eliminar participante de proyecto.<br>● Agregar participantes del proyecto.|



128 



|Id|RF02-05|
|---|---|
|Nombre|Realizar actividad|
|Descripción|El participante del proyecto puede completar la tarea. En esta<br>puede subir documentos. Si contiene documentos y se requieren<br>en la siguiente tarea, se adjuntan a la siguiente tarea. El<br>participante del proyecto recibe una notificación cuando se<br>recibe.|



|Id<br>|RF02-06<br>|
|---|---|
|Nombre<br>|Evaluar tarea recibida<br>|
|Descripción<br>|El participante del proyecto debe rechazar o aceptar los<br>documentos recibidos desde la tarea anterior. Al rechazar esta<br>puede adjuntar un mensaje para el participante. En cualquiera<br>de los dos casos se envía una notificación y un correo al<br>encargado de la tarea anterior y al jefe de proyecto.<br>|
|Id<br>|RF02-07<br>|
|Nombre<br>|Gestionar los documentos.<br>|
|Descripción|Un participante del proyecto puede subir o eliminar documentos<br>(esto incluye permisos, planos, informes y documentos variados)<br>para la realización de una tarea designada. Este se guarda con<br>un código que permite ordenarlos dentro de cada tipo y una<br>fecha de realización.|



129 



|Id|RF02-08|
|---|---|
|Nombre|Controlar costos de etapas y tareas de un proyecto|
|Descripción|Un jefe de proyecto debe controlar los costos relacionados a las<br>etapas y tareas de un proyecto. Para esto, puede:<br>● Aprobar el costo de una etapa<br>● Rechazar el costo de una etapa<br>● Aprobar el costo de una tarea<br>● Rechazar el costo de una tarea|
|Id<br>|RF02-09<br>|
|Nombre<br>|Controlar plazos de etapas y tareas de un proyecto<br>|
|Descripción<br>|Un jefe de proyecto debe controlar los plazos relacionados a las<br>etapas y tareas de un proyecto. Para esto, puede asignar:<br>● El tiempo de una etapa<br>● Las alarmas de una etapa<br>● El tiempo de una tarea<br>● Las alarmas de una tarea<br>~~_~~|
|Id<br>|RF03-01<br>|
|Nombre<br>|Gestión de credenciales para trabajadores de recursos<br>humanos.<br>|
|Descripción<br>|El administrador del módulo de recursos humanos puede<br>manejar y configurar los diferentes permisos para los usuarios del<br>sistema:<br>● Configurar permisos de visualización de los diferentes<br>sectores del módulo de recursos humanos.<br>● Agregar un trabajador de RR.HH.<br>● Eliminar a un trabajador de RR.HH.<br>~~=~~|



130 



|Id|RF03-02|
|---|---|
|Nombre|Gestión de contratos|
|Descripción|Un trabajador de RR.HH. puede gestionar los contratos de<br>diferentes trabajadores, el sistema debe ser capaz de:<br>● Visualizar contratos del personal.<br>● Agregar un contrato al sistema.<br>● Eliminar un contrato del sistema.<br>● Mover un contrato de lugar.<br>● Clasificar contratos entre internos y externalizados.|
|Id<br>|RF03-03<br>|
|Nombre<br>|Gestión de turnos<br>|
|Descripción<br>|Un trabajador de RR.HH. puede planificar y gestionar diferentes<br>turnos de otros trabajadores, generando mediante algoritmos.<br>● El trabajador puede dar parámetros para la generación<br>de horarios.<br>● El trabajador puede eliminar un horario.<br>● El trabajador puede modificar horarios.<br><sup>~~—~~</sup>|
|Id<br><br>|RF03-04<br><br>|
|Nombre<br><br>|Control de remuneraciones<br><br>|
|131<br>Descripción<br> <br>|El empleado de RR.HH. puede realizar tareas con las<br>remuneraciones de los trabajadores, entre las que están:<br>● Ver las remuneraciones en detalle de cada trabajador.<br>● Notificar problemas con las remuneraciones de un<br>trabajador.<br><br>|





|Id|RF03-05|
|---|---|
|Nombre|Evaluación de desempeño|
|Descripción|Un jefe de especialidad puede realizar acciones relacionadas a<br>la evaluación de un empleado por especialidad:<br>● Crear una evaluación.<br>● Editar una evaluación.<br>● Eliminar una evaluación.|



|Id<br>|RF03-06<br>|
|---|---|
|Nombre<br>|Firmar un contrato de trabajo<br>|
|Descripción<br>|Todos los empleados deben firmar un contrato de forma digital.<br>|
|Id<br>|RF03-07<br>|
|Nombre<br>|Gestión de seguros<br>|
|Descripción<br>|El empleado de RR.HH. puede agregar, eliminar y modificar<br>información de los seguros de los trabajadores de la empresa.<br>|
|Id<br>|RF04-01<br>|
|Nombre<br>|Gestionar proveedores<br>|
|Descripción<br>|El administrador de finanzas puede agregar, editar o eliminar los<br>datos de un proveedor.<br>|



132 





<!-- Start of picture text -->
Id  RF04-02<br>Nombre  Gestionar cuentas de gastos<br>Descripción  El administrador de finanzas puede:<br>● Registrar cuentas de gastos.<br>● Visualizar cuentas de gastos.<br>● Separa las cuentas de gastos por obra y etapa.<br>● Verificar el estado de las cuentas de gastos.<br><!-- End of picture text -->



<!-- Start of picture text -->
Id  RF05-01<br>Nombre  Verificación de acceso<br>Descripción  El encargado de seguridad puede verificar si una identificación<br>es válida de un participante de proyecto o un empleado de<br>proveedor.<br>Id  RF05-02<br>Nombre  Verificar cursos y equipamiento<br>Descripción  El encargado de seguridad puede verificar si una persona<br>cuenta con los cursos de seguridad y el equipamiento<br>correspondiente de un participante de proyecto o un empleado<br>de proveedor.<br>—<br>—<br>133<br><!-- End of picture text -->



|Id<br>|RF05-03<br>|
|---|---|
|Nombre<br>|Creación de tarjeta de identificación<br>|
|Descripción<br>|El administrador de seguridad puede crear tarjetas de<br>identificación a los participantes del proyecto y/o un empleado<br>de proveedor.<br>|
|Id<br>|RF06-01<br>|
|Nombre<br>|Gestionar trabajadores de soporte<br>|
|Descripción<br>|El administrador del módulo de soporte puede agregar,<br>modificar o eliminar operarios de soporte.<br>|
|Id<br>|RF06-02<br>|
|Nombre<br>|Crear solicitud de soporte<br>|
|Descripción<br>|Un trabajador de la empresa puede crear una nueva solicitud<br>de soporte.<br>|
|Id<br>|RF06-03<br>|
|Nombre<br>|Gestionar solicitud de soporte<br>|
|Descripción<br>|Un operario de soporte de nivel 1 o nivel 2 puede recibir<br>solicitudes de soporte con el fin de resolverlas.<br>|



134 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|Id|RF06-04|
|---|---|
|Nombre|Escalar solicitud de soporte|
|Descripción|Un operario de soporte de nivel 1 puede derivar una solicitud a<br>un operario de soporte de nivel 2 junto con la información ya<br>recopilada.|



|Id|RF06-05|
|---|---|
|Nombre|Marcar solicitud como resuelta|
|Descripción|Un operario de soporte de nivel 1 o de nivel 2 puede marcar la<br>solicitud que tenía asignada como resuelta para darla por<br>finalizada.|



135 



|Anexo 2: R<br>|equerimientos No Funcionales<br>|
|---|---|
|Id<br>|RNF01-01<br>|
|Nombre<br>|Seguridad por Geolocalización<br>|
|Descripción<br>|Los computadores del jefe de proyecto y el resto de los<br>participantes cuentan con dispositivos GPS.<br>|
|Id<br>|RNF01-02<br>|
|Nombre<br>|Alta disponibilidad<br>|
|Descripción<br>|El sistema cuenta con un SLA del 99,97%, por lo que el sistema<br>solo estará fuera de servicio 2 horas con 37 minutos como<br>máximo por año.<br>|
|Id<br>|RNF01-03<br>|
|Nombre<br>|Soporte remoto<br>|
|Descripción<br>|El sistema cuenta con un soporte remoto que demora menos de<br>20 minutos en solucionar el error.<br>|
|Id<br>|RNF01-04<br>|
|Nombre<br>|Alta portabilidad<br>|
|Descripción<br>|El sistema puede ser instalado de manera correcta en los<br>computadores de todos los participantes del proyecto.<br>|



136 



|Id<br>|RNF01-05<br>|
|---|---|
|Nombre<br>|Interfaz gráfica intuitiva<br>|
|Descripción<br>|El sistema posee una interfaz gráfica intuitiva y de fácil acceso,<br>señalando el progreso que se lleva a cabo en la etapa del<br>proyecto.<br>|
|Id<br>|RNF01-06<br>|
|Nombre<br>|Sistema de alertas<br>|
|Descripción<br>|La interfaz cuenta con un sistema de alertas, las cuales cuentan<br>con una verificación de lectura.<br>|
|Id<br>|RNF01-07<br>|
|Nombre<br>|Datacenter primario<br>|
|Descripción<br>|El sistema posee un datacenter externo primario, desde donde<br>se crean, leen, actualizan o eliminan los datos solicitados con<br>una respuesta inferior a 5 segundos.<br>|
|Id<br>|RNF01-08<br>|
|Nombre<br>|Datacenter secundario<br>|
|Descripción<br>|El sistema posee un datacenter externo de respaldo que se<br>actualiza cada 24 horas con la información del datacenter<br>primario.<br>|



137 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->

|Id|RNF01-09|
|---|---|
|Nombre|Funcionamiento off line|
|Descripción|El sistema cuenta con un modo de funcionamiento off line, el<br>cual se activa de manera automática cuando no se detecta|
||conexión, almacena de manera local los datos y cuando se|
||recupera la conexión estos se sincronizan con el data center|



138 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Anexo 3: Diagrama Arquitectura Lógica 

<u>https://drive.google.com/file/d/199UKk9EpFdZePdZ8aA4whFQ3o6bYG4v2/view? usp=sharing</u> 

139 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Anexo 4: Diagrama Arquitectura Física 

<u>https://drive.google.com/file/d/1DDhhhsYEeeeh9umXCrP1SJvigDmA3ApL/view ?usp=sharing</u> 

140 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Anexo 5: Topología de red de la Obra 

<u>https://drive.google.com/file/d/12CyrbCjr_kKDJgOLnS3OzY0ICRxJ6Cfa/view?us p=sharing</u> 

141 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Anexo 6: Arquitectura física basada en AWS 

<u>https://drive.google.com/file/d/1ZirF1Rub0Tsu_koCE6L889pn8lFfv0J/view?usp=sharing</u> 

142 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

# Anexo 7: EDT 

<u>https://drive.google.com/file/d/1A36k4xdZ5hYY6MyMHcPZOS8KB3HvCefK/view? usp=sharing</u> 

143 



<!-- Start of picture text -->
ODIGITALDREAMS<br><!-- End of picture text -->

Anexo 8: Carta Gantt expandida 

<u>https://drive.google.com/file/d/1ZKt1OesLsn_fS3A712YL9PNi7k4VTWgD/view?usp</u> =sharing 

144 



<!-- Start of picture text -->
ZODIGITAL<br><!-- End of picture text -->



<!-- Start of picture text -->
JUNIO, 2022<br><!-- End of picture text -->

145 

