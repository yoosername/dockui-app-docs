# dockui-app-docs

> Example App for use with [DockUI](https://github.com/yoosername/dockui)

## Quick start (Docker)

### Build Local Development Image

```shell
$ git clone https://github.com/yoosername/dockui-app-docs.git
$ cd dockui-app-docs
$ npm install
$ docker build --tag dockui/app-docs .
```

### Start the App

```shell
$ docker run -it \
  --env HTTP_PORT=3334 \
  --env HTTP_SCHEME=http \
  -p 3334:3334 \
  -v $(pwd):/app \
  dockui/app-docs
```
