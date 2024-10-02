FROM node:latest

RUN npm install -g @angular/cli@17

WORKDIR /app
COPY package.json .
COPY package-lock.json .
RUN npm install
COPY . .
ENV PATH /app/node_modules/.bin:$PATH
