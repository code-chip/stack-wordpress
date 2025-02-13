# Stack Wordpress
Stack docker for wordpress projects

What is WordPress?
WordPress is a free and open source blogging tool and a content management system (CMS) based on PHP and MySQL, which runs on a web hosting service. Features include a plugin architecture and a template system. WordPress is used by more than 22.0% of the top 10 million websites as of August 2013. WordPress is the most popular blogging system in use on the Web, at more than 60 million websites. The most popular languages used are English, Spanish and Bahasa Indonesia.

## Services
Mysql
PHPMyAdmin
Wordpress

## Requirements

- **Docker** 20.10.12+
- **Docker Compose** 1.25+
- **GIT** 2.25.1+

## How to Use
1- Download the shellscript run command `git clone git@github.com:code-chip/stack-wordpress.git new_projec`  
2- Access the fold with `cd new_projec`  
3- Change the remote repository to the new one `git remote set-url origin git@github.com:your_user_github/new_project.git`. Check the change by running the command `git remote --v`  
Before:
```bash
origin	git@github.com:code-chip/stack-wordpress.git (fetch)
origin	git@github.com:code-chip/stack-wordpress.git (push)
```
After
```bash
origin	git@github.com:your_user_github/new_project.git (fetch)
origin	git@github.com:your_user_github/new_project.git (push)
```
4- Fills the environment variable values int the .env file.  
5- Run the command `bin/dev build` or `docker-compose build`.  
6- Start services `bin/dev up` or `docker-compose up -d`.

## Available development commands
* `bin/dev build` will force (re)building the docker-compose stack.
* `bin/dev rebuild` will update the base docker images, build the docker-compose stack, stop the running containers and restart with the freshly built images.
* `bin/dev up` or `bin/dev start` will start the docker-compose stack.
* `bin/dev status` will print the current status of the docker-compose stack.
* `bin/dev restart` will restart the docker-compose stack.
* `bin/dev logs <service>` will print the logs for the given container.
* `bin/dev console <service>` will start a bash console inside the `wordpress, mysql or phpmyadmin` container.
* `bin/dev stop` will stop all running docker-compose stack containers.
* `bin/dev down` will stop and remove all docker-compose stack containers.

## Access broswer
Wordpress [http:localhost](http:localhost)  
PHPMyAdmin [http:localhost:8080](http:localhost:8080)  

## Documentation

* Maintained by:  
[the Docker Community⁠](https://github.com/docker-library/wordpress)

* Where to get help:  
[the Docker Community Slack]⁠(https://dockr.ly/comm-slack), [Server Fault](https://serverfault.com/help/on-topic)⁠, [Unix & Linux](https://unix.stackexchange.com/help/on-topic)⁠, or [Stack Overflow⁠](https://stackoverflow.com/help/on-topic)

* Where to file issues:  
https://github.com/docker-library/wordpress/issues⁠

* Supported architectures: ([more info](https://github.com/docker-library/  official-images#architectures-other-than-amd64)⁠)
amd64, arm32v5, arm32v6, arm32v7, arm64v8, i386, mips64le, ppc64le, riscv64, s390x

* Published image artifact details:  
repo-info repo's repos/wordpress/ directory⁠ (history⁠)
(image metadata, transfer size, etc)

* Image updates:  
[official-images repo's](https://github.com/docker-library/official-images/issues?q=label%3Alibrary%2Fwordpress) library/wordpress label⁠
[official-images repo's](https://github.com/docker-library/official-images/blob/master/library/wordpress) library/wordpress file⁠ ([history](https://github.com/docker-library/official-images/commits/master/library/wordpress)⁠)

* Source of this description:  
[docs repo's wordpress](https://github.com/docker-library/docs/tree/master/wordpress)/ directory⁠ ([history](https://github.com/docker-library/docs/commits/master/wordpress)⁠)
