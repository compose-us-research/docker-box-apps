# docker-box-apps

Repository for dockerfiles to install a specific app inside a docker container.

## Writing sandboxed apps yourself

As a convention, folder names need to match the name of the executable you want
to run with [docker-box](https://github.com/compose-us-research/docker-box). 
Inside the `Dockerfile` you can add all necessary installation steps for the app
you want to run.

### Using Dockerfile or docker-compose.yml

`docker-box` first checks for a `docker-compose.yml` file. If it sees one, it 
will run the command through the `app` service. If you don't specify any 
additional arguments, it will run `docker-compose up` instead of using 
`docker-compose run app ...`.

If it cannot find a `docker-compose.yml` file, it will try to use `docker run`.

For an example using `docker-compose.yml`, see the [image-fun](./image-fun) 
directory. For an example with `Dockerfile`, see [youtube-dl](./youtube-dl).
