FROM node:alpine
RUN npm install -g newman newman-reporter-htmlextra
WORKDIR /etc/newman
COPY  . .
CMD [ "newman", "run", "sck-online-store.postman_collection.json", "-e", "sck-online-store.postman_environment.json","-r", "htmlextra,cli,junit" ]