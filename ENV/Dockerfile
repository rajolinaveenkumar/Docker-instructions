FROM almalinux:9

ENV NODE_ENV=prod
ENV APP_HOME=/usr/share/nginx/html/index.html

WORKDIR $APP_HOME
# No need specify full location bcz we set an working directory
RUN rm -rf index.html 
COPY index.html index.html
CMD ["nginx", "-g", "daemon off;"]


# Tip:
# You can override ENV values at runtime using docker run -e:

    
# What this does:
# 1. Sets NODE_ENV and APP_HOME environment variables.
# 2. $APP_HOME can be used later in the Dockerfile (WORKDIR $APP_HOME).
# 3. The environment variables will also be available inside the container when it runs.

