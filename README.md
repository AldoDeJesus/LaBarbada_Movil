# Planeación del proceso de desarrollo de software - Movil 

El proyecto consiste en desarrollar una aplicación nativa para el restaurante La Barbada, que permitirá a los usuarios realizar pedidos de manera rápida y eficiente directamente desde sus dispositivos móviles. La aplicación ofrecerá notificaciones push y un rendimiento optimizado para móviles, proporcionando una experiencia fluida y accesible sin necesidad de acceder a un navegador web. Esto permitirá a los usuarios interactuar de forma más directa y cómoda con el restaurante a través de sus teléfonos.

## Tabla de Contenidos
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Objetivos del Proyecto](#objetivos-del-proyecto)
- [Riesgos y medidas para mitigarlos](#riesgos-y-medidas-para-mitigarlos )
- [Estrategia de comunicación](#estrategia-de-comunicación ) 
- [Metodología de Trabajo (Scrum)](#metodología-de-trabajo-scrum)
- [Herramienta para la gestión de issues](#herramienta-para-la-gestión-de-issues)
- [Control de Versiones](#control-de-versiones)
- [Revisión entre los Miembros del Equipo](#revisión-entre-los-miembros-del-equipo)
- [Flujo de Trabajo](#flujo-de-trabajo)
- [Estrategia de Versionamiento y Gestión de Ramas](#estrategia-de-versionamiento-y-gestión-de-ramas)
- [Creación Revisión y Fusión de Ramas](#creación-revisión-y-fusión-de-ramas)
- [Estrategia de Despliegue](#estrategia-de-despliegue)
- [Entornos](#entornos) 
- [Pila Tecnologica](#pila-tecnologica)
- [Instalación](#instalación)
- [Uso](#uso)


## Descripción del Proyecto
El proyecto consiste en desarrollar una aplicación nativa para el restaurante La Barbada, que permitirá a los usuarios realizar pedidos de manera rápida y eficiente directamente desde sus dispositivos móviles. La aplicación brindará una experiencia de usuario fluida y optimizada, facilitando la interacción con el restaurante de forma más directa y conveniente a través de sus teléfonos.


## Objetivos del Proyecto

### Objetivos

- Desarrollar una aplicación móvil complementaria a la página web existente, enfocada en mejorar la experiencia de los usuarios finales al permitirles realizar pedidos fácilmente desde sus dispositivos móviles.
- Ofrecer un proceso de compra rápido y eficiente para usuarios de dispositivos móviles.
- Proporcionar una nueva vía para realizar pedidos en cualquier momento y lugar desde dispositivos móviles.

### Alcance

- La aplicación estará destinada exclusivamente para los usuarios finales, es decir, clientes que desean realizar pedidos.
- Todas las funcionalidades administrativas (gestión de productos, pedidos, usuarios, etc.) continuarán gestionándose a través de la plataforma web.
- La aplicación móvil permitirá a los usuarios navegar por el menú del restaurante, personalizar pedidos y realizar pagos en línea.
- Se integrarán un apartado (pantalla) para mantener a los usuarios informados sobre el estado de sus pedidos.


## Riesgos y medidas para mitigarlos

## 1. Definición poco clara de requerimientos y objetivos
**Riesgo:** Si los objetivos del proyecto y los requerimientos no están bien definidos desde el inicio, esto puede generar malentendidos, cambios continuos y retrasos.  
**Medida de mitigación:**
- Asegurarse de tener un documento de especificaciones bien detallado.
- Usar metodologías ágiles (Scrum) para manejar cambios de requerimientos de manera flexible pero controlada.

## 2. Complejidad en la integración con el sistema web existente
**Riesgo:** Integrar la aplicación móvil con el sistema web de e-commerce ya existente (como bases de datos, APIs, back-end) puede ser complicado y llevar a problemas técnicos, errores o fallos.  
**Medida de mitigación:**
- Realizar una evaluación inicial de la arquitectura existente y planificar adecuadamente la integración de APIs.
- Utilizar herramientas de prueba automatizadas para asegurar que las integraciones funcionen correctamente antes de lanzarlas.
- Realizar pruebas para verificar el funcionamiento de APIs dentro de la aplicación.

## 3. Problemas de rendimiento y escalabilidad
**Riesgo:** La aplicación móvil puede experimentar problemas de rendimiento bajo carga, (por ejemplo, fallos en carga de contenido), afectando la experiencia del usuario.  
**Medida de mitigación:** Desarrollar y optimizar la aplicación para que funcione de manera eficiente en dispositivos móviles.

## 4. Problemas de seguridad y protección de datos
**Riesgo:** Dado que una aplicación de e-commerce maneja datos sensibles (métodos de pago), existe el riesgo de vulnerabilidades que podrían exponer esos datos a ataques o fraudes.  
**Medida de mitigación:**
- Implementación de pasarela de pago segura y confiable.
- Usar estándares de seguridad para las transacciones y almacenamiento de información.
- Asegurar que los datos de usuario y las transacciones sean almacenados correctamente.

## 5. Mala experiencia de usuario (UX/UI)
**Riesgo:** Una experiencia de usuario deficiente o una interfaz complicada para los usuarios finales.  
**Medida de mitigación:**
- Diseñar una interfaz intuitiva y adaptada a dispositivos móviles.
- Realizar pruebas de usabilidad con usuarios reales durante el desarrollo para identificar problemas en la experiencia del usuario.
- Mantener el diseño simple y optimizado para dispositivos de diferentes tamaños de pantalla.

## 6. Problemas de compatibilidad con dispositivos y sistemas operativos
**Riesgo:** La aplicación puede no funcionar correctamente en diferentes versiones de sistemas operativos (iOS/Android) o en dispositivos de diferentes resoluciones, lo que puede afectar a una parte significativa de los usuarios.  
**Medida de mitigación:**
- Usar herramientas de desarrollo multiplataforma como React Native para reducir la duplicación de código y asegurar la compatibilidad en diversas plataformas.
- Realizar pruebas en una variedad de dispositivos y emuladores para garantizar que la aplicación funcione correctamente en distintas versiones de los sistemas operativos y tamaños de pantalla.

## 7. Retrasos en el desarrollo y sobrecostos
**Riesgo:** La falta de control en los plazos y costos puede resultar en retrasos importantes, sobrecostos, y posible insatisfacción con el cliente.  
**Medida de mitigación:**
- Crear un cronograma claro con actividades definidas y utilizar metodologías ágiles para adaptarse a cambios sin comprometer plazos.
- Realizar revisiones constantes del proyecto y gestionar las expectativas con el cliente.
- Tener un presupuesto de contingencia y una planificación detallada de los recursos para evitar sobrecostos.

## 8. Malas prácticas de desarrollo y código no escalable
**Riesgo:** El uso de prácticas de desarrollo ineficientes puede llevar a código desorganizado, difícil de mantener o escalar a largo plazo.  
**Medida de mitigación:**
- Implementar revisiones de código y utilizar herramientas de control de versiones como Git.
- Asegurar una buena documentación del código.

## 9. Problemas de compatibilidad con pasarelas de pago
**Riesgo:** Integrar diferentes pasarelas de pago puede ser complejo y, si no se realiza correctamente, puede afectar la confianza de los usuarios o incluso generar errores en las transacciones.  
**Medida de mitigación:**
- Utilizar pasarelas de pago confiables y bien documentadas.
- Realizar pruebas exhaustivas de las pasarelas de pago en diferentes escenarios (tarjetas).
- Asegurarse de cumplir con las normativas de pago y manejar adecuadamente los fallos en las transacciones.

## Estrategia de comunicación 
## 1. Reuniones periódicas
- Realizar reuniones cada 2 semanas a través de **Google Meet** para:
  - Tratar problemas y revisar tareas pendientes.
  - Priorizar nuevas tareas y asignar roles y responsabilidades.
  - Proporcionar un resumen del progreso del proyecto.
  - Asegurar que todos los miembros del equipo estén informados.

## 2. Planificación y seguimiento con ClickUp
- Utilizar **ClickUp** como herramienta de gestión de tareas para:
  - Asignar y priorizar tareas.
  - Realizar un seguimiento del estado de cada tarea.

## 3. Uso de Git y GitHub para control de versiones
- Implementar **Git** y **GitHub** como herramientas de control de versiones.
- Utilizar **pull requests** para facilitar la comunicación entre los miembros del equipo sobre nuevas funcionalidades o correcciones de errores.

## Metodología de Trabajo (Scrum)
Se está utilizando la metodología **Agile Scrum** para gestionar y ejecutar el proyecto, lo que permite una entrega incremental del producto y la mejora continua a través de ciclos iterativos.

## Herramienta para la gestión de issues
Para la gestión de issues se ha decidido usar **ClickUp** como herramienta en los que hemos añadido a los integrantes y personas quienes revisaran las actividades. 

## Control de Versiones
El esquema de versionamiento usado para desarrollar el proyecto será a través de las tecnologías **Git** junto a **GitHub**, donde se tendrá un repositorio en el cual se encontrarán distintas ramas, siendo la principal la `main` o `master`, junto a 2 más (`Feature` y `Errors`), las cuales serán usadas cada una para abarcar distintas situaciones o casos:

- **Feature:** para nuevas características o nuevos requisitos.
- **Errors:** usado para atender errores específicos de distintos módulos o errores críticos que se tengan que aislar.

Asimismo, dichas tecnologías ayudarán al equipo a tener una copia del proyecto actualizada, además de poder realizar cambios entre ramas para no afectar directamente a la `master`, evitando realizar cambios indebidos. Esto también permite revertir cambios, fusionando ramas solo cuando los cambios hayan sido aprobados por el equipo.

## Revisión entre los Miembros del Equipo

- **GitHub** permite la colaboración eficaz mediante el uso de ramas, lo que permite que cada miembro del equipo pueda:
  - Realizar cambios.
  - Corregir errores.
  - Añadir nuevas características al proyecto sin afectar el código de producción.

- Se utilizarán **Pull Requests** para realizar cambios entre ramas, asignando a un revisor del equipo de desarrollo para que:
  - Revise y valide los cambios propuestos.
  - Comente y apruebe los cambios antes de integrarlos al código base.

## Flujo de Trabajo
El flujo de trabajo seleccionado es **GitHub Flow**, que se adapta a las características del proyecto y al tamaño del equipo, compuesto por 2 integrantes. Cada miembro está encargado de una rama dedicada a una tarea específica, como la corrección de errores o la implementación de nuevas funcionalidades. No se realizan cambios directos en la rama principal (**main**), lo que garantiza que solo se integre código estable.

## Estrategia de Versionamiento y Gestión de Ramas
La estrategia de versionamiento elegida es **GitHub Flow** debido a su simplicidad y adaptabilidad a un equipo pequeño. Las ramas están divididas de la siguiente manera:
- **Feature:** Ramas dedicadas a la corrección o cambios de funcionamiento basados en la retroalimentación del cliente. Incluye ajustes de diseño y funcionalidad.
- **Errores:** Rama dedicada a la identificación y corrección de errores de funcionamiento o mejoras en los componentes del proyecto.
- **Máster:** Rama por defecto, donde se fusionan los cambios realizados en las ramas anteriores después de pasar por revisión y pruebas.

## Creación Revisión y Fusión de Ramas
1. *Creacion* 
  * Para trabajar de manera eficiente y organizada, se recomienda crear ramas específicas para cada nueva característica o corrección de errores. Utiliza el siguiente comando para crear una nueva rama:

  ```bash
    git checkout -b nombre-de-la-rama
  ```
2. *Revision*
  * Una vez que se han realizado cambios en una rama, se debe enviar un Pull Request (PR) para iniciar la revisión del código
   1. Realiza un push de tu rama al repositorio remoto:
        ```bash
          git push origin nombre-de-la-rama
        ```
   2. Ve a GitHub y selecciona "Pull Requests".
   3. Haz clic en "New Pull Request"
   4. Selecciona tu rama y sigue las instrucciones para completar el PR.
   
3. *Fusión* 
  * Una vez que el Pull Request ha sido revisado y aprobado, puedes fusionar los cambios en la rama principal (main). Esto se puede hacer directamente en la interfaz de GitHub:
    1. Haz clic en el botón "Merge Pull Request" en la página del PR.
    2. Confirma la fusión.
  
  
## Estrategia de Despliegue
La estrategia seleccionada es **Despliegue Directo (Big Bang)** debido a que solo se cuenta con un servidor, y aunque conlleva riesgos, es una estrategia que permite realizar la implementación de la nueva versión del sistema de una sola vez. 
Algunas características clave de esta estrategia:
- Implementación de la nueva versión en todo el sistema de una vez.
- Menor complejidad en comparación con otras estrategias, ya que no requiere configurar múltiples entornos.
- Riesgos mitigados mediante pruebas exhaustivas en entornos de desarrollo antes del despliegue en producción.
- Apto para proyectos con un volumen de tráfico moderado y actualizaciones no frecuentes.

## Entornos

### Desarrollo

#### Gestión de tareas y planificación:
- **ClickUp:** usado para la gestión de proyectos y tareas, para planificar el desarrollo, asignar tareas, y gestionar el progreso.

#### Control de versiones:
- **Git + GitHub:** usado para manejar el control de versiones, colaborar en el código y gestionar revisiones mediante pull requests y ramas.

#### Entorno de desarrollo:
- **Visual Studio Code (VSCode):** como editor de código para React Native y Node.js. Soporte robusto para JavaScript/TypeScript y muchas extensiones útiles.

### Staging

#### Testing de móviles:
- **Expo:** usado para probar la aplicación móvil de React Native en diferentes dispositivos o simuladores para ver cómo se comporta en condiciones cercanas a producción.

### Producción
#### Servidor:
- **Hostinger:** usado para desplegar el backend en producción.


## Pila Tecnológica


- **Node.js**
  ![Node.js](https://lh3.googleusercontent.com/proxy/ULN9eqCb30WW559cJhquYsjR5GkhIEtt_NW0TRjzmwoX2tMs_FpOUWamTj-isgUwAa9W05VzndBMhBHnVnHiLM0QbA)

- **Express**
  ![Express](https://cdn.iconscout.com/icon/free/png-256/free-express-9-1175170.png)

- **React Native**
  ![React](https://cdn.prod.website-files.com/669eb1086f08fffc3efda56e/66b3adb6328800b9c05ea857_react_native_e0c7e12161.png)

- **MySQL**
  ![MySQL](https://www.mysql.com/common/logos/logo-mysql-170x115.png)



## Instalación
Sigue estos pasos para instalar y configurar el proyecto en tu entorno local.

1. Clona el repositorio:
    ```bash
    git clone https://github.com/EmmanuelR214/LaBarbada_Movil.git
    ```

2. Entra en el directorio del proyecto:
    ```bash
    cd LaBarbada_Movil
    ```

3. Instala las dependencias:
    ```bash
    npm install
    ```

4. Ejecuta el proyecto localmente:
    ```bash
    npm start
    ```

## Uso
Después de la instalación, puedes acceder a la aplicación en tu navegador en `http://localhost:3000`.
