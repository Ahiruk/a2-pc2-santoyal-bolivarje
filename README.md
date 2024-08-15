# a2-pc2-santoyal-bolivarje
Este proyecto contiene la solucion al siguiente problema:

Crear un ambiente con tres contenedores que ofrezcan servicios web, la distribución en la siguiente:

- Contenedor 1: proxy (algunas opciones son nginx y caddy), exponiendo el puerto 80

- Contenedor 2: aplicación web tomada de https://github.com/proyectosingenieriauninorte exponiendo el puerto 8000

- Contenedor 3: aplicación web tomada de https://github.com/proyectosingenieriauninorte exponiendo el puerto 8001

En el localhost se debe ver la página de bienvenida con links a los servicios, con el subdominio /c2 se debe ir a la página del contenedor 2 y con el subdominio /c3 al contenido del contenedor 3.

## Autores: 
- Luisa Fernanda Guzman Santoya
- Jorge Eduardo Bolivar Mojica
## Paso 1: Clonacion de los repocitorios
Primero clonamos los repositorios que iban a estar en nuestros contenedores 2 y 3
## Paso 2: Configuracion de Ngnix
La configuración de Nginx se encuentra en el archivo nginx.conf, este archivo define cómo se manejan las rutas para las aplicaciones web.
## Paso 3: Construccion del archivo docker-compose.yml
El archivo docker-compose.yml orquesta la construcción y ejecución de los tres contenedores:
## Paso 4: Construir y Ejecutar los Contenedores
Para construir y levantar los contenedores se usa:
docker-compose up --build
## Paso 5: Ajuste del html 
Para mejorar un poco la interfaz de usuario se hace uso de un archivo html, con stilos css

