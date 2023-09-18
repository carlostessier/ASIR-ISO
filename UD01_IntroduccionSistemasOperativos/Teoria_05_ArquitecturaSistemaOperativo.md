---
title: UD01 - Introducción a los Sistemas Operativos
author: Angel Berlanas Vicente, Carlos Tessier
header-includes: |
lang: es-ES
keywords: [ASIR, ISO, Arquitectura de un Sistema Informático, licencias]
---


\newpage

# Concepto y Funciones de los Sistemas Operativos

Los sistemas operativos (SO) son software especializados que actúan como intermediarios entre el hardware del ordenador y el usuario, proporcionando un entorno en el que los programas de aplicación pueden ejecutarse de manera eficiente y segura.

## Roles Clave de un Sistema Operativo

El sistema operativo juega varios roles esenciales en la gestión de la computadora. Aunque la simplificación y la abstracción del hardware son aspectos primordiales, sus responsabilidades van más allá:

### Seguridad y Protección

Una de las tareas cruciales del SO es garantizar la seguridad y la integridad de la información y los recursos del sistema. Debe:

* Defenderse contra accesos no autorizados, ataques maliciosos y vulnerabilidades.
* Proteger los datos y programas de los usuarios de interferencias y daños, ya sean intencionales o accidentales.
* Implementar mecanismos de autenticación y control de acceso.
* Utilizar modos de operación diferenciados, como el modo kernel (o sistema) y el modo usuario. En el modo kernel, el SO tiene acceso total al hardware y puede ejecutar cualquier instrucción. Por otro lado, los programas en modo usuario tienen restricciones y no pueden interactuar directamente con el hardware ni ejecutar instrucciones sensibles.

### Abstracción del Hardware

El SO ofrece una vista simplificada y uniforme del hardware, ocultando muchos de los detalles intrincados y especificidades de los componentes individuales. Esto permite que:

* Los programas de aplicación no necesiten ser escritos para un hardware específico.
* Los usuarios interactúen con el sistema de una manera más intuitiva, sin tener que conocer los detalles técnicos del hardware subyacente.

![Arquitectura del SO](ArquitecturaSistemaOperativo/SO_Capas.PNG)

**Nota:** El gráfico de "Capas del SO" muestra una representación simplificada de cómo el sistema operativo se sitúa entre el hardware y las aplicaciones, ofreciendo diversos niveles de abstracción y servicios.

A medida que avanzamos en el estudio de los sistemas operativos, es esencial comprender la complejidad y las múltiples capas de operación que existen bajo la superficie de la interacción diaria del usuario. Estas capas trabajan en conjunto para garantizar que el sistema funcione de manera eficiente, segura y confiable.

# Concepto de Abstracción en Sistemas Operativos

La abstracción es un principio clave en el diseño y funcionamiento de los sistemas operativos. Se centra en ocultar la complejidad subyacente de los sistemas y proporcionar interfaces más simplificadas y generales a los niveles superiores. 

## Propósito de la Abstracción

El software moderno y los lenguajes de programación buscan minimizar la exposición a detalles de bajo nivel. Esto se realiza mediante:

* **Simplificación de Interacciones:** Al encapsular y esconder detalles internos, los sistemas operativos proporcionan interfaces más comprensibles y manejables para los programadores y usuarios.
* **Creación de Recursos Virtuales:** Estos recursos, construidos sobre la base de los recursos físicos, ofrecen capacidades ampliadas y generalmente superiores, transformando la percepción de la máquina física en una "máquina extendida".
  
![Representación de la Abstracción](ArquitecturaSistemaOperativo/SO_MaquinaExtendida.PNG)

A través de la lente de abstracción, la máquina física se transfigura en un entorno con características y capacidades ampliadas, donde elementos como carpetas compartidas, usuarios de red o impresoras compartidas se manifiestan como si fueran componentes innatos.

## Beneficios desde la Perspectiva del Usuario

El sistema operativo, mediante la abstracción, introduce servicios y facilidades que trascienden las capacidades directas del hardware:

