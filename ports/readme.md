# Portainer (CE) #
This example provides a base setup for using Portainer. More details on how to customize the installation and the compose file can be found in portainer documentation.

Demo
You can try out the public demo instance first: http://demo.portainer.io/

username: admin
password: tryportainer

services:
  portainer:
    image: portainer/portainer-ce:alpine
Deploy with docker compose
When deploying this setup, the web interface will be available on port 9000 (e.g. http://localhost:9000).

$ docker compose up -d
Starting portainer ... done
Expected result: 
* Navigate to http://localhost:9000 in your web browser to access the portainer web interface and create an account.

Stop the containers with

$ docker compose down
# To delete all data run:
$ docker compose down -v
Troubleshooting
Select the correct image for your OS. You can take a look at the published tags at DockerHub
e.g. currently, the latest tag is for Windows (amd64) and alpine for Linux (amd64, arm/v7)
