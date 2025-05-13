# sccellfie-website

## Overview
This repository contains the necessary files to deploy the **www.sccellfie.org** website using Docker Compose. Follow the steps below to set up and run the website.

## Prerequisites
Ensure you have the following installed on your machine:
- [Git](https://git-scm.com/)
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Deployment Steps

### 1. Clone the Repository
```sh
git clone git@github.com:ventolab/sccellfie-website.git
cd sccellfie-website
```

### 2. Start the Containers
Run the following command to start the website in detached mode:
```sh
docker compose up -d
```

### 3. Access the Website
Open your browser and navigate to:
```
http://YOUR_MACHINE_IP:80
```
By default, the website runs on port **80**.

## Stopping the Deployment
To stop and remove the running containers, use:
```bash
docker compose down
```

## Logs & Debugging
To check the logs of the running containers, use:
```bash
docker compose logs -f
```

## Troubleshooting
- Ensure that no other services are running on port **80**.
- Use `docker ps` to verify that the containers are running.
- If needed, restart the deployment:
```bash
  docker compose down
  docker compose up -d
```

