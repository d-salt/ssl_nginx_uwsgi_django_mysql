FROM nginx:1.13
WORKDIR /etc/nginx
RUN apt-get update
RUN apt-get install -y openssl
RUN openssl req -days 365 -new -nodes -newkey rsa:4096 -x509 -keyout cert.pem -out cert.pem -subj "/C=JP/ST=Tokyo/L=Chuo-ku/CN=localhost"
