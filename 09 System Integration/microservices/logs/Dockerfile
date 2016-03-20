# https://hub.docker.com/_/node/
FROM node:wheezy
WORKDIR /home
RUN mkdir data
RUN npm install ioredis
ADD server.js /home/server.js
CMD ["node", "/home/server.js"]
