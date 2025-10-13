# FROM debian:buster-20240612-slim
FROM node:20.5.0-alpine3.18

RUN addgroup react && adduser -S -G react react
USER react

WORKDIR /app/
RUN mkdir datos
COPY --chown=react package*.json .
RUN npm install
COPY --chown=react . .

# COPY ["nombre fich con espacios.txt", .]
# ADD URL . # Descarga archivos desde una URL
# ADD fich.zip . # Ojo pq ADD descomprime los ZIPs en el destino

# RUN apk install php

ENV API=https://as.com

# ##### Esto es solo info!!! No expone el puerto realmente!!!
EXPOSE 5173


CMD ["npm", "run", "dev"]
