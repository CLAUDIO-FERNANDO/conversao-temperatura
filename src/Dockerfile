# FROM ubuntu
# RUN apt-get update
# RUN curl -fsSL https://deb.nodesource.com/setup_21.x | bash - &&\
# apt-get install -y nodejs
# WORKDIR /app
# COPY . .
# #RUN  apt-get install npm --yes
# CMD [ "node","server.js" ]


FROM node:12.18.1
 
WORKDIR /app
 
COPY package.json package.json
COPY package-lock.json package-lock.json
 
RUN npm install
 
COPY . .
 
CMD [ "node", "server.js" ]

