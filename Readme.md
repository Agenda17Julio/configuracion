# Pasos para ejecutar el proyecto
## Primero que nada descargar los repositorios


[Repositorio Backend](https://github.com/Agenda17Julio/agenda17Backend)
[Repositorio Frontend](https://github.com/Agenda17Julio/agenda17Backend)



## Seguir los siguiente pasos

- Descargar docker en el droplet o servidor
- Descargar docker-compose en el droplet o servidor
- Descargar los 2 repositorios( frontend y backend en la misma carpeta con estos nombres ) 
- No olvides configurar las variables de entorno para el backend.

**Nota:** Recuerda que todos los archivos deben estar en la misma carpeta siguiente este orden.
```
> appProject
    > backend
    > frontend
    > .gitignore
    > .docker-compose.yml
    > package.json
    > package.lock.json
    > Readme.md
```

 ´

---
## Ambiente Sin docker

Si deseas ejecutar la aplicación sin necesidad de instalar docker lo unico que tienes que hacer es ejecutar los siguientes comandos, ubicado en la raíz del proyecto.

instala todas las dependencias funcionales.
``
    npm run init
``

construye los archivos binarios para producción.
``
    npm build
``

inicializa el servidor backend
``
    npm start
``

´

---
## Docker

Una vez que tengas instalado docker y docker compose lo siguiente es ejecutar el demonio de docker-compose

``
docker-compose up -d
``

Si todo sale bien lo siguiente es verificar el estado del contenedor
``
docker ps
``

Si el contenedor esta OK entonces puedes acceder a tu navegador con la dirección ip del servidor.


```sh
npm init
npm build
docker-compose up -d
docker ps
```