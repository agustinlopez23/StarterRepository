FROM node:18-alpine

# Crear y usar el directorio de la app
WORKDIR /app

# Copiar package.json e instalar dependencias
COPY package*.json ./
RUN npm install

# Copiar el código fuente
COPY . .

# Compilar TypeScript
RUN npm run build

# Exponer el puerto
EXPOSE 4000

# Comando para iniciar el servidor
CMD ["npm", "run", "start"]
