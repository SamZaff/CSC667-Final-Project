FROM node:alpine
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY package.json package.json
RUN npm install
COPY . /usr/src/app
WORKDIR /usr/src/app/help
RUN npm install
RUN npm run build
EXPOSE 3004