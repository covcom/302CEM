FROM node:wheezy
WORKDIR /home
RUN mkdir data
RUN npm install restify
ADD server.js /home/server.js
CMD ["node", "/home/server.js"]