#user an existing docker image as base 
FROM alpine
# Dowload and install deps 
RUN apk add --update redis 
# Tell image what to do when it starts as a container 
CMD [ "redis-server" ]
