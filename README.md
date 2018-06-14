## Dockerizando un App ASP.NET Core

Ejemplo de una aplicación ASP.NET Core dentro de un contenedor Docker utilizando la imagen *microsoft/aspnetcore-build:2.0.0*.

Se utiliza un segundo contenedor *nginx* para hacer un reverse proxy y acceder a Kestrel.

## Ejecutar el Proyecto

### Requerimientos Técnicos
- OS: Windows 10 Pro, macOS 10.12, Linux
- Docker
- IDE
    - Windows: Visual Studio 2017 Community
    - macOS: Visual Studio/Visual Studio Code/Sublime Text/VIm
    - Linux: Visual Studio Code/Sublime Text/VIm
- Tools:
    - .NET Core SDK

Una vez que tenemos el software instalado y clonado el proyecto, procederemos a construirlo en nuestro disco con el siguiente comando:
```
docker-compose build
```
Ten en cuenta que si es la primera vez que lo corres, se procederan a descargar las imagenes que se esten utilizando en el proyecto, esto tarda aproximadamente 10 minutos dependiento la conexión que tengas, luego ya no sera necesario, incluso si decides crear un proyecto nuevo.

Para correr:
```
docker-compose up
```

#### Autor
Gustavo Barrientos Guerrero [@tavobarrientos](http://www.github.com/tavobarrientos)