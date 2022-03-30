ARG TAG=latest
FROM node:$TAG
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
RUN chmod +x ./entrypoint.sh
CMD ["node","server.js"]