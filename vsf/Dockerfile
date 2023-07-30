FROM node:16-alpine

WORKDIR /var/www

COPY . .

RUN apk add --no-cache libc6-compat

RUN yarn install

COPY ./vue-storefront.sh /usr/local/bin/

RUN chmod a+x /usr/local/bin/vue-storefront.sh

ENTRYPOINT ["vue-storefront.sh"]
