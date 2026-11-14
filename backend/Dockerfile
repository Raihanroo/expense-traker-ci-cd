FROM node:22-alpine

WORKDIR /app

RUN npm install --global npm@11.21.2

COPY package*.json ./
RUN npm install --omit=dev

COPY src ./src

EXPOSE 5000

CMD ["node", "src/server.js"]
