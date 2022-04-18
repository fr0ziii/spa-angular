# Este proyecto consiste en la implementación de una aplicación SPA a través de Angular

![main](https://user-images.githubusercontent.com/58311234/163860823-81f2e3f9-5a58-4abe-8b6c-6d25c0e49fb6.PNG)

# Estructura de la aplicación

Al iniciar la aplicación, la ventana principal  te dirige a la ruta '/add-student' qué es desde donde añadimos los estudiantes a la base de datos.

![sidenav](https://user-images.githubusercontent.com/58311234/163860862-afacb4fc-7f46-414c-92e1-8e02fdcbf93e.PNG)

Tenemos dos opciones en el menú contextual del lado derecho:
   Añadir estudiante: Nos dirige a la ruta '/add-student', desde donde podemos añadir un estudiante
   
   ![anadir](https://user-images.githubusercontent.com/58311234/163861069-4e4565e3-9161-4aab-a612-0ed2157549a0.PNG)

   Ver estudiantes: Nos dirige a la ruta '/students-list', desde donde podemos ver todos los estudiantes que se encuentran en la base de datos y para cada estudiante, la opción de "Editar" o "Borrar".
   
   ![lista_estudiantes](https://user-images.githubusercontent.com/58311234/163861076-50368b39-a5d9-4e23-b0ed-ebd68dd24089.PNG)

A su vez, si hacemos clic en el título de la barra de navegación ("SPA con Angular") nos mostrará una alerta en el navegador y a la vez nos redigirirá a la ruta '/students-list'.

Si hacemos clic en el icono derecho de la barra de navegación, podemos mostrar/ocultar el menú contextual derecho.

Para editar un estudiante, debemos dirigirnos a la vista de "Lista de Estudiantes', y hacer clic en 'Editar', este botón nos llevará a la ruta '/edit-student'.

Para borrar un estudiante, debemos dirigirnos a la vista de "Lista de Estudiantes', y hacer clic en 'Borrar', este botón nos enviará una alerta para confirmar si estamos seguros de borrar.

# SPA con Angular

Este proyecto ha sido generado con [Angular CLI](https://github.com/angular/angular-cli) version 13.3.0.

## Iniciar la aplicación

Una vez descargado el repositorio, digirse al directorio principal y ejecutar el comando:  `npm i` 

Ejecuta la orden `ng serve` para el servidor de desarrollo. Dirigete a `http://localhost:4200/`. La aplicación se recargará automáticamente si cambias algunos de los ficheros fuente.

Para activar la base de datos y a su vez la API, debe de descargar y instalar MongoDB Compass.

(Descarga disponible en: `https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.6-signed.msi`)

1. Conectarse a su servidor de base de datos, y crear una base de datos con el nombre "users".

![mongodb_intro](https://user-images.githubusercontent.com/58311234/163861155-3b5a8a73-fcbf-4ae3-85ef-6f525143c0e2.PNG)

3. Dentro de "users", crear una colección llamada "students" que le permitirá almacenar los estudiantes de la aplicación.
4. 
![mongodb_2](https://user-images.githubusercontent.com/58311234/163861184-fc56f4d4-701d-4d6e-9bcc-5a3e1a3e9b82.PNG)

Una vez realizado los pasos anteriores, debe dirigirse a la carpeta 'backend' que se encuentra en el directorio principal
Y ejecutar estas órdenenes:

    `npm i
    npm i nodemon
    npx nodemon`.

Dentro del directorio principal, hay un archivo llamado "input.json" que sirve como prueba de datos para la API.

Para utilizarla ha de añadirla a la colección "students" de la base de datos "users".

Tras esto, dirigite a  `http://localhost:8000/api` y podrá ver los datos que están almacenado en la base de datos en formato JSON y a su vez sirve de API a la aplicación (añadir, editar, borrar).

## Build

Ejecuta `ng build` para construir el proyecto.

Este proyecto ha sido generado con [Angular CLI](https://github.com/angular/angular-cli) version 13.3.0.

## Autor

Este proyecto ha sido realizado por David Iglesias Guerra
