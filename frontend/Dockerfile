#Dockerfile (tag: v3)
#FROM node:latest

#RUN npm install webpack -g

#Downloading node modules to complile webpack
#WORKDIR /tmp
#COPY package.json /tmp/
#RUN npm config set registry http://registry.npmjs.org/ && npm install

#Running Webpack Compiled
#WORKDIR /app
#COPY . /app
#RUN cp -a /tmp/node_modules /usr/src/app
#RUN webpack
#RUN npm install webpack-cli -g

#ENV PORT = 8000

#EXPOSE 8000

FROM node:latest
RUN mkdir /app
WORKDIR /app
COPY . /app
RUN npm install

EXPOSE 8000

CMD [ "npm", "start", "run" ]
