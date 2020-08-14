# wordpress-image

Simple wordpress install with alpine linux, apache2 and php7

Includes the latest wordpress download exploded in `/var/www/localhost/htdocs`

### Running the container
If you are pulling from docker via `docker pull` or `docker run` skip to the "**Start the container:**" section.

Download the source files.

**Build the container:**

`docker build -t wordpress .`

___
**Start the container:**

`docker run -id --name wordpress -p 8080:80 awksed/wordpress-image`

>Apache is listening on port 80 of the container, so you will need to expose port 80.

>Ports are in the format of: `<localhost port>:<container port>` example: `8080:80`

>Point your browser to the http://host:port/ and run the setup.

#### No DB is included. Choose an approriate host for the DB during the WordPress setup
