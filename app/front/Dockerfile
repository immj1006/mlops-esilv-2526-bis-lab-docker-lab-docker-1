FROM nginx:alpine

RUN apk add --no-cache bash

WORKDIR /usr/share/nginx/html

COPY . .

RUN sed -i 's/\r//' entrypoint.sh

ENTRYPOINT ["bash", "entrypoint.sh"]