* **Ejecución Simultánea:** Permite la ejecución concurrente de múltiples programas, potenciando la multitarea.
* **Interacción Mejorada:** Favorece la comunicación entre el usuario y las aplicaciones, generando una experiencia de usuario más amigable y eficiente.
* **Administración Optimizada:** Se encarga de la gestión eficaz de recursos, almacenamiento y servicios.

En resumen, el objetivo primordial de la abstracción en el sistema operativo es maximizar la eficacia del hardware, a la vez que simplifica y enriquece su utilización para usuarios y aplicaciones.

\newpage

# Responsabilidades de los Sistemas Operativos

Los sistemas operativos desempeñan múltiples funciones cruciales en la informática moderna, actuando como intermediarios entre el hardware y el usuario. A medida que la tecnología avanza, estas funciones se han adaptado y ampliado para satisfacer las necesidades contemporáneas. Veamos las principales responsabilidades de un sistema operativo en detalle:

## Funciones Esenciales de los Sistemas Operativos

### Administración de Procesos

Es vital comprender la distinción entre un programa y un proceso. Mientras que un programa es una entidad estática, cuando se carga en memoria y comienza su ejecución se transforma en un proceso activo. Los sistemas operativos gestionan el inicio, ejecución y terminación de estos procesos.

### Control de Memoria

La administración de memoria es intrínseca a la gestión de procesos. Al ejecutar un proceso, el sistema operativo asigna un espacio de memoria exclusivo para él. Posteriormente, cuando el proceso concluye, esa memoria es liberada para ser reutilizada.

### Manejo de Archivos

En esencia, un archivo es una representación de datos almacenados. El sistema operativo facilita la creación, lectura, modificación y eliminación de estos archivos, garantizando una organización óptima y una protección adecuada de los mismos.

### Coordinación de Dispositivos de Entrada/Salida (E/S)

Los dispositivos de E/S (como teclados, ratones o impresoras) requieren de una gestión especializada para asegurar su correcta comunicación con el sistema. El sistema operativo se encarga de ofrecer una interfaz intuitiva y eficiente para estos dispositivos.

### Gestión de Conexiones de Red

Los sistemas operativos modernos manejan aspectos relacionados con la conectividad de red, desde la configuración de hardware y software hasta la administración de protocolos y aplicaciones de red.

### Seguridad y Accesibilidad

Un aspecto esencial es garantizar que los recursos del sistema estén protegidos y que solo los usuarios autorizados puedan acceder o modificar determinada información o configuración.

\newpage

# Clasificación Actualizada de Sistemas Operativos

Los sistemas operativos pueden ser categorizados según diferentes criterios. Uno de los más utilizados se basa en los servicios que proporcionan.

![Clasificación de SO Modernos](ArquitecturaSistemaOperativo/SO_Tipos.PNG)
\

### Basados en la Cantidad de Usuarios

#### Monousuarios

Estos sistemas se diseñan para atender a un único usuario en un momento dado, independientemente de la capacidad multitarea del equipo.

**Ejemplos de SO Monousuarios actuales:**

* Windows 11 Home
* MacOS Monterey (en un contexto de usuario doméstico)

#### Multiusuario

Están diseñados para atender múltiples usuarios simultáneamente, ya sea en un entorno local o a través de una red.

**Ejemplos de SO Multiusuario actuales:**

* Linux (por ejemplo, Ubuntu 22.04)
* Windows Server 2022

### Basados en la Capacidad de Tareas

#### Monotarea

Estos sistemas permiten la ejecución de una única tarea a la vez. Son menos comunes en la era actual debido a la demanda de multitarea.

#### Multitarea

Estos sistemas son capaces de gestionar y ejecutar múltiples tareas al mismo tiempo, proporcionando una experiencia más fluida y productiva para el usuario.

**Ejemplos de sistemas multitarea modernos:**

* Windows 11 Pro
* MacOS Monterey
* Android 13

\newpage

# Sistemas Operativos en Red y Computación Distribuida

La computación ha evolucionado significativamente en las últimas décadas. La capacidad de conectar múltiples máquinas y hacer que trabajen en conjunto ha llevado a la creación de sistemas increíblemente poderosos que trascienden la capacidad de cualquier computadora individual. Veamos con más detalle los sistemas operativos distribuidos y cómo han influido en esta revolución.

