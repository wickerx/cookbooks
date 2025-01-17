# Node.js

## Docker

### Running

```sh
docker run -it --rm \
  $(echo $DOCKER_RUN_OPTS) \
  -h node \
  --name node \
  node:12.4-alpine /bin/sh
```

## Installation

### Homebrew

```sh
brew install nodejs
```

### YUM

```sh
curl -sL https://rpm.nodesource.com/setup_11.x | sudo -E bash -
sudo yum check-update
sudo yum -y install nodejs
```

### APT

```sh
curl -sL https://deb.nodesource.com/setup_11.x | sudo -E bash -
sudo apt update
sudo apt -y install nodejs
```

### Zypper

```sh
sudo zypper refresh
sudo zypper install -y nodejs10
```

### Chocolatey

```sh
choco install -y nodejs
```

### Source

#### Dependencies

##### APT

```sh
sudo apt update
sudo apt -y install curl g++ make
```

#### Build & Install

```sh
curl https://nodejs.org/dist/v11.8.0/node-v11.8.0.tar.gz | tar -xz
( cd node-v11.8.0 && ./configure && make && sudo make install ) && rm -r node-v11.8.0
```

## Configuration

### Windows

#### Node path

```sh
setx /m NODE_PATH %AppData%\npm\node_modules
```

## Commands

```sh
node -h
```

## REPL

```sh
node
```
