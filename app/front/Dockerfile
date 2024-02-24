FROM nginx:latest

WORKDIR /usr/share/nginx/html

COPY ./index.html index.html
COPY ./style.css style.css
COPY ./entrypoint.sh /docker-entrypoint.sh

RUN chmod +x /docker-entrypoint.sh

ENV WS_BACK_URL=http://localhost:8080

ENTRYPOINT ["/docker-entrypoint.sh"]
EXPOSE 80