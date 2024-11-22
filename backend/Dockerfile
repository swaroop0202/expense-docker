FROM node:20
EXPOSE 8080
ENV DB_HOST=mysql
RUN useradd expense 
ENV DB_HOST=mysql
RUN mkdir /opt/server 
RUN chown -R expense:expense /opt/server
WORKDIR /opt/server
COPY *.js .
COPY package.json .
RUN npm install 
CMD [ "node","index.js" ]