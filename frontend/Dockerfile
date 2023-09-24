FROM node:lts-alpine3.17

ENV CI=true
ENV PORT=3000

WORKDIR /code
COPY package.json /code/package.json
COPY package-lock.json /code/package-lock.json
COPY . /code
RUN npm install
#RUN adduser -D -u 1001 -g 1001 nonroot
#USER nonroot
CMD ["npm", "start"]