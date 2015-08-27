FROM ubuntu:14.04

RUN apt-get update
RUN apt-get upgrade -y

RUN apt-get install -y nodejs

RUN ln -s /usr/bin/nodejs /usr/bin/node

RUN apt-get install -y npm
RUN npm install ws
#RUN npm install socket.io

ADD server.js /root/server.js

EXPOSE 8080

ENTRYPOINT ["/usr/bin/node", "/root/server.js"]
