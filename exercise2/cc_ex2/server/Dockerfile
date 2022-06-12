FROM node:12.18.1
ENV NODE_ENV=production
RUN mkdir -p /usr/src/server
WORKDIR /usr/src/server
COPY package.json /usr/src/server/
RUN npm install --production
COPY . /usr/src/server
EXPOSE 3000
CMD [ "node","server.js"]
