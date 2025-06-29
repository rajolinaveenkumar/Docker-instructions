FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://gist.githubusercontent.com/lillylangtree/b55828fa05ed3470d352/raw/3a7183fb56493ca42b5ddeeb73895f5a8cb1d6d3/index.html /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
