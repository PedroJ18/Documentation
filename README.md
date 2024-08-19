UNIVERSIDAD PERUANA<br>
 DE CIENCIAS APLICADAS



  <img src="https://hackmd.io/_uploads/ryJoz7YcR.png" alt="Logo" />



  **SI729 Desarrollo de Aplicaciones Open Source** <br>
    **Sección: WS53**<br>
    **Carrera: Ingeniería de Software**<br>
    **Ciclo: 5-6**<br>
    **Profesor:**<br>
    **Juan Antonio Flores Moroco**<br>
    **"Informe de Trabajo Final"**<br>
    **Tema: SphereHub**<br>
    **Producto: BookSphere**<br>
    **Agosto 2024**<br>

**Integrantes:**


- Gómez Vallejos Sergio André - U20221D401
- Salon Puerta Merly - U20201B772
- Romero Qwistgaard, Russell Stephen - U20211043
- Nanfuñay Liza, Pedro Jesús - U202215462
- Fabian Puente, Ronaldo Macedonio - U20201B193


<p style="text-align: center;">
  <strong>Registro de versiones de informe:</strong><br>
</p>


| Entregables  | Fecha | Autor | Descripción de modificación |
|-----------|-----------|-----------|-----------|
| TB1| Fila 1, Columna 2 | Fila 1, Columna 3 | Fila 1, Columna 4 |
| TP | Fila 2, Columna 2 | Fila 2, Columna 3 | Fila 2, Columna 4 |
| TB2 | Fila 3, Columna 2 | Fila 3, Columna 3 | Fila 3, Columna 4 |
| TF | Fila 4, Columna 2 | Fila 4, Columna 3 | Fila 4, Columna 4 |


**Project Report Collaboration Insights**

| URL del Repositorio |
|----------------------|
| https://github.com/orgs/BookSphere-SH/repositories |




<p style="text-align: center; font-weight: bold;">
  Tabla de contenido
  
</p>

