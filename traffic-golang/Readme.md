# Hello Docker Compose Readme #

This README file provides an overview of the `Docker Compose configuration` and code provided in this repository. The Docker Compose configuration consists of two services: `frontend` and `backend`, and it is designed to run a simple Go application that responds with a "Hello from Docker!" message.

# compose.yaml: #
  the compose.yaml defines two functions
    * `frontend`: Runs Traefik, a reverse proxy and load balancer, on port 90.
    * `backend`: Builds and runs a Go application on port 80, and Traefik routes requests to it.

# dockerfile: #
  The Dockerfile defines two build stages:
    * `build`: Compiles the Go application and produces an executable named backend.
    * `dev-envs`: Sets up development environment tools and user configurations.

# Running the Application #
   * Access the application by navigating to http://localhost:9090 in your web browser.
   * one should see the following message
                  ##         .
    ## ## ##        ==
 ## ## ## ## ##    ===
/"""""""""""""""""\___/ ===
{                       /  ===-
\______ O           __/
 \    \         __/
  \____\_______/

Hello from Docker!
    
