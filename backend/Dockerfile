FROM node:18-alpine

WORKDIR /app

# Instalar dependencias primero 
COPY package*.json ./
RUN npm ci --omit=dev

# Copiar solo lo necesario
COPY . .

# Seguridad: no usar root
RUN addgroup -S app && adduser -S app -G app
USER app

EXPOSE 3000

CMD ["node", "src/server.js"]
