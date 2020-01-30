# docker-box-apps

Repository for dockerfiles to install a specific app inside a docker container.

## Writing sandboxed apps yourself

As a convention, folder names need to match the name of the executable you want
to run with [docker-box](https://github.com/compose-us-research/docker-box). 
Inside the `Dockerfile` you can add all necessary installation steps for the app
you want to run.
