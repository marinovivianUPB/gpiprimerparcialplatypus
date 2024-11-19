---
theme: penguin
title: E-Learning - Platypus Sys. Inc.
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
layout: intro
---

# E-Learning by Platypus Sys. Inc.

Portal Web de E-Learning para ROMMOS S.R.L.

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <carbon:arrow-right class="inline"/>
  </span>
</div>

<!--
Buenos días a todos los presentes. Somos Platypus Systems Incorporated. Realizarmos un P
-->

---

# Tabla de Contenidos

<Toc minDepth="1" maxDepth="2"></Toc>

---
layout: new-section
---

# Plan de Proyecto

---
level: 2
---

# ¿Qué haremos en cada Fase?  
5 meses, aprox. 22 semanas

- 📝 **Inicio - Semanas 1 a 2**  
  Reunión inicial con ROMMOS S.R.L. para definir objetivos específicos, y funcionalidades principales (gestión de cursos, usuarios y noticias).  
  Identificación de partes interesadas y asignación de roles clave dentro de Platypus Systems y ROMMOS.  
  Recepción de la carta de aceptación y aprobación de los términos acordados en ella, que incluye límites, responsabilidades, costos, entre otros .  

- 🤹 **Planificación - Semanas 2 a 4**  
  Desarrollo del plan de proyecto detallado, alineado con la metodología SCRUM.    
  Selección y confirmación de tecnologías: frameworks para desarrollo frontend y backend.  
  Análisis y planificación de riesgos, incluyendo mitigación para dependencia de servicios externos (hosting, internet y base de datos de ROMMOS S.R.L.).

---

- 🎨 **Diseño - Semanas 3 a 6**  
Desarrollo de la identidad visual basada en la imagen corporativa de ROMMOS S.R.L.  
Creación de wireframes y mockups para las interfaces de usuario, como ser: página de inicio, sección de cursos y talleres, panel de usuario, noticias y contacto.  
Creación de diagramas UML de: casos de uso, clases, secuencia, actividades, componentes y estados.
Mockup de la funcionalidad de inscripción de usuarios con integración de tarjeta de crédito.  
Revisión y aprobación de los mockups por parte de ROMMOS, incluyendo iteraciones necesarias para ajustes.    

- 🧑‍💻 **Desarrollo - Semanas 5 a 18**  
Dividido en 7 Sprints de 2 semanas.  
Configuración inicial del hosting y conexión con la base de datos proporcionada por ROMMOS.  
Conexión a BudPay API para realizar cobros a tarjetas de crédito.  
Desarrollo de los módulos determinados:  
  - **Módulos Comunes**: Página de inicio, panel de usuario, login, sign-up con pasarela de pago, secciones de contacto y noticias (feedback en noticias), y menú de navegación.
  - **Módulos de Estudiante**: Sección de cursos y talleres (gestión de inscripciones, progreso y calificaciones).
  - **Módulos de Administrador**: Herramientas para gestionar cursos, gestionar inscritos, y publicar noticias.  

---

- 🛠 **Pruebas y Control de Calidad - Semanas 6 a 20**  
Pruebas de funcionalidad: Asegurar que todas las funcionalidades (módulos comunes, de estudiantes y de administradores) operan según lo planeado.  
Pruebas de rendimiento: Optimización del tiempo de carga y estabilidad para su uso exclusivo en computadoras y laptops.  
Pruebas de compatibilidad: Verificar comportamiento en navegadores compatibles.  
Resolución de problemas técnicos identificados durante las pruebas.  

- 📤 **Implementación - Semanas 17 a 20**  
Configuración del entorno de producción en el servidor de hosting seleccionado por ROMMOS.  
Despliegue de la plataforma en línea con un monitoreo inicial del desempeño.  
Implementación de ajustes finales según retroalimentación inicial tras el lanzamiento.

---

- 🌟 **Cierre - Semanas 19 a 22**  
Entrega formal del sistema a ROMMOS S.R.L., acompañado de manuales para usuarios y administradores.  
Capacitación: Asistencia al equipo de ROMMOS en el uso de las herramientas de gestión (cursos, noticias y usuarios).  
Documentación final del proyecto: detalles técnicos, configuraciones, y procedimientos de mantenimiento recomendados.  
Revisión de lecciones aprendidas entre los equipos de Platypus Systems y ROMMOS para proyectos futuros.  

- 🛡️ **Mantenimiento - 1 mes desde el Cierre**  
Soporte técnico inicial: Supervisión del sistema durante el primer mes posterior al lanzamiento para resolver errores no detectados en las pruebas.  
Actualizaciones menores: Ajustes en la interfaz o funcionalidad, según lo definido en la Carta de Aceptación y subsecuentes adendas.  
Documentación adicional: Registro de problemas reportados y soluciones implementadas.  

---
level: 2
---

# Diagrama de Gantt

<img
  src="./grantGPIEntrega1.png"
  alt=""
/>

