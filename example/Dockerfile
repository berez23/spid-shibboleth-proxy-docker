FROM node:16.8.0-alpine3.13
RUN apk --update add gettext
COPY docker-bootstrap.sh /usr/local/bin/
WORKDIR /src/app
COPY . .
RUN npm install
EXPOSE 8080
CMD ["docker-bootstrap.sh"]
