FROM almalinux:9

ENV NODE_ENV=prod
ENV APP_HOME=/usr/share/nginx/html/

RUN dnf install nginx -y
WORKDIR $APP_HOME
# No need specify full location bcz we set an working directory
RUN rm -rf index.html 
COPY index.html index.html
CMD ["nginx", "-g", "daemon off;"]