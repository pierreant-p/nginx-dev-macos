# nginx dev server

This readme describes how to install a local nginx server for development, on MacOS.

In this readme, we assume that your development folder is `~/dev`.


## Install

```
brew install nginx

git clone git@github.com:/pierreant-p/nginx-dev-macos ~/dev
```


## Config

Add the dev nginx config file and relaod the server

```
sudo ln -s ~/dev/nginx-dev-macos/dev.conf /usr/local/etc/nginx/servers/
```

Replace `/YOUR/DEV/FOLDER` in `dev.conf` by the actual folder that contains your development files.
Eg: `/Users/pierreant-p/dev`.

Restart nginx.

```
sudo nginx -s reload
```
