FROM node:14-alpine

WORKDIR /usr/app

COPY ./package.json /usr/app

RUN npm install 

COPY ./ /usr/app

EXPOSE 4000

CMD ["npm","start"]