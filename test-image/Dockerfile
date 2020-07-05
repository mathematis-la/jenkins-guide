FROM node:6-alpine

#create feports directory
RUN mkdir -p /JUnit

#create a server directory
RUN mkdir -p /home/node/tests
WORKDIR /home/node/tests

#install app dependencies
COPY /test-image/package.json /home/node/tests
RUN npm install

#copy test source
COPY test.js /home/node/tests

EXPOSE 9000

CMD ["npm","test"]