---
level: 2
---

# Herramientas

|                                                    |                             |        |
| -------------------------------------------------- | --------------------------- |--------|
| Trello | Para organizar tareas y seguir el progreso | Todas las fases |
|  | de cada fase. |
| Discord | Para comunicación entre miembros del equipo | Todas las fases |
|  | y para realizar reuniones con los interesados del proyecto |
| Google Docs y Notion                               | Para mantener documentación actualizada y organizada | Todas las fases |
| Figma                | Para la creación de mockups, la definición | Diseño |
|  |  de la imagen del Portal Web y la creación de diagramas |

---

|                                                    |                             |        |
| -------------------------------------------------- | --------------------------- |--------|
| Github | Para el control de versiones y facilitar | Desarrollo |
|  | la colaboración entre los dessarrolladores del equipo |
| Vue.js | Framework de Javascript utilizado para desarrollar UI | Desarrollo |
| Express para Node.js | El framework Express se utilizará para la API y | Desarrollo |
|  | lógica de negocio. |
| CyberSource | Pasarela de pago que se utilizará | Desarrollo |
|  | para realizar los cobros por tarjeta de usuarios. |

---

|                                                    |                             |        |
| -------------------------------------------------- | --------------------------- |--------|
| Vitest | Para realizar las pruebas de UI en Vue.js | Pruebas y Control de Calidad |
| Mocha y Chai | Estos frameworks de Node.js se utilizarán | Pruebas y Control de Calidad |
|  | para realizar las pruebas del módulo Backend. |
| Cypress | Este framework de testing de Javascript | Pruebas y Control de Calidad |
|  | permitirá la realización de pruebas funcionales de UI |
| Jmeter | Herramienta de testeo que permite realizar | Pruebas y Control de Calidad |
|  | pruebas de carga, estrés y rendimiento |

---

|                                                    |                             |        |
| -------------------------------------------------- | --------------------------- |--------|
| AWS S3 | Para el despliegue del módulo Frontend | Implementación |
|  | se utilizará el servicio de almacenamiento AWS S3 |
| Heroku | Esta plataforma basada en la nube será | Implementación |
|  | utilizada para desplegar el módulo Backend |

---
level: 2
---

# Recursos

|                                                    |                             |
| -------------------------------------------------- | --------------------------- |
| Equipos (Hardware) | Computadoras portátiles adecuadas para diseño, desarrollo y pruebas para todos los miembros del equipo de Desarrolladores. Además, deben tener acceso a los servidores de ROMMOS S.R.L. para realizar la conexión con la base de datos y pode desplegar un ambiente de prueba antes de pasar al ambiente de producción.|
| Personal | - Desarrolladores Frontend con experiencia en desarrollo web con Vue.js |
|  | - Desarrolladores Backend con experiencia en desarrollo web con Node.js y Express |
|  | - Diseñador con experiencia en Figma y diseño de UI/UX |
|  | - Especialistas en Quality Assurance con experiencia en automatización de pruebas y familiarizados con los frameworks Mocha y Chai, Cypress y Vitest, además de la herramienta JMeter. |

---

|                                                    |                             |
| -------------------------------------------------- | --------------------------- |
| Personal | - Ingeniero en DevOps con certificación en Amazon Web Services y familiarizado con plataformas de despliegue como Heroku. |
| Información del Cliente | Detalles específicos de ROMMOS S.R.L., sus servicios y objetivos, así como acceso a cualquier material o sistema que deba integrarse en la plataforma, como ser la base de datos que contiene datos de estudiantes, administradores y cursos.|

---
level: 2
---

# Entregables

|                                                    |                             |
| -------------------------------------------------- | --------------------------- |
| Planificación | - Términos de Referencia |
|  | - Carta de Aceptación |
| Diseño | - Mockups |
| Pruebas y Control de Calidad | - Gestión de Riesgos |
|  | - Pruebas y Hosting |

---
layout: new-section
---

# Nuestro Equipo

---
level: 2
layout: presenter
presenterImage: './dylan.jpg'
---

# Dylan Jitton - Doctor D

- **Desarrollador Frontend y Backend**
- **Ingeniero DevOps**

---
level: 2
layout: presenter
presenterImage: './perry.jpg'
---

# Vivian Marino - Agente VMware

- **Desarrollador Frontend y Backend**
- **Especialista en Quality Assurance**

---
level: 2
layout: presenter
presenterImage: './perry.jpg'
---

# Luis Paricollo - Agente P

- **Líder de Proyecto** - Responsable de la planificación y supervisión de todas las fases
- **Desarrollador Backend**
- **Especialista en Quality Assurance**

---
level: 2
layout: presenter
presenterImage: 'https://res.cloudinary.com/alvarosaburido/image/upload/v1622370075/as-portfolio/alvaro_saburido.jpg'
---

# Katzumi Urdininea - Agente U

- **Diseñador de User Interface y User Experience**
- **Desarrollador Frontend**
