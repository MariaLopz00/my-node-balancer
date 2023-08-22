# Usar una imagen de Node.js
FROM node:14

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /usr/src/app/web1

# Copiar los archivos de la aplicación al contenedor
COPY package*.json ./
COPY . .

# Instalar las dependencias
RUN npm install express mysql2

# Exponer el puerto en el que la aplicación va a estar escuchando
EXPOSE 80

# Comando para iniciar la aplicación
CMD [ "node", "index.js" ]
