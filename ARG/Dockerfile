ARG version 
FROM almalinux:${version:-9}
ENV owner="Naveen Rajoli" \
    project="Prod"

ARG USERNAME=naveenrajoli
ENV USERNAME=$USERNAME
RUN echo "Hello User: ${USERNAME}, image version: ${version}" > /tmp/devops.txt
CMD ["sleep", "100"]