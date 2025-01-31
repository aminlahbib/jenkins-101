This repository contains a Docker Compose configuration for a demo installation of Jenkins. This setup is not intended for production systems.
Credits: This approach is mostly based on the [offical instructions](https://www.jenkins.io/doc/book/installing/docker/) but takes advantage of Docker Compose (by using a `docker-compose.yml` file) to reduce the number of steps needed to get Jenkins up and running.

# Docker Installation

## Step 1

Install Docker locally (probably using Docker Desktop is the easiest approach).

## Step 2

Clone this repository or download it's contents. 

## Step 3

Open a terminal window in the same directory where the `Dockerfile` from this repository is located. Build the Jenkins Docker image:
```
docker build -t my-jenkins .
```

## Step 3

Start Jenkins:

```
docker compose up -d
```

## Step 4

Open Jenkins by going to: [http://localhost:9090/](http://localhost:9090/) and finish the installation process.


## Step 5

If you wish to stop Jenkins and get back to it later, run:

```
docker compose down
```
