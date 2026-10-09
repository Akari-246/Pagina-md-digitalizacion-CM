<!--  TEMA  -->

# Fundamentos de ciberseguridad
 
[<-- Volver al inicio](README.md) | [Siguiente: Malware y el caso WannaCry -->](malware-y-wannacry.md)
 
## Índice
 
1. [¿Qué es la ciberseguridad?](#qué-es-la-ciberseguridad)
2. [¿Qué se protege?](#qué-se-protege)
3. [Gestión del riesgo](#gestión-del-riesgo)
4. [¿De qué nos protegemos? Las amenazas](#de-qué-nos-protegemos-las-amenazas)
5. [¿Quién está detrás? Tipos de hacker](#quién-está-detrás-tipos-de-hacker)
6. [Las amenazas del futuro](#las-amenazas-del-futuro)
---
 
<br>

## ¿Qué es la ciberseguridad?
 
Es la práctica de proteger personas, sistemas y datos frente a ciberataques mediante tecnologías, procesos y políticas. Abarca la infraestructura informática (hardware, software, redes) y, sobre todo, la información que contiene o que circula por las redes. Se apoya en estándares, protocolos, herramientas y leyes que minimizan los riesgos.  
 
<br>

> La ***seguridad de la información*** protege los datos en cualquier formato (también en papel), mientras que la ***seguridad informática*** se centra en el medio digital.
 
<br>

La seguridad informática busca garantizar tres propiedades, conocidas como la **tríada CIA**:
 
<img src="https://www.4itn.mx/wp-content/uploads/elementor/thumbs/Triada-06-q4wfz6cf9oeyhtdq7h672zttknd0zsfrhbs4d0qo80.png" alt="Tríada CIA: confidencialidad, integridad y disponibilidad" width="250"><br>


- **Confidencialidad**: solo accede a la información quien está autorizado.
- **Integridad**: los datos no se alteran sin permiso.
- **Disponibilidad**: los datos están accesibles cuando se necesitan.

<br>

## ¿Qué se protege?
 
- **Infraestructura**: equipos y sistemas frente a fallos, robos, incendios, sabotajes, desastres naturales o cortes eléctricos.
- **Usuarios**: que su uso del sistema no comprometa la seguridad.
- **Información**: el activo principal, protegida en su confidencialidad, integridad y disponibilidad.  

<br>

## Gestión del riesgo
 
Las organizaciones usan modelos y normas para ordenar su trabajo:  
 
### El cubo de McCumber (1991)
 
El Cubo de McCumber es un modelo conceptual y marco de trabajo tridimensional creado por **John McCumber**. Se utiliza en el ámbito de la ciberseguridad y la seguridad de la información para evaluar, diseñar y gestionar de manera integral la protección de los sistemas y los datos dentro de una organización.  
Parte de una idea: la seguridad **no depende de un solo elemento**, sino de varias dimensiones conectadas entre sí, que se representan como las caras de un cubo.
 
<img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/McCumber_cube.jpg" alt="Cubo de McCumber: tres dimensiones de la seguridad de la información" width="270"><br>
 
#### Dimensión 1: los principios (tríada CIA)
- **Confidencialidad:** solo accede a la información quien está autorizado. *Ejemplo:* en una base de datos médica, solo el personal sanitario autorizado ve los datos del paciente.
- **Integridad:** la información no se altera sin autorización ni por error. *Ejemplo:* que nadie no autorizado pueda modificar registros financieros para cometer un fraude.
- **Disponibilidad:** la información y los sistemas funcionan cuando se necesitan. *Ejemplo:* que una tienda online esté accesible en las horas punta de ventas.

#### Dimensión 2: los estados de los datos 
Los datos pueden estar **almacenados**, **en transmisión** (en tránsito por la red) o **en procesamiento**. Cada estado tiene distintos riesgos.
 
#### Dimensión 3: las medidas de protección
* **Tecnología:** antivirus, firewalls, cifrado, parches.
* **Políticas y prácticas:** normas, procedimientos y directrices de seguridad.
* **Factor humano:** que los usuarios conozcan su papel y sus responsabilidades.
Como cada dimensión tiene tres elementos, el cubo forma 27 combinaciones (3 × 3 × 3). Cada minicubo responde a una pregunta concreta. Por ejemplo: ***confidencialidad + tecnología + procesamiento*** significa *¿cómo uso la tecnología para proteger la privacidad de los datos mientras se procesan?*.
 
#### ¿Por qué está en esta web?
1. **Organiza el contenido**. Da un marco para ordenar temas que parecen sueltos: qué protegemos, dónde y con qué.
2. **Explica los conceptos clave**. La confidencialidad, integridad y disponibilidad aparecen en todo el sitio.
3. **Enseña que la seguridad no es solo tecnología**. Un antivirus no basta sin normas ni usuarios formados, por eso los [consejos de protección](malware-y-wannacry.md#cómo-protegerse) mezclan herramientas y hábitos.
4. **Permite analizar casos reales**, como [WannaCry visto con el cubo](malware-y-wannacry.md#wannacry-visto-con-el-cubo-de-mccumber).
5. **Es una herramienta profesional** que usan las organizaciones para identificar vulnerabilidades y amenazas.  

Fuentes: [Wikipedia: McCumber cube](https://en.wikipedia.org/wiki/McCumber_cube), [Epampliega: cubo de McCumber](https://epampliega.com/blog/index.php/2023/09/07/que-es-el-cubo-de-mccumber/)
 
<br>

### El ENS (Esquema Nacional de Seguridad)
Fija los requisitos mínimos de seguridad de las administraciones públicas españolas. Define tres figuras principales (artículo 10):  
 
1. **Responsable de la Información**
2. **Responsable del Servicio**
3. **Responsable de la Seguridad**  
La guía **CCN-STIC 801** añade el **Responsable del Sistema de Información**, encargado del buen funcionamiento del sistema y de aplicar las medidas necesarias.
 
Más información en [INCIBE](https://www.incibe.es), el instituto español de ciberseguridad.
 
<br>

## ¿De qué nos protegemos? Las amenazas
**Causas habituales**: usuarios (suelen tener permisos excesivos), malware, errores de programación explotables, intrusos, siniestros, personal técnico interno y fallos electrónicos o lógicos.
 
Según el **origen**:
 
* Internas: según el CSI, entre el 60 % y el 80 % de los incidentes vienen de dentro. Son más peligrosas porque conocen la red y los firewalls/IPS no suelen vigilar el tráfico interno.
* Externas: vienen de fuera; aquí es clave la seguridad perimetral.
Según el **efecto**: robo o destrucción de información, anulación de sistemas, suplantación de identidad, venta de datos, estafas.
 
Según el **medio**: virus, phishing, ingeniería social, denegación de servicio y spoofing (DNS, IP, DHCP).
 
De todos estos medios, el más extendido es el malware. [Malware y el caso WannaCry](malware-y-wannacry.md)
 
<br>

## ¿Quién está detrás? Tipos de hacker
Un hacker es una persona con grandes conocimientos informáticos capaz de analizar sistemas y detectar vulnerabilidades. **No todos son criminales**.
 
### Los que protegen o aprenden
* **White Hat** (éticos): autorizados, protegen empresas y gobiernos.  
* **Red Hat**: combaten a los Black Hat con tácticas más agresivas.  
* **Green Hat**: aprendices con muchas ganas de aprender, que a veces se pasan de la raya.

### Los que atacan
* **Black Hat**: actúan con mala intención para robar datos o causar daño.  
* **Script Kiddies**: aficionados que usan herramientas ajenas para llamar la atención.  
* **Patrocinados por un Estado**: trabajan para gobiernos en operaciones de espionaje o ciberguerra.  
* **Insiders malintencionados**: empleados que filtran datos o sabotean a su propia organización (la amenaza interna que vimos antes).

### Los intermedios
* **Gray Hat**: actúan sin autorización, pero sin intención clara de dañar.  
* **Hacktivistas**: usan el hacking para causas políticas o sociales.  
Fuentes: [WeLiveSecurity](https://www.welivesecurity.com/es/otros-temas/tipos-hacker-diferencias/), [CampusCiberseguridad](https://www.campusciberseguridad.com/blog/tipos-de-hackers/)
 
<br>

## Las amenazas del futuro
Con la Web 3.0 (web semántica), los ataques se profesionalizan y ya no buscan solo robar claves, sino manipular el significado del contenido digital (por ejemplo, alterar el saldo de una cuenta para provocar pánico y luego robar). También crece la elaboración de perfiles de usuario a partir de búsquedas, historial, geolocalización e imágenes.
 
---
 
[<-- Volver al inicio](README.md) | [Siguiente: Malware y el caso WannaCry -->](malware-y-wannacry.md)