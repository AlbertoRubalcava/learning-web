# Docker Static Site Tutorial

This repository contains a simple setup using Docker and Docker Compose to serve static HTML, CSS, and a blank JavaScript file with an Nginx server.

The HTML includes a boilerplate form and a section that prints the URL query parameters and uses Bootstrap for styling.

## Directory Structure

learning-web/
├── docker-compose.yml
├── Dockerfile
├── nginx.conf
└── static/
    ├── index.html
    ├── style.css
    └── script.js

## Prerequisites

You must install Git as well as Docker on your machine. Your Git tool must be associated with your GitHub account.

### Git and GitHub
The easiest way to install Git and have it tied to your GitHub account is to use the [GitHub Desktop app](https://desktop.github.com).

The more "advanced" way is to download Git from the [official downloads page](https://git-scm.com/downloads).

_Note:_ If you're using macOS or Linux and prefer to use the Git cli, make sure to also download the [Git Credential Manager](https://github.com/git-ecosystem/git-credential-manager). This will allow you to have your passwords saved when cloning repos using HTTPS.

### Docker and Docker Compose

To install Docker and Docker Compose simply visit the official [Docker website](https://docs.docker.com/engine/install/)

## Setup Instructions

### Step 0: Fork the repository

Make sure you fork this repository first so that you can continue to the next step. You do this by logging in to your GitHub account, and click on the Fork button on this repository.

### Step 1: Clone the Repository

Once you've forked the repository, we must clone it to our machine. Navigate through your terminal and run the following command:

```bash
git clone https://github.com/your-username/docker-static-site-tutorial.git
cd docker-static-site-tutorial
```

or clone the repository through the GitHub Desktop App and follow the prompts.

### Step 2: Run and build the container

In your terminal, navigate to the project's root directory and run

```bash
docker-compose up -d
```

This command is a shorthand for the following two commands `docker-compose build` and `docker-compose up` in detached mode.

### Step 3: Verifying that everything worked

Open a new web browser and visit: `http://localhost:8080`. You should be presented with the sample index page.

### Step 4: Stopping the container

To stop your container, in your terminal navigate to the project's root directory and run

```bash
docker-compose down
```
