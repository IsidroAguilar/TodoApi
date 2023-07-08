# TodoApi

Este proyecto es el quinto proyecto del curso de Desarrollo web en .NET Core y tiene como objetivo proporcionar una introducción a los conceptos básicos de la creación de una API web basada en controladores que utiliza una base de datos.

## Requisitos

- .NET Core SDK 
- Visual Studio
- SQL Server o cualquier otra base de datos compatible

## Instalación

1. Clona o descarga el repositorio del proyecto TodoApi.
2. Abre el proyecto en Visual Studio.

## Configuración de la base de datos

1. Crea una base de datos en tu servidor de base de datos. Puedes utilizar SQL Server u otra base de datos compatible.
2. Abre el archivo `appsettings.json` en el proyecto.
3. En la sección `"ConnectionStrings"`, actualiza el valor de `"DefaultConnection"` con la cadena de conexión a tu base de datos.

## Ejecución

1. Abre una terminal en el directorio raíz del proyecto.
2. Ejecuta el siguiente comando para restaurar las dependencias del proyecto:

   ```
   dotnet restore
   ```

3. Ejecuta el siguiente comando para compilar el proyecto:

   ```
   dotnet build
   ```

4. Ejecuta el siguiente comando para aplicar las migraciones y crear las tablas en la base de datos:

   ```
   dotnet ef database update
   ```

5. Ejecuta el siguiente comando para iniciar la API:

   ```
   dotnet run
   ```

La API estará disponible en la dirección `http://localhost:5000`.

## Uso

La API proporciona endpoints para realizar operaciones CRUD (crear, leer, actualizar y eliminar) en la entidad "Tarea". Puedes utilizar herramientas como Postman o cURL para interactuar con la API.

- Para obtener todas las tareas: `GET /api/tareas`
- Para obtener una tarea específica: `GET /api/tareas/{id}`
- Para crear una nueva tarea: `POST /api/tareas`
- Para actualizar una tarea existente: `PUT /api/tareas/{id}`
- Para eliminar una tarea: `DELETE /api/tareas/{id}`

## Contribución

Si deseas contribuir a este proyecto, puedes hacerlo siguiendo estos pasos:

1. Realiza un fork del repositorio.
2. Crea una rama para tu nueva funcionalidad (`git checkout -b nueva-funcionalidad`).
3. Realiza los cambios necesarios y realiza commit de tus cambios (`git commit -am 'Agrega nueva funcionalidad'`).
4. Sube tus cambios a tu repositorio remoto (`git push origin nueva-funcionalidad`).
5. Abre una solicitud de extracción en el repositorio original.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para obtener más detalles.

## Contacto

Si tienes alguna pregunta o sugerencia, no dudes en ponerte en contacto conmigo a través de mi correo electrónico: [isidro.aguilar94@gmail.com](mailto:isidro.aguilar94@gmail.com).

--- 

¡Gracias por utilizar TodoApi! Espero que este proyecto te ayude a comprender los conceptos básicos de la creación de una API web basada en controladores que utiliza una base de datos. Si tienes alguna pregunta o problema, no dudes en comunicármelo. ¡Disfruta del desarrollo web en .NET Core!
