### WordPress Development Containers for Visual Studio Code

`wordpress-devcontainer` is a simple configuration to support fully-dockerised development of WordPress themes and plugins using Visual Studio Code.

#### Requirements

- [Visual Studio Code](https://code.visualstudio.com/)
- [Visual Studio Code Remote Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

`wordpress-devcontainer` currently ships with:

- `wordpress:6.5.5-php8.3-apache`
- `mysql:9.0.0`
- `phpmyadmin:5.2.1-apache`

#### How to Use

Copy the `.devcontainer` folder into your project's folder. Open your project's folder in VS Code. Re-open VS Code in remote containers (`Remote-Containers: Reopen in Container`) and, after that, you will have everything set up for development.

A more detailed description of VS Code Dev Container can be found [here](https://code.visualstudio.com/docs/devcontainers/tutorial).

At this point your WordPress project can be accessed by [`localhost`](http://localhost) on your local machine.

Additional configuration can be defined in `.devcontainer/docker-compose.yaml`, like, among others, `WORDPRESS_TABLE_PREFIX`.

#### phpMyAdmin

[`phpMyAdmin`](https://www.phpmyadmin.net/) can be accessed via [`localhost:8080`](http://localhost:8080).

#### Extensions

`wordpress-devcontainer` currently ships with the following extensions for development in Visual Studio Code:

- ["eamodio.gitlens"](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- ["xdebug.php-pack"](https://marketplace.visualstudio.com/items?itemName=xdebug.php-pack)
- ["xdebug.php-debug"](https://marketplace.visualstudio.com/items?itemName=xdebug.php-debug)
- ["matthiashunt.wordpress-syntax-highlighter"](https://marketplace.visualstudio.com/items?itemName=matthiashunt.wordpress-syntax-highlighter)
