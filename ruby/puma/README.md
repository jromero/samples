# Ruby sample app using Puma web server

## Building

`pack build puma-sample --buildpack gcr.io/paketo-community/ruby`

## Running

`docker run --interactive --tty --publish 9292:8080 puma-sample`

`9292` is the default port for rack compliant web servers. As of date, the puma
buildpack requires that the app source have a `config.ru` file.

## Viewing

`curl http://localhost:8080`