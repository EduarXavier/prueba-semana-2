FROM node:20-alpine3.17

LABEL version=1.0

WORKDIR /app/

COPY ./app/ .

RUN npm i

ENV USER="Eduar"

EXPOSE 8080

CMD ["npm", "start"]



