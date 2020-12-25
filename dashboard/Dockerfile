FROM node:14.15.1-alpine3.12
ARG REACT_APP_BASE_URL
ENV REACT_APP_BASE_URL $REACT_APP_BASE_URL
WORKDIR '/node'
COPY ./src/package.json ./
RUN npm install
ENV PATH=/node/node_modules/.bin:$PATH
WORKDIR '/node/app'
COPY ./src .
EXPOSE 3333
CMD npm start