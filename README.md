# dsrm-docker

This repository is for docker part of Dorm Social Rooms Manager.

## Requirements
To run whole project in docker you need:

- Backend with mariadb server: https://github.com/dorm-social-room-manager/dsrm-backend
- Frontend: https://github.com/dorm-social-room-manager/dsrm-frontend

## Downloading the repository

- Open your terminal / git-bash in location where you create a directory which will contain this repository

- Run the following command in your terminal / git-bash

  ```bash
  git clone https://github.com/dorm-social-room-manager/dsrm-docker.git
  cd ./dsrm-docker
  ```

- Next you need to download frontend and backend to the same location

  ```bash
  git clone https://github.com/dorm-social-room-manager/dsrm-backend.git
  git clone https://github.com/dorm-social-room-manager/dsrm-frontend.git
  ```

## Necessary configuration

- You need to build backend image

  ```bash
  cd ./dsrm-backend
  ./mvnw compile jib:dockerBuild
  cd ..
  ```

## Running application

- To run application you need to run this command
  ```bash
  docker compose up
  ```
