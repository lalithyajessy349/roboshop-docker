FROM node:20    #nodeje image
WORKDIR /opt/server  #create directory
COPY package.json .    #copied application code
COPY *.js .
RUN nmp install  #to install dependencies
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node","server.js"]    #to start the container
