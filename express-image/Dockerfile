FROM node:6-alpine

# Create a server directory
RUN mkdir -p /home/node/app
WORKDIR /home/node/app

#install server dependencies
COPY /express-image/package.json /home/node/app
RUN npm install

#COPY node Application
COPY app.js /home/node/app

#Open Port
EXPOSE 9000

CMD ["npm","start"]
