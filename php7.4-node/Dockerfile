FROM bonnierpublications/php-alpine:php7.4
LABEL maintainer="paris@bonnier.dk"

# Install Node + NPM
RUN apk add --update nodejs nodejs-npm

EXPOSE 8080

# Configure a healthcheck to validate that everything is up&running
HEALTHCHECK --timeout=10s CMD curl --silent --fail http://127.0.0.1:8080/fpm-ping
