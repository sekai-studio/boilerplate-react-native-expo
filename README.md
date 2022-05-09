# MY EXPO APP

It's a boilerplate to build quickly an app with expo.

## Prerequisites

- [Docker Engine](https://docs.docker.com/engine/) (version `20.10`)
- [Docker Compose](https://docs.docker.com/compose/) (version `2.4`)
- [nodejs](https://nodejs.org/en/) (version `16.14.2`)

To check versions:
```sh
docker --version && docker-compose --version && node -v
```

### On OSX: install Docker

#### <u>With Docker website</u>

follow the instructions from this [Page](https://docs.docker.com/get-docker/)

**OR**

#### <u>With Brew</u>

Brew is a popular package manager on *macOS*.
However it doesn't come pre-installed: follow the instructions from the Brew [Website](https://brew.sh/index_fr):

```sh
brew cask install docker
```

## Gettting started

Git clone this project in a working directory, next:

```
cd //**yourNameApp**//
yarn i 
cd .docker
echo "REACT_NATIVE_PACKAGER_HOSTNAME=###YOUR_IP_ADDRESS###" > .env 
docker-compose up -d 
```

Output:
```
container //**yourNameApp**// Started 
```

## Run the application 

Open a terminal, and make sure an image is created why the name is `//**yourNameApp**//`:

```
docker ps
```

After, access to the console:

```
docker exec -it //**yourNameApp**// bash
```

And, start the application.

<u>with debugger</u>:
```
yarn run start
```
To access the debugger page [localhost:19000/debugger-ui](http://localhost:8081/debugger-ui/)

<u>without debugger</u>:
```
yarn run no-debugger
```