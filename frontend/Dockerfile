FROM node:lts

ARG NODE_ENV=developemnt
ENV NODE_ENV $NODE_ENV

WORKDIR /app

ARG PORT=8080
ENV PORT $PORT
EXPOSE $PORT 8081 8082

COPY package.json /app
COPY package-lock.json /app
RUN npm i

COPY . /app

CMD npm run start