## Concepto de Sistema Operativo Distribuido

Un sistema operativo distribuido conecta un conjunto de computadoras que están geográficamente dispersas a través de una red de comunicaciones. Estas máquinas operan de manera coordinada, ofreciendo la ilusión al usuario de que están interactuando con un solo sistema unificado. Esto significa que un recurso (como un archivo o un programa) puede residir en cualquier máquina del sistema y aún ser accesible para cualquier usuario, independientemente de su ubicación.

### Beneficios Principales

- **Aumento del Rendimiento**: Al conectar múltiples computadoras, se multiplica la potencia de procesamiento, permitiendo abordar tareas que serían imposibles para una sola máquina.
  
- **Confiabilidad y Tolerancia a Fallos**: Si un componente falla, el sistema continúa funcionando gracias a los componentes redundantes. Es decir, la operatividad no se ve comprometida por el fallo de una sola máquina.

- **Escalabilidad**: La capacidad del sistema puede ampliarse simplemente añadiendo más máquinas al conjunto.

## Computación Distribuida: Grid y Clustering

Los desafíos computacionales actuales, como la simulación de fenómenos naturales, la búsqueda de nuevos fármacos o las operaciones a gran escala de motores de búsqueda, requieren de potencias de procesamiento que exceden las capacidades de los sistemas tradicionales. Aquí es donde la computación distribuida brilla.

