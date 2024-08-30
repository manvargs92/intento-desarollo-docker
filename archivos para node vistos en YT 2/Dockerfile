# indica a Docker que imagen instalará y su versión
FROM node:16
    
# indica a Docker en cual ruta posicionarse en dónde creará un directorio para la aplicación en el contenedor
WORKDIR /usr/src/app

# indica a Docker que copie el archivo package.json dentro de la ruta indicada en la líneade arriba
COPY package*.json ./

# indica a Docker que debe ejecutar un comando dentro del contenedor, en este caso npm install para que se instalen las dependencias
RUN npm install

# indica a Docker que copie todos los archivos del proyecto al contenedor (ruta-origen ruta-destino)
COPY . .

# indica a Docker en qué puerto se ejecutará la aplicación, debe coincidir con el indicado en la aplicación
EXPOSE 3000

# indica a Docker cuál comando ejecutará en la consola de Windows
CMD [ "node", "server.js" ]