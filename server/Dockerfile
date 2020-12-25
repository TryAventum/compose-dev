FROM node:14.15.1-alpine3.12 as debug
WORKDIR "/app"
COPY ./src/package.json ./
RUN npm install
RUN npm install -g nodemon
COPY ./src .
CMD ["nodemon", "--inspect=0.0.0.0", "--ignore", "content/", "--ignore", "locales/", "index.js"]