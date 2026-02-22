FROM node:20-alpine AS build
WORKDIR /app
COPY pacakge*.json ./
RUN npm install
RUN npm audit fix --force
COPY . .
RUN npm start
