# indica a Docker que imagen instalará y su versión
FROM node:18

# indica a Docker que debe ejecutar un comando dentro del contenedor, en este caso, la ruta dentro del contenendor dónde debe crear un directorio para el proyecto
RUN mkdir -p /home/app

# indica a Docker que copie todos los archivos del proyecto dentro del directorio dónde estará el proyecto
COPY . /home/app

# indica a Docker en qué puerto se ejecutará la aplicación, debe coincidir con el indicado en la aplicación
EXPOSE 3000

# indica a Docker cuál comando ejecutará en la consola de Windows
CMD ["node", "/home/app/index.js"]
