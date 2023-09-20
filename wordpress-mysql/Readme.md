# Creating WordPress with MySQL #
This is a project to define and launch one of the basic setups for WordPress.
Reference link : Markup :  [WordPress image page]([http://www.google.fr/ "Named link title"](https://hub.docker.com/_/wordpress)) and http://www.google.fr/ or <http://example.com/>

#Prequisites
* Docker service installed

#Project Structure
.
├── compose.yaml
└── README.md

#steps:
* all the configuration regarding the docker is represented in the compose.yaml, it defines the services `db` for the `database` and `wordpress` for the `WordPress application`. 
* When you deploy this setup using `Docker Compose`, it maps the `WordPress container's port 80` to `port 80` on the host, as specified in the `compose.yaml` file.
* Open your web browser and navigate to `http://localhost:80` to access the WordPress installation page.

#Docker commands:
 * `docker compose up -d` - creates the necessary network and volumes, and starts the WordPress and database containers.
 * `docker ps` - verifies the containers that are running and the mapped ports.
 * `$ docker compose down -v` - This will delete the volumes, ensuring a clean removal of all data.

