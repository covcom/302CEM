# https://hub.docker.com/_/node/
FROM node:wheezy
WORKDIR /home
RUN npm install request restify ioredis mysql-promise
ADD server.js /home/server.js
EXPOSE 80:8080
CMD ["node", "/home/server.js"]
