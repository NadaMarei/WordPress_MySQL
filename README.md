# WordPress_MySQL

This repository contains a Docker Compose file that sets up a local development environment for WordPress with MySQL as the database.

## Prerequisites
- Docker
- Docker Compose

## Getting Started
1- Clone this repository to your local machine using the command:</br>
`git clone https://github.com/NadaMarei/WordPress_MySQL.git` </br>
</br>
2- Navigate to the repository's root directory: `cd WordPress_MySQL`</br>
</br>
3- Run the following command to start the containers in detached mode:`docker compose up -d`</br>
</br>
4- Access WordPress by navigating to `http://localhost:8000` in your web browser.</br>
</br>
5- Follow the on-screen instructions to set up WordPress.</br>
#### Once you have completed the setup, you will be able to log in to the WordPress admin panel using the credentials you provided.

## Stopping the Environment
To stop the environment, run the following command in the repository's root directory: </br>
`docker compose down`
</br>
#### This will stop and remove the containers, networks, and volumes created by the Docker Compose file.

## Accessing MySQL
To access the MySQL database, you can use a tool like`phpMyAdmin`. The `host is localhost`, the `port is 8080`, and the `username is wp_user` and `password is 1234`. </br>

 #### You can also access the MySQL container directly using the following command:</br>
 `docker exec -it mysql bash` </br>
 </br>
 This will open a bash shell inside the MySQL container, where you can run MySQL commands and interact with the database directly.
 
 ## Customizing the Environment
If you need to customize the environment, you can edit the `docker-compose.yml` file to change the configuration of the containers. For example, you can change the port mapping for the WordPress container, add additional environment variables for the MySQL container, or mount volumes to persist data across container restarts.

## License
This repository is licensed under the MIT License. See the LICENSE file for more information.

## Acknowledgments
This repository was built with ❤️ by <a href="https://github.com/NadaMarei">- Nada Marei</a> . Thank you to the open-source community for creating and maintaining the tools and technologies that make this project possible.