- **Computación Grid**: Se refiere a la combinación de recursos computacionales de múltiples ubicaciones para alcanzar un objetivo común. Ejemplos notables incluyen el proyecto [Seti@Home](http://setiweb.ssl.berkeley.edu/), que busca señales de vida extraterrestre aprovechando el procesamiento no utilizado de computadoras voluntarias.

- **Computación Zombie**: Es un modelo en el que se aprovecha la capacidad de procesamiento no utilizada de computadoras que están encendidas pero inactivas. En lugar de desperdiciar ese potencial en protectores de pantalla o tareas menores, se utiliza para procesos más complejos.

- **Clustering**: Implica conectar múltiples computadoras (usualmente a través de una red de alta velocidad) para que funcionen como una sola entidad. Estas agrupaciones, o "clusters", ofrecen redundancia y alta disponibilidad. Google, por ejemplo, utiliza clusters para manejar las innumerables solicitudes de búsqueda que recibe diariamente.

### Sistemas Operativos para Clustering y Grids:

Algunos de los sistemas operativos actuales y relevantes para esta tarea son:

- Kubernetes (para orquestación de contenedores en clusters)
- Apache Hadoop (para procesamiento distribuido de grandes conjuntos de datos)
- OpenStack (para cloud computing)

![Google Data Center](ArquitecturaSistemaOperativo/SO_Google.PNG)

En la imagen, observamos el rudimentario pero funcional primer servidor de **Google**. Representa la esencia del pensamiento innovador: optimizar y escalar según las necesidades, incluso si eso significa deshacerse de la carcasa externa para aprovechar al máximo el espacio y los recursos.

# Explorando las Versiones de Windows

La elección del sistema operativo correcto es esencial para garantizar un rendimiento y seguridad óptimos en nuestras actividades informáticas. A continuación, te ofrecemos un recorrido por las versiones de Windows, considerando las actualizaciones más recientes.

## Windows para Servidores

Si estás buscando un sistema operativo robusto para servidores, Windows ofrece una variedad de opciones específicas según tus necesidades. Desde las versiones anteriores hasta la reciente Windows Server 2022, cada edición brinda características y capacidades específicas.

Para una visión más detallada sobre las características y comparativas entre versiones, te recomendamos consultar:

[Comparativa de Windows Server](https://www.microsoft.com/es-mx/cloud-platform/windows-server-comparison)

![Representación de Windows Server](Versiones/WindowsServer_cover.png)

## La Trayectoria de Windows: Desde sus Inicios hasta Windows 11

Windows ha evolucionado considerablemente desde sus inicios con Windows 3.11 hasta llegar a Windows 11. A lo largo de los años, Microsoft ha lanzado diversas versiones, cada una con su periodo de soporte específico. Es importante recordar que, una vez finalizado el soporte, la versión en cuestión deja de recibir actualizaciones críticas.

![Gráfico de Fin del Soporte](Versiones/fin-soporte-windows.png)

## Windows 10 y su Filosofía de Actualizaciones

Desde su lanzamiento, Windows 10 ha implementado un modelo de actualización continua, lo que significa que se incorporan mejoras y parches de seguridad con regularidad. Este enfoque busca ofrecer a los usuarios las últimas características de seguridad y rendimiento.

Para estar informado sobre las actualizaciones más recientes y su contenido, es fundamental visitar:

[Historial de Actualizaciones de Windows 10](https://support.microsoft.com/es-es/help/4464619/windows-10-update-history)

Aunque en el material original se menciona la versión 1809 de Windows 10, es vital estar al tanto de que han existido múltiples actualizaciones desde entonces, fortaleciendo aún más la seguridad y funcionalidad del sistema.

![Imagen de Windows 10 1809](Versiones/windows10-1809.png)

## Adentrándonos en Windows 11

Tras Windows 10, Microsoft ha presentado Windows 11, una versión que promete ser más intuitiva, segura y orientada a la productividad. Con una interfaz renovada y características optimizadas, Windows 11 se posiciona como la próxima era en el mundo de los sistemas operativos para escritorio. Si decides explorar esta versión, es vital familiarizarte con sus requisitos y características para aprovecharla al máximo.

---

Mantenerse al día con las versiones y actualizaciones es crucial para garantizar un sistema seguro y eficiente. Ya sea que prefieras Windows para servidores, escritorio o ambas opciones, elegir la versión adecuada es el primer paso hacia una experiencia informática optimizada.

## Explorando el Diverso Universo de GNU/Linux

GNU/Linux es un ecosistema vasto y diverso, con numerosas variantes desarrolladas por comunidades y empresas alrededor del mundo. Empresas reconocidas como Red Hat (ahora parte de IBM), Canonical (creadora de Ubuntu), y hasta Microsoft, han abrazado la flexibilidad y el potencial de este sistema operativo. Ejemplo de su omnipresencia es el sistema operativo Android, desarrollado por Google, el cual está basado en el kernel de Linux.

La combinación del kernel Linux y las herramientas GNU conforman la base fundamental sobre la que se construyen estas distintas variantes o distribuciones.

![GNU/LinuX Diversidad](Versiones/Gnu-and-penguin-color.png)
\ 

### Un Vistazo al Pasado

Durante la década de 1970, `UNIX` dominaba el panorama tecnológico como un sistema operativo privativo, siendo el favorito entre los círculos académicos e industriales. Su popularidad radicaba en:

* Su portabilidad y adaptabilidad.
* Una arquitectura limpia y sencilla.
* Estabilidad notoria.
* Políticas de distribución de software abiertas.
* Normativas anti-monopolio que obligaban a AT&T, su propietario, a compartir el código con instituciones selectas.

### El Viaje de Richard Stallman

En contraste, Richard Stallman emergió de los laboratorios del MIT, perteneciendo a una tradición de programadores con una visión diferente.

![Visión de Stallman](Versiones/stallman.jpg)
\ 

A medida que la década de 1980 comenzaba, la comunidad _hacker_ del MIT enfrentaba desafíos. Stallman, acostumbrado a un ambiente donde el software se compartía y se mejoraba colectivamente, vio la necesidad de crear un sistema operativo libre y moderno como respuesta a la creciente ola de software privativo. Nace así el proyecto GNU, con la misión de ser compatible con UNIX, pero con una esencia libre y colaborativa.

### Linus Torvalds y el Nacimiento del Kernel Linux

En 1991, armado con las herramientas proporcionadas por el proyecto GNU, Linus Torvalds comenzó a desarrollar el kernel de Linux, inspirado en Minix, un sistema creado por Andrew Tanenbaum.

![El Creador de Linux](Versiones/Linus-Torvalds.jpg)
\ 

Las motivaciones iniciales de Torvalds surgieron de su deseo de tener una alternativa libre a Minix. Pese a las controversias iniciales con otros sistemas, Torvalds apostó por Linux, y en 1992, optó por la Licencia Pública General (GPL). El proyecto ganó tracción, y con la colaboración global, Linux evolucionó para ser una opción robusta y compatible con UNIX.

La fusión del sistema GNU con el kernel Linux dio como resultado un sistema operativo completamente libre y funcional, conocido tanto como "GNU/Linux" como simplemente "distribución Linux".

Aunque a lo largo de este módulo se usará tanto `GNU/LinuX` como `LinuX`, es vital reconocer que el término más preciso y reconocido en la comunidad es **GNU/LinuX**.

### Distribuciones y Familias: El Árbol de la Vida de Linux

Las distribuciones, al basarse en otras previas, heredan ciertas características y metodologías. Por ejemplo, las variantes basadas en Debian utilizan archivos `.deb` para la instalación de software y cuentan con repositorios específicos para esos paquetes.

![Herencia Debian y Ubuntu](Versiones/debian_ubuntu.jpg)
\ 

Navegar por el vasto mar de distribuciones puede ser un desafío. Es esencial estar informado sobre las tendencias y las decisiones de las comunidades y empresas detrás de estas versiones.

Para una visión más detallada de las distribuciones de GNU/LinuX, consulte el siguiente enlace:

[Distribuciones Populares de GNU/LinuX](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg)

## Panorama de Distribuciones de GNU/Linux Destacadas

El ecosistema de GNU/Linux está repleto de distribuciones, cada una con su enfoque y propósito particular. A continuación, se presenta una revisión de algunas de las distribuciones más prominentes que han dejado una huella en la comunidad y la industria.

### Debian: La Madre de Distribuciones

![Logo de Debian](Versiones/debian.jpeg)
\ 

[Debian](https://www.debian.org/intro/about#what) es reconocida por su rigurosa adhesión a los principios del software libre y por su sistema de gestión de paquetes "apt". Es la base de muchas otras distribuciones, incluido Ubuntu.

### Ubuntu: Facilidad y Elegancia

![Logo de Ubuntu](Versiones/ubuntu-logo.png)
\ 

[Ubuntu](https://www.ubuntu.com/) es una de las distribuciones más populares y accesibles para principiantes. Creada por Canonical, combina la estabilidad de Debian con un toque moderno, proporcionando actualizaciones regulares y características de vanguardia.

### Fedora: Innovación y Avance

![Logo de Fedora](Versiones/fedora.png)
\ 

[Fedora](https://getfedora.org/es/) es conocida por incorporar las últimas tecnologías y herramientas, sirviendo a menudo como campo de pruebas para características que eventualmente se incorporan en Red Hat Enterprise Linux.

### Red Hat: Estabilidad Empresarial

![Logo de RedHat](Versiones/redhat.svg.png)
\ 

[Red Hat](https://www.redhat.com/es) es una de las principales distribuciones comerciales, enfocada en proporcionar soluciones estables y soportadas para empresas. Su modelo de negocio se basa en el soporte y los servicios.

### OpenSUSE: Flexibilidad y Elección

![Logo de OpenSUSE](Versiones/opensuse.png)
\ 

[OpenSUSE](https://www.opensuse.org/) ofrece dos principales versiones: Leap, que se centra en la estabilidad, y Tumbleweed, que es rolling release y tiene las últimas versiones de software.

### ArchLinux: Sencillez y Control Total

![Logo de ArchLinuX](Versiones/archlinux.png)
\ 

[ArchLinux](https://www.archlinux.org/) adopta la filosofía de mantener las cosas simples. Es conocido por su sistema de paquetes "pacman" y por ofrecer a los usuarios un control total sobre su sistema.

### Alpine: Minimalismo y Seguridad

![Logo de Alpine](Versiones/alpine.png)
\ 

[Alpine](https://alpinelinux.org/) es una distribución ligera diseñada para la seguridad, simplicidad y eficiencia de recursos. Es especialmente popular en entornos de contenedores, como Docker.
