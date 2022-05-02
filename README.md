# ProLab

## Contents

- [Introducción](#introducción)
- [Requerimientos](#requerimientos)
  - [Requerimientos funcionales](#requerimientos-funcionales)
  - [Requerimientos no funcionales](#requerimientos-no-funcionales)
- [Herramientas usadas para la solución](#herramientas-usadas-para-la-solución)
- [Necesidad](#necesidad)
- [MER (Modelo Entidad Relación)](#mer-modelo-entidad-relación)
- [Arquitectura de software](#arquitectura-de-software)
- [Metodología usada](#metodología-usada)


## Introducción
Software de inventario en un laboratorio con elementos químicos

El presente trabajo tiene como objetivo presentar una propuesta de software al control y manejo de sustancias químicas en un laboratorio de detergentes de aseo. Este aplicativo de escritorio se desarrollará en C# y con una base de datos desarrollada en SQL. El proyecto se plantea como recurso de enseñanza y aprendizaje desde la unidad de estudio de Base de datos en la Universidad EAN dictada por el profesor Brayan Torres. Durante el diseño y desarrollo del proyecto se buscará de manera practica, implementar los conceptos de entidades, relaciones, consultas y acciones que tienen las bases de datos en un espacio como el inventario de sustancias químicas en un laboratorio de detergentes de aseo.

Adicionalmente el informe tendrá los requerimientos relacionados con los alcances del proyecto, el diseño de la interfaz, el modelo entidad relación, el código de la aplicación del escritorio, la metodología usada y los resultados obtenidos a partir de este.

# Requerimientos

[[Volver a tabla de contenido](#contents)]

## Requerimientos funcionales

<br>

[[Volver a tabla de contenido](#contents)]

<br>

| Número de requerimiento | RF001 |
| ------------------------------ | -----|
| Nombre de requerimiento | Modulo de control de inventario.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | La aplicación debe permitir el control del inventario de un operario acerca del material que se encuentra en un laboratorio químico.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF002 |
| ------------------------------ | -----|
| Nombre de requerimiento | Reporte de movimientos de salida y entrada de inventario.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | La aplicación debe permitir llevar el reporte de los movimientos de salida y entrada de los químicos que se manejan en el laboratorio.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF003 |
| ------------------------------ | -----|
| Nombre de requerimiento | Infraestructura de la aplicación |
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | La aplicación debe desarrollarse en Visual Basic con lenguaje de Python, para poder ser usada en sistemas operativos tales como Windows.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF004 |
| ------------------------------ | -----|
| Nombre de requerimiento | Disponibilidad de la aplicación. |
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | El sistema deberá funcionar las 24 horas del día y los 7 días a la semana para todos los usuarios.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF005 |
| ------------------------------ | -----|
| Nombre de requerimiento | Modulo de clasificación de sustancias químicas  en la aplicación.  |
| Tipo | Requisito |
| Fuente del requerimiento | Usuario |
| Proceso | El operario deberá usar la escala de peligrosidad ofrecida por la aplicación para realizar la respectiva clasificación de las sustancias químicas en el laboratorio.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF006 |
| ------------------------------ | -----|
| Nombre de requerimiento | Respaldo de datos |
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | Los datos de la aplicación deben respaldarse cada 24 horas en una ubicación segura a la cual solo tengan acceso usuarios autorizados.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF007 |
| ------------------------------ | -----|
| Nombre de requerimiento | Permisos del sistema. |
| Tipo | Restricción |
| Fuente del requerimiento | Administrador |
| Proceso | Los permisos para acceder al sistema solo podrán ser cambiados por el administrador de acceso a datos.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RF008 |
| ------------------------------ | -----|
| Nombre de requerimiento | Memoria |
| Tipo | Restricción |
| Fuente del requerimiento | Administrador |
| Proceso | La aplicación no podrá ocupar más de 5 GB de espacio en disco. |
| Prioridad del requerimiento | Media/Deseado |

## Requerimientos no funcionales

[[Volver a tabla de contenido](#contents)]

<br>

| Número de requerimiento | RNF001 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Usuario |
| Proceso | La aplicación debe ser intuitiva y fácil de usar por parte de los operarios de que controlan el inventario. Esta puede medirse con una encuesta de satisfacción.|
| Prioridad del requerimiento | Alta/Esencial |
<br>

| Número de requerimiento | RNF002 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Usuario |
| Proceso | La aplicación debe ser intuitiva y fácil de usar por parte de los operarios de que controlan el inventario. Esta puede medirse con una encuesta de satisfacción.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF003 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | En la aplicación deberá redactarse la descripción de las sustancias químicas que se almacenan en el laboratorio por parte de los operarios.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF004 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | El sistema deberá funcionar las 24 horas del día y los 7 días a la semana para todos los usuarios |
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF005 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Usuario |
| Proceso | El operario deberá usar la escala de peligrosidad ofrecida por la aplicación para realizar la respectiva clasificación de las sustancias químicas en el laboratorio.|
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF006 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | Los datos de la aplicación deben respaldarse cada 24 horas en una ubicación segura a la cual solo tengan acceso usuarios autorizados. |
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF007 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | Los permisos para acceder al sistema solo podrán ser cambiados por el administrador de acceso a datos. |
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF008 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | La aplicación no podrá ocupar más de 5 GB de espacio en disco. |
| Prioridad del requerimiento | Media/Deseado |

<br>

| Número de requerimiento | RNF009 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Requisito |
| Fuente del requerimiento | Administrador |
| Proceso | Cada uno de los productos contará con un identificador el cual permitirá que las consultas realizadas por el usuario sean eficientes. |
| Prioridad del requerimiento | Alta/Esencial |

<br>

| Número de requerimiento | RNF010 |
| ------------------------------ | -----|
| Nombre de requerimiento | Usabilidad de la aplicación.|
| Tipo | Restricción |
| Fuente del requerimiento | Usuario |
| Proceso | El sistema no permitirá revelar a usuarios no autorizados datos  de características específicas de los envíos o  números de contacto directo de los proveedores. |
| Prioridad del requerimiento | Alta/Esencial |


## Herramientas usadas para la solución.

[[Volver a tabla de contenido](#contents)]

## Necesidad

[[Volver a tabla de contenido](#contents)]

## Diseño de interfaz.

[[Volver a tabla de contenido](#contents)]

## MER (Modelo Entidad Relación)

[[Volver a tabla de contenido](#contents)]

## Arquitectura de software

[[Volver a tabla de contenido](#contents)]

El proyecto se basará en el Modelo Vista Controlador debido a su gran utilización en el mercado, esto se debe a que la estructura desarrollada por modulos, permite al desarrollador trabajar en paralelo sin afectar la operación del software.

Porlo tanto si un usuario desea navegar en una pagina y decide visualizar el estado de un producto, este relalizara una peticiòn directa a un controlador en especifico. Posteriormente este realizarà la solicitud con la secciòn modelo para que este a su vez realice una consulta a la base de datos.
Posteriormente se enviará la información al controlador y desde allí a la vista quien finalmente presentará la respuesta al usuario con la solicitud.

Unas de las caracteristicas y ventajas más destacadas de este modelo son:
- Fácil mantenimiento del código.
- Fácil de extender y crecer (facilidad de modificación).
- Los componentes del modelo MVC pueden ser probados por separado del usuario ya que todas las clases y objetos son independientes entre sí.

## Metodología usada.

[[Volver a tabla de contenido](#contents)]

Metodología de desarrollo.

Para el desarrollo de este proyecto haremos uso de conocimientos no solamente de la unidad de estudio sino de 
metodologías de gestión de proyectos Scrum – Agile con un componente KANBAN que nos permita 
seguimiento a las actividades y estará basado en desarrollo iterativo de 2 sprints con backlog.

Para establecer la estimación delas actividades y construir un backlog realizamos un sprint planning 
donde identificamos las actividades a realizar, refinamos las actividades y posteriormente 
realizaremos la estimación de acuerdo a las actividades definidas
Backlog preliminar.

Sprint 1:
<br><br>
• Definir plataforma de desarrollo
<br>
• Definir diseño de la aplicación 
<br>
• Hacer un prototipo de la web con el MVP definido
<br>
• Codificar solución
<br>
• Pruebas unitarias
<br>
• Pilotear
<br>
• Despliegue
<br>
• Testear prototipo y realizar ajustes si se requieren
<br><br>

Sprint 2:
<br><br>
• Definición de nuevas funcionalidades
<br>
• Prototipito de nuevas funcionalidades
<br>
• Testear prototipo y realizar ajustes si se requieren
<br>
• Codificar solución
<br>
• Pruebas unitarias
<br>
• Pilotear
<br>
• Despliegue
