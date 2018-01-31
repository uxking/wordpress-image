# wordpress-image

Simple wordpress install with alpine linux, apache2 and php5

Includes the latest wordpress download exploded in `/var/www/localhost/htdocs`

### Running the container
Start the container via:

`docker run -id --name wordpress -p 8080:80 awksed/wordpress-image`

>Apache is listening on port 80 of the container, so you will need to expose port 80.

>Ports are in the format of: `<localhost port>:<container port>` example: `8080:80`


