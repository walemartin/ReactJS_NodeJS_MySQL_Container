FROM node:lts-alpine3.17


RUN mkdir -p /app
WORKDIR /app

COPY package*.json /app
COPY . /app
#RUN  npm i bcrypt
#RUN npm install bcrypt

#RUN  npm rebuild bcrypt --update-binary
RUN apk add --no-cache make gcc g++ python3
#RUN adduser -D -u 1001 -g 1001 nonroot
#USER nonroot 
RUN npm install
CMD ["npm", "start"]