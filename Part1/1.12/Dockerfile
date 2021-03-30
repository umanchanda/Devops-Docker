FROM node:14

COPY /example-frontend .

RUN npm install && npm install -g serve

RUN npm run build

EXPOSE 5000

CMD [ "serve", "-s", "-l", "5000", "build" ]
