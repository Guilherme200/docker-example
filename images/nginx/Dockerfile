FROM nginx:latest

LABEL version="1.0.0" description="Site com NGINX" maintainer="Guilherme Matoso"

RUN apt update && apt install curl -y

COPY ./index.html /usr/share/nginx/html/

VOLUME /arquivos

EXPOSE 80

ENV API_NAME='meu_site'

WORKDIR /usr/share/nginx/html/

ENTRYPOINT ["/usr/sbin/nginx"]

CMD ["-g", "daemon off;"]