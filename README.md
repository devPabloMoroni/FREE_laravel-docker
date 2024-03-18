<p align="center">
<img src="https://chatkitty.com/assets/images/feature-cbeb779dc53b732d404ab5c3d4c54940.png" alt="Vue Logo"  width="200">
<br>
<img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" alt="Laravel Logo" width="300">
<br>
<img src="https://aulasoftwarelibre.github.io/taller-de-pas/Sesion-1/images/horizontal-logo-monochromatic-white.png" alt="Docker Logo" width="400">
</div>



## Descripcion del Proyecto

Este repositorio contiene un CRUD básico desarrollado en Laravel, Vue.js y Docker, diseñado como parte de una prueba técnica. El proyecto proporciona una aplicación web para la gestión de datos mediante operaciones CRUD (Crear, Leer, Actualizar y Eliminar) sobre una base de datos.
#### Características principales
- **Tecnologías utilizadas:** El proyecto se basa en el framework PHP Laravel para el backend, Vue.js para el frontend y Docker para la gestión del entorno de desarrollo.
- **Operaciones CRUD:** Permite realizar operaciones de Crear, Leer, Actualizar y Eliminar sobre los datos almacenados en la base de datos.
- **Visualización de datos:** Incluye una sección para visualizar gráficos de barras que proporcionan una representación visual de la información almacenada en la base de datos.
- **Generación de reportes:** Dispone de una sección para obtener reportes con opciones para exportarlos en formatos Excel y PDF, imprimirlos, copiarlos al portapapeles, entre otros.
- **Arquitectura MVC:** Utiliza el patrón de diseño Modelo-Vista-Controlador (MVC) para organizar y estructurar el código de la aplicación.
- **Separación de responsabilidades:** Se hace uso de la separación de responsabilidades entre el backend (Laravel) y el frontend (Vue.js) para una mejor mantenibilidad y escalabilidad del proyecto.
- **Contenedores Docker:** Se incluye una configuración de Docker para facilitar la instalación y ejecución del proyecto en diferentes entornos sin la necesidad de configuraciones adicionales.

### Requerimientos
El proyecto fue realizado usando las siguientes versiones:
- PHP v8.1
- Node.js v20
- Composer v2.7
- Docker v25
- Docker-compose v2.24
- GIT v2.44
> [!TIP]
> Para una mayor compatibilidad utilizar las mismas versiones antes detalladas

### Instalación de paquetes necesarios
1. Instalar PHP [-->Go to](https://www.php.net/manual/es/install.php)
2. Instalar Node.js [-->Go to](https://nodejs.org/en/download)
3. Instalar Composer [-->Go to](https://getcomposer.org/download/)
4. Instalar Docker [-->Go to](https://docs.docker.com/engine/install/)
5. Instalar Docker-compose [-->Go to](https://docs.docker.com/compose/install/)
6. Instalar GIT [-->Go to](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git)

### Instalación del Repositorio
1. Abrir una terminal y clonar el repositorio
```git
git clone git@github.com:devPabloMoroni/FREE_laravel-docker.git
```
> [!WARNING]
> A partir de hace uno años no se permite clonar repositorios por HTTPS, si aparece algún problema con respecto a esto debes instalar los certificados SSH [Mirá como hacerlo!](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/about-ssh)

2. Moverse a la carpeta
```javascript
cd FREE_laravel-docker
```
3. Copiar el archivo `.env.example` a `.env` 
```javascript
cp .env.example .env
```
y configurar las variables de entorno de la base de datos de la siguiente manera:
```javascript
DB_CONNECTION=mysql
DB_HOST=DB
DB_PORT=3306
DB_DATABASE=laravuecompany
DB_USERNAME=root
DB_PASSWORD=
```
4. En el caso de usar nvm ejecutar:
```javascript
nvm install 20
```
```javascript
nvm use 20
```
5. Abrir una terminal dentro del proyecto y ejecutar:
```javascript
npm i
```
6. Configuración de Dependencias con Composer
```javascript
composer install
```
7. Inicialización de Entorno
```javascript
docker-compose up -d
```
8. Verificar nombre del contenedor de la app
```javascript
docker ps
```
9. Entrar al contenedor de la app
```javascript
docker exec -it APP sh
```
10. Crear KEY para proyecto
```javascript
php artisan key:generate
```
> [!WARNING]
> En el caso de que de algún error con el cache ejecutar `php artisan cache:clear`

11. Ejecutar migraciones
```javascript
php artisan migrate
```
12. Ejecutar Seeders
```javascript
php artisan migrate --seed
```
13. Salir del contenedor
```javascript
exit
```
14. Ejecutar npm desde el entorno local
```javascript
npm run dev
```
15. Acceder a la aplicacion desde tu navegador preferido
```javascript
http://localhost:8000/
```
16. Registrar tu usuario
17. Empezar a utilizar!