1. [CAPÍTULO I: Introducción](#CAPÍTULO-I-Introducción)<br>
      1.1. [Startup Profile](#Startup-Profile)<br>
      1.1.1. [Descripción de la Startup](#Descripción-de-la-Startup)<br>
      1.1.2. [Perfiles de integrantes del equipo](#Perfiles-de-integrantes-del-equipo)<br>
   1.2. [Solution Profile](#Solution-Profile)<br>
      1.2.1. [Antecedentes y problemática](#Antecedentes-y-problemática)<br>
      1.2.2. [Lean UX Process](#Lean-UX-Process)<br>
             1.2.2.1 [Lean UX Problem Statements](#Lean-UX-Problem-Statements)<br>
             1.2.2.2 [Lean UX Assumptions](#Lean-US-Assumptions)<br>
             1.2.2.3 [Lean UX Hypothesis Statements](#Lean-UX-Hypothesis-Statements)<br>
             1.2.2.4 [Lean UX Canvas](#Lean-UX-Canvas) <br>
1.3. [Segmentos objetivo](#Segmentos-objetivo) <br>
2. [CAPÍTULO II: Requirements Elicitation & Analysis](#Capítulo-II-Requirements-Elicitation--Analysis) <br>
   2.1. [Competidores](#Competidores) <br>
      2.1.1. [Análisis competitivo](#Análisis-competitivo) <br>
      2.1.2. [Estrategias y tácticas frente a competidores](#Estrategias-y-tácticas-frente-a-competidores) <br>
   2.2. [Entrevistas](#Entrevistas) <br>
      2.2.1. [Diseño de entrevistas](#Diseño-de-entrevistas) <br>
      2.2.2. [Registro de entrevistas](#Registro-de-entrevistas)<br> 
      2.2.3. [Análisis de entrevistas](#Análisis-de-entrevistas)<br> 
   2.3. [Needfinding](#Needfinding) <br>
      2.3.1. [User Personas](#User-Personas) <br>
      2.3.2. [User Task Matrix](#User-Task-Matrix) <br>
      2.3.3. [User Journey Mapping](#User-Journey-Mapping) <br>
      2.3.4. [Empathy Mapping](#Empathy-Mapping) <br>
      2.3.5. [As-is Scenario Mapping](#As-is-Scenario-Mapping) <br>
   2.4. [Ubiquitous Language](#Ubiquitous-Language) <br>
3. [CAPÍTULO III: Requirements Specification](#Capítulo-III-Requirements-Specification) <br>
   3.1. [To-Be Scenario Mapping](#To-Be-Scenario-Mapping) <br>
   3.2. [User Stories](#User-Stories) <br>
   3.3. [Impact Mapping](#Impact-Mapping) <br>
   3.4. [Product Backlog](#Product-Backlog) <br>
4. [CAPÍTULO IV: Product Design](#Capítulo-IV-Product-Design) <br>
   4.1. [Style Guidelines](#Style-Guidelines) <br>
      4.1.1. [General Style Guidelines](#General-Style-Guidelines) <br>
      4.1.2. [Web Style Guidelines](#Web-Style-Guidelines) <br>
   4.2. [Information Architecture](#Information-Architecture) <br>
      4.2.1. [Organization Systems](#Organization-Systems) <br>
      4.2.2. [Labeling Systems](#Labeling-Systems) <br>
      4.2.3. [SEO Tags and Meta Tags](#SEO-Tags-and-Meta-Tags) <br>
      4.2.4. [Searching Systems](#Searching-Systems) <br>
      4.2.5. [Navigation Systems](#Navigation-Systems) <br>
   4.3. [Landing Page UI Design](#Landing-Page-UI-Design) <br>
      4.3.1. [Landing Page Wireframe](#Landing-Page-Wireframe) <br>
      4.3.2. [Landing Page Mock-up](#Landing-Page-Mock-up) <br>
   4.4. [Web Applications UX/UI Design](#Web-Applications-UX-UI-Design) <br>
      4.4.1. [Web Applications Wireframes](#Web-Applications-Wireframes) <br>
      4.4.2. [Web Applications Wireflow Diagrams](#Web-Applications-Wireflow-Diagrams) <br>
      4.4.3. [Web Applications Mock-ups](#Web-Applications-Mock-ups) <br>
      4.4.4. [Web Applications User Flow Diagrams](#Web-Applications-User-Flow-Diagrams) <br>
   4.5. [Web Applications Prototyping](#Web-Applications-Prototyping) <br>
   4.6. [Domain-Driven Software Architecture](#Domain-Driven-Software-Architecture) <br>
      4.6.1. [Software Architecture Context Diagram](#Software-Architecture-Context-Diagram) <br>
      4.6.2. [Software Architecture Container Diagrams](#Software-Architecture-Container-Diagrams) <br>
      4.6.3. [Software Architecture Components Diagrams](#Software-Architecture-Components-Diagrams) <br>
   4.7. [Software Object-Oriented Design](#Software-Object-Oriented-Design) <br>
      4.7.1. [Class Diagrams](#Class-Diagrams) <br>
      4.7.2. [Class Dictionary](#Class-Dictionary) <br>
   4.8. [Database Design](#Database-Design) <br>
      4.8.1. [Database Diagram](#Database-Diagram) <br>
5. [CAPÍTULO V: Product Implementation, Validation & Deployment](#Capítulo-V-Product-Implementation--Validation--Deployment) <br>
   5.1. [Software Configuration Management](#Software-Configuration-Management) <br>
      5.1.1. [Software Development Environment Configuration](#Software-Development-Environment-Configuration) <br>
      5.1.2. [Source Code Management](#Source-Code-Management) <br>
      5.1.3. [Source Code Style Guide & Conventions](#Source-Code-Style-Guide--Conventions) <br>
      5.1.4. [Software Deployment Configuration](#Software-Deployment-Configuration) <br>
   5.2. [Landing Page, Services & Applications Implementation](#Landing-Page--Services--Applications-Implementation) <br>
      5.2.1. [Sprint 1](#Sprint-1) <br>
         5.2.1.1. [Sprint Planning 1](#Sprint-Planning-1) <br>
         5.2.1.2. [Sprint Backlog 1](#Sprint-Backlog-1) <br>
         5.2.1.3. [Development Evidence for Sprint Review](#Development-Evidence-for-Sprint-Review) <br>
         5.2.1.4. [Testing Suite Evidence for Sprint Review](#Testing-Suite-Evidence-for-Sprint-Review) <br>
         5.2.1.5. [Execution Evidence for Sprint Review](#Execution-Evidence-for-Sprint-Review) <br>
         5.2.1.6. [Services Documentation Evidence for Sprint Review](#Services-Documentation-Evidence-for-Sprint-Review) <br>
         5.2.1.7. [Software Deployment Evidence for Sprint Review](#Software-Deployment-Evidence-for-Sprint-Review) <br>
         5.2.1.8. [Team Collaboration Insights during Sprint](#Team-Collaboration-Insights-during-Sprint) <br>
      5.2.2. [Sprint 2](#Sprint-2) <br>
         5.2.2.1. [Sprint Planning 2](#Sprint-Planning-2) <br>
         5.2.2.2. [Sprint Backlog 2](#Sprint-Backlog-2) <br>
         5.2.2.3. [Development Evidence for Sprint Review](#Development-Evidence-for-Sprint-Review-2)<br> 
         5.2.2.4. [Testing Suite Evidence for Sprint Review](#Testing-Suite-Evidence-for-Sprint-Review-2) <br>
         5.2.2.5. [Execution Evidence for Sprint Review](#Execution-Evidence-for-Sprint-Review-2) <br>
         5.2.2.6. [Services Documentation Evidence for Sprint Review](#Services-Documentation-Evidence-for-Sprint-Review-2) <br>
         5.2.2.7. [Software Deployment Evidence for Sprint Review](#Software-Deployment-Evidence-for-Sprint-Review-2) <br>
         5.2.2.8. [Team Collaboration Insights during Sprint](#Team-Collaboration-Insights-during-Sprint-2) <br>
      5.2.3. [Sprint 3](#Sprint-3) <br>
         5.2.3.1. [Sprint Planning 3](#Sprint-Planning-3) <br>
         5.2.3.2. [Sprint Backlog 3](#Sprint-Backlog-3) <br>
         5.2.3.3. [Development Evidence for Sprint Review](#Development-Evidence-for-Sprint-Review-3) <br>
         5.2.3.4. [Testing Suite Evidence for Sprint Review](#Testing-Suite-Evidence-for-Sprint-Review-3) <br>
         5.2.3.5. [Execution Evidence for Sprint Review](#Execution-Evidence-for-Sprint-Review-3) <br>
         5.2.3.6. [Services Documentation Evidence for Sprint Review](#Services-Documentation-Evidence-for-Sprint-Review-3) <br>
         5.2.3.7. [Software Deployment Evidence for Sprint Review](#Software-Deployment-Evidence-for-Sprint-Review-3) <br>
         5.2.3.8. [Team Collaboration Insights during Sprint](#Team-Collaboration-Insights-during-Sprint-3) <br>
      5.2.4. [Sprint 4](#Sprint-4) <br>
         5.2.4.1. [Sprint Planning 4](#Sprint-Planning-4) <br>
         5.2.4.2. [Sprint Backlog 4](#Sprint-Backlog-4) <br>
         5.2.4.3. [Development Evidence for Sprint Review](#Development-Evidence-for-Sprint-Review-4) <br>
         5.2.4.4. [Testing Suite Evidence for Sprint Review](#Testing-Suite-Evidence-for-Sprint-Review-4) <br>
         5.2.4.5. [Execution Evidence for Sprint Review](#Execution-Evidence-for-Sprint-Review-4) <br>
         5.2.4.6. [Services Documentation Evidence for Sprint Review](#Services-Documentation-Evidence-for-Sprint-Review-4) <br>
         5.2.4.7. [Software Deployment Evidence for Sprint Review](#Software-Deployment-Evidence-for-Sprint-Review-4) <br>
         5.2.4.8. [Team Collaboration Insights during Sprint](#Team-Collaboration-Insights-during-Sprint-4) <br>
   5.3. [Validation & Testing](#Validation--Testing) <br>
      5.3.1. [Testing Plan](#Testing-Plan) <br>
      5.3.2. [Quality Assurance](#Quality-Assurance) <br>
      5.3.3. [User Acceptance Testing (UAT)](#User-Acceptance-Testing-UAT) <br>
   5.4. [Product Deployment](#Product-Deployment) <br>
      5.4.1. [Deployment Plan](#Deployment-Plan) <br>
      5.4.2. [Deployment Process](#Deployment-Process) <br>
      5.4.3. [Post-Deployment Review](#Post-Deployment-Review) <br>
6. [CAPÍTULO VI: Appendix](#Capítulo-VI-Appendix) <br>
   6.1. [References](#References) <br>
   6.2. [Glossary](#Glossary) <br>
   6.3. [Acronyms](#Acronyms) <br>
   6.4. [Bibliography](#Bibliography)<br>
   # STUDENT OUTCOME
El curso contribuye al cumplimiento del Student Outcome ABET: 
##### ABET – EAC - Student Outcome 3 
Criterio: Capacidad de comunicarse efectivamente con un rango de audiencias. En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 3. 

| **Criterio específico** | **Acciones realizadas** | **Conclusiones** |
|-------------------------|------------------------|------------------|
| Comunica oralmente con efectividad a diferentes rangos de audiencia. |                        |                  |
| Comunica por escrito con efectividad a diferentes rangos de audiencia. |                        |                  |
# CAPÍTULO I: Introducción
## Startup Profile
### Descripción de la Startup

#### Descripción General:

### Perfiles de integrantes del equipo

## Solution Profile
### Antecedentes y problemática

### Lean UX Process
#### Lean UX Problem Statements
#### Lean UX Assumptions
#### Lean UX Hypothesis Statements
#### Lean UX Canvas
### Segmentos objetivo
#### 1. Lectores Ávidos Particulares o Estudiantes:

Este segmento objetivo abarca a lectores apasionados y estudiantes que buscan acceder a una amplia variedad de libros y audiolibros, ya sea por interés personal o para cumplir con sus obligaciones académicas. Estos usuarios valoran la accesibilidad, la diversidad de títulos, y la posibilidad de personalizar su experiencia de lectura. Además, están interesados en interactuar con otros lectores a través de reseñas y comunidades en línea que enriquecen su experiencia literaria.


#### 2. Instituciones Educativas:
El segundo segmento objetivo incluye a instituciones educativas, editoriales y autores independientes que desean distribuir sus obras o recursos educativos de manera más eficiente y llegar a un público más amplio. Estos actores valoran una plataforma que les permita gestionar sus contenidos de forma digital y mantener un control sobre su distribución, con la posibilidad de obtener ingresos a través de suscripciones o ventas directas. Además, les interesa participar en una comunidad donde puedan interactuar con lectores, recibir feedback, y promover sus obras.


####  Variable geográfica:

País: Perú
Ciudad: Zonas urbanas y suburbanas
    
Variable demográfica:

Género: Femenino / Masculino
Ocupación: Estudiantes, lectores, instituciones educativas, editores, autores independientes
Estado civil: Todos los estados
Edad y etapa del ciclo de vida: Ciudadanos mayores de 15 años

#### Variable psicográfica:

Nivel Socioeconómico (NSE): Todos los niveles socioeconomicos
Características de personalidad: Curiosidad, deseo de aprendizaje continuo, aprecio por la lectura, compromiso con la educación y el desarrollo personal.

# Capítulo II: Requirements Elicitation & Analysis
## Competidores
BookSphere enfrenta competencia de plataformas como Google Play Books, Audible y Scribd. Google Play Books proporciona una amplia gama de libros electrónicos y audiolibros, pero carece de una componente social. Audible, especializado en audiolibros, ofrece una gran biblioteca y buena integración con dispositivos Amazon, aunque no cuenta con funciones comunitarias. Scribd ofrece acceso ilimitado a diversos contenidos digitales bajo suscripción, pero su interacción social es limitada. A diferencia de estos competidores, BookSphere destaca por integrar una comunidad literaria activa, permitiendo a los usuarios compartir reseñas y participar en discusiones, lo que enriquece la experiencia del usuario.
## Análisis Competitivo
<table>
   <tr>
      <td align="center" colspan="6">Competitive Analysis Landscaspe</td>
   </tr>
   <tr>
      <td colspan="2">¿Porqué llevar a cabo este análisis?</td><td colspan="4">¿Cómo podemos proporcionar un buen servicio entre los restaurantes y los consumidores de manera que la comunicación entre ambos sea efectiva y agradable?</td>
   </tr>
   <tr align="center">
      <td colspan="2"><td>SphereHub<br><img src="https://hackmd.io/_uploads/S15TtAi90.jpg" alt="Google Play Books" style="max-width: 80px;"/></td><td>Google Play Books<br><img src="https://hackmd.io/_uploads/SkbrwAo5A.jpg" alt="Google Play Books" style="max-width: 80px;"/></td><td>Audible<br><img src="https://hackmd.io/_uploads/S191dAo5C.png" alt="Audible" style="max-width: 80px;"/></td><td>Scribd<br><img src="https://hackmd.io/_uploads/SJ4_u0i9R.png" alt="Audible" style="max-width: 90px;"/></td>
   </tr>




   <tr>
      <td rowspan="2">Perfil</td><td>Overview</td><td> SphereHub es una empresa emergente que, a través de BookSphere, busca revolucionar el acceso a libros y recursos educativos digitales. Integrando una experiencia inmersiva y social, BookSphere se posiciona como una plataforma integral para estudiantes y lectores que desean descubrir, interactuar y compartir conocimientos.	 </td><td>Google Play Books ofrece un extenso catálogo de libros digitales y audiolibros, con opciones de compra y alquiler directamente en la plataforma de Google.</td><td> Audible, una subsidiaria de Amazon, se especializa en audiolibros y contenido de audio, ofreciendo una vasta colección de títulos y suscripciones.</td><td> Scribd es un servicio de suscripción que ofrece acceso a una vasta biblioteca digital de libros, audiolibros, documentos y más. Su modelo de suscripción todo en uno lo convierte en una opción popular para consumidores de contenido digital. </td>
   </tr>
   <tr>
      <td>Ventaja competitiva. ¿Qué valor ofrece a los clientes?</td><td> BookSphere se diferencia por combinar el acceso a libros con una comunidad interactiva, similar a la experiencia de Steam, donde los usuarios pueden dejar reseñas, comentarios y participar en foros relacionados con la literatura.</td><td> Google Play Books ofrece una integración nativa con Android, y su modelo permite a los usuarios comprar títulos específicos sin necesidad de suscripción.</td><td> Audible cuenta con una extensa selección de audiolibros exclusivos y la integración con dispositivos Amazon, como Alexa, lo que mejora la experiencia del usuario.	 </td><td> Scribd ofrece un acceso ilimitado a su biblioteca por una suscripción mensual, cubriendo una amplia gama de géneros y formatos.	 </td>
   </tr>
   <tr>
      <td rowspan="2">Perfil de Marketing</td><td>Mercado Objetivo</td><td>  Nos enfocamos en lectores apasionados y estudiantes que buscan una plataforma digital intuitiva para acceder a libros, audiolibros y recursos educativos. Además, nuestro objetivo es colaborar con editoriales, autores independientes e instituciones educativas que desean distribuir sus obras de manera innovadora y llegar a un público más amplio. </td><td> Usuarios de dispositivos Android que buscan conveniencia en la adquisición de contenido digital.
 </td><td> Consumidores que prefieren la experiencia auditiva para leer, incluyendo profesionales y entusiastas de la literatura.	 </td><td> Lectores generales que consumen una variedad de contenido digital, desde libros hasta revistas y documentos.	 </td>
   </tr>
   <tr>
      <td>Estrategias de Marketing</td><td> SphereHub planea enfocarse en campañas digitales dirigidas a instituciones educativas y crear alianzas estratégicas con editoriales y universidades. Además, promoverá la plataforma en redes sociales y a través de influencers literarios.	 </td><td> Google Play Books se apoya en la preinstalación en dispositivos Android y en su visibilidad dentro del ecosistema Google para llegar a un público amplio.
 </td><td> Audible invierte en campañas de marketing masivas, especialmente a través de Amazon y dispositivos Alexa, destacando su oferta de prueba gratuita y su contenido exclusivo.	 </td><td> Scribd apuesta por publicidad online y alianzas con creadores de contenido. También se enfoca en la retención mediante recomendaciones personalizadas y una experiencia sin interrupciones.	 </td>
   </tr>
   <tr>
      <td rowspan="3">Perfil de Producto</td><td>Productos & Servicios</td><td> Acceso a una amplia variedad de libros, audiolibros, y recursos educativos, junto con funcionalidades sociales para mejorar la interacción y el descubrimiento de contenido.	 </td><td> Libros digitales, audiolibros, revistas.
 </td><td> Audiolibros, podcasts, contenido exclusivo.	 </td><td> Libros, audiolibros, documentos, artículos, revistas.	 </td>
   </tr>
   <tr>
      <td>Precios & Costos</td><td> Ofreceremos un modelo flexible similar al de Steam, pero centrado en libros y audiolibros, con opciones de compra individual y suscripciones que permiten a los usuarios acceder a una vasta colección de contenido digital. </td><td> Compra individual de títulos.
 </td><td> Suscripción mensual para un crédito mensual, con opciones de compra adicional.	 </td><td> Suscripción mensual con acceso ilimitado.	 </td>
   </tr>
   <tr>
      <td>Canales de distribución (Web y/o Móvil)</td><td> Disponible en la web y como app móvil, con sincronización de progreso en múltiples dispositivos.	 </td><td> Web, iOS, Android. </td><td> Web, iOS, Android, dispositivos Alexa.	 </td><td> Web, iOS, Android, Kindle.	
 </td>
   </tr>

   <tr>
      <td rowspan="5">Análisis SWOT</td><td>Fortalezas</td><td> Comunidad interactiva, integración de funcionalidades sociales, enfoque en estudiantes y lectores serios.	 </td><td> Gran alcance y facilidad de acceso a través de dispositivos Android y Google.
 </td><td> Gran selección de contenido exclusivo y alto enfoque en la experiencia auditiva.	 </td><td> Acceso ilimitado a una biblioteca extensa por una tarifa plana.	 </td>
   </tr>
   <tr>
      <td>Debilidades</td><td> Dependencia inicial de alianzas estratégicas para construir una biblioteca robusta.	 </td><td> Competencia con otras plataformas de Google en el mismo ecosistema. </td><td> Alto costo si el usuario desea más de un libro al mes.	 </td><td> Puede saturarse el contenido debido a la amplitud de la biblioteca.	 </td>
   </tr>
   <tr>
      <td>Oportunidades</td><td> Crecimiento en el sector educativo, expansión a mercados internacionales, adopción de tecnologías emergentes.	 </td><td> Expansión en mercados donde Android es dominante. </td><td> Creciente popularidad de los audiolibros y podcasts.	 </td><td> Expansión a otros mercados verticales, como educación.	 </td>
   </tr>
   <tr>
      <td>Amenazas</td><td> Competencia fuerte en el mercado de libros digitales, barreras tecnológicas para la expansión en comunidades sin acceso a internet de alta calidad.	 </td><td> Competencia dentro del propio ecosistema de Google y otras apps con modelos más atractivos. </td><td> Nuevos jugadores en el mercado de audiolibros o cambios en las preferencias de consumo.	 </td><td> Competencia con plataformas de distribución más grandes, como Amazon.	 </td>
   </tr>

</table> 

<br/>


## Estrategias y tácticas frente a competidores
BookSphere VS Audible, Scribd, Google Play Books

### Estrategias:

Diferenciación: BookSphere se diferencia al ofrecer una plataforma interactiva que combina el acceso a libros, audiolibros y recursos educativos con características sociales, como la posibilidad de compartir reseñas, comentarios, y participar en comunidades de lectores. Esta integración de contenido y red social crea una experiencia de usuario única que no se encuentra en los competidores tradicionales.

Enfoque en el usuario: BookSphere se enfoca en entender las preferencias y comportamientos de sus usuarios, personalizando la experiencia de navegación y recomendación de libros y recursos. A través de algoritmos avanzados, la plataforma adaptará su contenido para ofrecer recomendaciones relevantes, manteniendo a los usuarios comprometidos y leales a la plataforma.

Alianzas estratégicas: BookSphere buscará establecer colaboraciones con editoriales, autores independientes y entidades educativas para expandir su catálogo digital. Además, creará alianzas con influencers y comunidades de lectores online para promover la plataforma y atraer a nuevos usuarios, generando un efecto de red que fortalezca su posición en el mercado.

### Tácticas:

Mejora tecnológica constante: BookSphere implementará mejoras continuas en su plataforma utilizando tecnologías avanzadas, como inteligencia artificial para recomendaciones personalizadas, análisis de comportamiento del usuario, y características de gamificación para fomentar la interacción dentro de la comunidad. También se actualizarán las opciones de lectura y escucha, como modos offline y sincronización entre dispositivos.

Análisis de la competencia: BookSphere realizará un análisis constante de los movimientos y estrategias de competidores como Audible, Scribd, y Google Play Books. Este análisis permitirá ajustar las tácticas de marketing y producto, asegurando que BookSphere se mantenga a la vanguardia en términos de innovación y satisfacción del usuario.

Integración de la comunidad: BookSphere se centrará en fortalecer su componente de red social, incentivando la participación de los usuarios a través de desafíos de lectura, clubes de lectura virtuales, y eventos en línea. La plataforma también ofrecerá incentivos, como acceso anticipado a nuevos títulos o descuentos en membresías, para usuarios activos y comprometidos en la comunidad.
## Entrevistas
Esta sección del informe abordará los aspectos objetivos de las entrevistas, incluyendo las preguntas realizadas, y ofrecerá un análisis detallado de cada una de ellas.
## Diseño de entrevistas
## Preguntas principales: 
## Registro de entrevistas
### Segmento: Estudiantes

### Análisis de entrevistas
    
#### Entrevista 1
| **Datos del entrevistado** | 
|--------------------------|
| **Nombre:**  Saico Gonzales José Fernando |
| **Edad:**  19 años |
| **Procedencia:**  Lima, Carabayllo |
| ![Entrevista1](https://hackmd.io/_uploads/HkebyaCqC.png)|
| **Resumen:** José Gonzales, estudiante que utiliza libros y audiolibros digitales al menos dos o tres veces por semana, valora una amplia variedad de títulos y una interfaz intuitiva en las plataformas. Prefiere combinar libros para estudios y audiolibros para actividades multitarea. Descubre nuevos libros a través de recomendaciones y reseñas, y busca funciones como listas de lectura personalizadas y recordatorios de lectura en las plataformas. Aprecia la personalización de recomendaciones y le gustaría interactuar con autores. Sin embargo, encuentra que la interacción en plataformas actuales a veces es limitada y desea mejoras en la interactividad y organización de las plataformas.  . |
## Needfinding
### User Personas
### User Task Matrix
### User Journey Mapping
### Empathy Mapping
### As-is Scenario Mapping
## Ubiquitous Language
# Capítulo III: Requirements Specification
## To-Be Scenario Mapping
texto
## User Stories
texto
## Impact Mapping
texto
## Product Backlog
texto
# Capítulo IV: Product Design
## Style Guidelines
### General Style Guidelines
texto
### Web Style Guidelines
texto
## Information Architecture
### Organization Systems
texto
### Labeling Systems
texto
### SEO Tags and Meta Tags
texto
### Searching Systems
texto
### Navigation Systems
texto
## Landing Page UI Design
### Landing Page Wireframe
texto
### Landing Page Mock-up
texto
## Web Applications UX/UI Design
### Web Applications Wireframes
texto
### Web Applications Wireflow Diagrams
texto
### Web Applications Mock-ups
texto
### Web Applications User Flow Diagrams
texto
## Web Applications Prototyping
texto
## Domain-Driven Software Architecture
### Software Architecture Context Diagram
texto
### Software Architecture Container Diagrams
texto
### Software Architecture Components Diagrams
texto
## Software Object-Oriented Design
### Class Diagrams
texto
### Class Dictionary
texto
## Database Design
### Database Diagram
texto
# Capítulo V: Product Implementation, Validation & Deployment
## Software Configuration Management
### Software Development Environment Configuration
texto
### Source Code Management
texto
### Source Code Style Guide & Conventions
texto
### Software Deployment Configuration
texto
## Landing Page, Services & Applications Implementation
### Sprint 1
#### Sprint Planning 1
texto
#### Sprint Backlog 1
texto
#### Development Evidence for Sprint Review
texto
#### Testing Suite Evidence for Sprint Review
texto
#### Execution Evidence for Sprint Review
texto
#### Services Documentation Evidence for Sprint Review
texto
#### Software Deployment Evidence for Sprint Review
texto
#### Team Collaboration Insights during Sprint
texto
### Sprint 2
#### Sprint Planning 2
texto
#### Sprint Backlog 2
texto
#### Development Evidence for Sprint Review
texto
#### Testing Suite Evidence for Sprint Review
texto
#### Execution Evidence for Sprint Review
texto
#### Services Documentation Evidence for Sprint Review
texto
#### Software Deployment Evidence for Sprint Review
texto
#### Team Collaboration Insights during Sprint
texto
### Sprint 3
#### Sprint Planning 3
texto
#### Sprint Backlog 3
texto
#### Development Evidence for Sprint Review
texto
#### Testing Suite Evidence for Sprint Revie
texto
#### Execution Evidence for Sprint Review
texto
#### Services Documentation Evidence for Sprint Review
texto
#### Software Deployment Evidence for Sprint Review
texto
#### Team Collaboration Insights during Sprint
texto
### Sprint 4
#### Sprint Planning 4
texto
#### Sprint Backlog 4
texto
#### Development Evidence for Sprint Review
texto
#### Testing Suite Evidence for Sprint Review
texto
#### Execution Evidence for Sprint Review
texto
#### Services Documentation Evidence for Sprint Review
texto
#### Software Deployment Evidence for Sprint Review
texto
#### Team Collaboration Insights during Sprint
texto
## Validation Interviews
### Diseño de Entrevistas
texto
### Registro de Entrevistas
texto
### Evaluaciones según heurísticas
texto
## Video About-the-Product
texto
# Conclusiones
## Conclusiones y recomendaciones
texto
## Video About-the-Team
texto

# Bibliografía
texto
# Anexos
texto

