FROM nginx:latest

WORKDIR /usr/share/nginx/html

COPY ./index.html index.html
COPY ./style.css style.css
COPY ./entrypoint.sh /usr/local/bin/

RUN chmod +x /usr/local/bin/entrypoint.sh

ENV WS_BACK_URL=http://localhost:8080

ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
EXPOSE 80