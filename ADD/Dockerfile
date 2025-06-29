FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://gist.githubusercontent.com/chrisvfritz/bc010e6ed25b802da7eb/raw/18eaa48addae7e3021f6bcea03b7a6557e3f0132/index.html /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
