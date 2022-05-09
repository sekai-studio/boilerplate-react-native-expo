FROM node:16.14.2-buster-slim

RUN apt-get update
RUN apt-get install -y git

RUN yarn global add expo-cli@5.3.2

RUN mkdir /var/myAppName
WORKDIR /var/myAppName

CMD sleep infinity