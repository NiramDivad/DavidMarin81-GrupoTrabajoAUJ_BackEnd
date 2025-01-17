# GrupoTrabajoAUJ_BackEnd
Proyecto de API RESTful para el proceso de selección de "Grupos de trabajo" de <a href="https://adoptaunjunior.es/" target="_blank">Adopta un Junior</a>

## Motivación
<details>
  <summary>Descripción</summary>
    <ul>
        <li>
        Con esta aplicación puedes agregar tus propias citas motivacionales, las cuales se muestran en una lista personalizada. Cada motivación puede ser editada o eliminada según lo desees.
        </li>
        <li>Características principales:</li>
            <ul>
                <li><b>Añadir motivaciones</b>: introduce tus frases motivadoras favoritas en la aplicación</li>
                <li><b>Lista personalizada</b>: visualiza todas tus motivaciones en una lista fácil de navegar</li>
                <li><b>Edición y Eliminación</b>: modifica y borra motivaciones en cualquier momento para mantener tu lista actualizada</li>
            </ul>
        <i>* Este proyecto es una demostración de mis habilidades en desarrollo backend utilizando Java y Spring Boot. Fue creado como parte del proceso de selección para los grupos de trabajo de <a href="https://adoptaunjunior.es/" target="_blank">Adopta un Junior</a>
        en BackEnd. La aplicación es una API RESTful que permite operaciones CRUD sobre un recurso de "Motivaciones", utilizando una base de datos H2 en memoria para el almacenamiento</i>
        </li>
    </ul>
</details>

<details>
  <summary>Tecnologías utilizadas</summary>
    <ul>
        <li><b><u>Java</u></b>: Lenguaje de programación para el desarrollo del backend.</li>
        <li><b><u>Spring Boot</u></b>: Framework para facilitar la creación de aplicaciones web en Java</li>
        <li><b><u>Spring Data JPA</u></b>: Abstracción para la interacción con bases de datos</li>
        <li><b><u>H2 Database</u></b>: Base de datos en memoria para el desarrollo</li>
        <li><b><u>Maven</u></b>: Herramienta de gestión de proyectos y dependencias</li>
    </ul>
</details>

<details>
  <summary>Características</summary>
    <ul>
        <li>CRUD Completo: Gestión de motivaciones mediante operaciones CRUD (Crear, Leer, Actualizar y Eliminar)</li>
        <li>API RESTful: Implementación de endpoints HTTP para interactuar con el recurso "Motivation"</li>
        <li>Base de Datos en Memoria: Uso de H2 para simplificar la persistencia de datos durante el desarrollo</li>
    </ul>
</details>

## Instalación y Ejecución
- Sigue estos pasos para configurar y ejecutar la aplicación en tu entorno local:
    - Clonar el repositorio
        ~~~bash
        git clone https://github.com/DavidMarin81/DavidMarin81-GrupoTrabajoAUJ_BackEnd
        cd GrupoTrabajoAUJ_BackEnd
        ~~~

    - Construir el proyecto- 
        ~~~bash
        # Asegúrate de tener Maven y Java instalados
        mvn clean install
        ~~~

    - Ejecutar la apliación
        ~~~bash
        mvn spring-boot:run
        ~~~
    - Prueba la app desde un navegador web:
        ~~~bash
        [mvn spring-boot:run](http://localhost:8080/)
        ~~~
    - Prueba la API sin un navegador web:
        - Puedes utilizar herramientas como **POSTMAN** para probar los endpoints de la API:
            ~~~bash
            # Obtener todas las motivaciones
            GET/motivations
            ~~~
            ~~~bash
            # Crear una nueva motivación
            POST/motivations
            ~~~
            ~~~bash
            # Obtener una motivación por ID
            GET/motivations/{id}
            ~~~
            ~~~bash
            # Actualizar una motivación existente
            PUT/motivations/{id}
            ~~~
            ~~~bash
            # Eliminar una motivación
            DELETE/motivations/{id}
            ~~~
        - Ejemplo para introducir datos:
        ![image](https://github.com/user-attachments/assets/50d48e48-c3ba-47c4-bf4a-22edb3c70e9c)
        - Ejemplo para obtener todas las motivaciones:
        ![image](https://github.com/user-attachments/assets/dee31b8a-95d7-4c98-9c49-324691457ead)
    - Uso de la base de datos H2
        - Accede a la consola de H2 para inspeccionar la base de datos en 
            ~~~bash
            http://localhost:8080/h2-console
            ~~~

            JDBC URL
            ~~~bash
            jdbc:h2:mem:testdb
            ~~~

            Username
            ~~~bash
            root
            ~~~

            Password
            ~~~bash
            abc123.
            ~~~
