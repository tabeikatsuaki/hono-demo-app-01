FROM node:23-bookworm

WORKDIR /app

COPY src ./src
COPY package.json package-lock.json ./
COPY tsconfig.json ./

RUN npm install

