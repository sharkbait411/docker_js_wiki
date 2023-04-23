# Dockerized - Wiki.js
## Current Documentation Version:
- Latest Update Version 1.0.0, updated by Matthew Branche on 05/01/2021

## Shell Purpose and Introduction
The purpose of this repository is to provide users with a centralized location for centralized links to critical tools, centralize documentation

## Architecture
This Shell uses a Docker Compose functionality and uses the below directory architecture:
- Main shell directory
    - main files:
      - changelog.md (documentation of release notes for each version upgrade of the shell)
      - README.md 
      - version.md (file used to document current version)
      - .env_wiki_example
      - .env_db_example
      - LICENSE
      - docker-compose.yml
      
## Running Shell
To start using this wiki, a user must complete the following steps:
- or download a copy of the repo to you desired location, or git clone. 
  - cd to the root source code directory, 
  - update the .env_db_example file name to .env_db and update the DB credentials
  - update the .env_wiki_example file name to .env_wiki and provide your correct wiki credentials (making sure to match with your DB credentials in .env_db)
  - run "docker-compose up -d" to start the wiki
  - Once the services is online, you can access the service via a web browser: http://YOUR-SERVER-IP:3000/
  - You should also be able to confirm access via the above, by completing a "docker-compose logs" and see the below message:
```
wiki_1  | 2023-04-23T21:39:45.738Z [MASTER] info: HTTP Server: [ RUNNING ]
wiki_1  | 2023-04-23T21:39:45.739Z [MASTER] info: 🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻
wiki_1  | 2023-04-23T21:39:45.739Z [MASTER] info:
wiki_1  | 2023-04-23T21:39:45.739Z [MASTER] info: Browse to http://YOUR-SERVER-IP:3000/ to complete setup!
wiki_1  | 2023-04-23T21:39:45.739Z [MASTER] info:
wiki_1  | 2023-04-23T21:39:45.739Z [MASTER] info: 🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺🔺

```
  - Once on the web browser you can initial the installation of the wiki, by setting your admin email/login, and password and building an initial page either by Markdown, html template, etc..
  
## Reference docs
- installing docker reference: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04
- installing docker-compose reference: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-22-04

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
