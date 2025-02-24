# Directus instance

This repository contains a Docker Compose setup for a Directus instance for the EMI sample handling. This setup is temporary (longer term solution is beeing built at https://github.com/earth-metabolome-initiative/emi-monorepo). To get started, follow the instructions below.

## Prerequisites

Before you begin, make sure you have the following prerequisites installed:

- Docker: [Install Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)

## Setup

### 1. Clone the repository to your local machine:

```bash
git clone https://github.com/digital-botanical-gardens-initiative/Directus-prod.git
cd Directus-prod
```

### 2. Create a .env file in the root folder and edit it to suit your needs:
```bash
cp .env.example .env
vim .env
```

### 3. Deploy the application:

```sh
docker compose up -d
```

Note: using the latest Directus image you might need to launch this command several time see https://github.com/directus/directus/issues/20542

This command will start the necessary services, including the database and your application.

## Accessing Your Application

Once the deployment is complete, you can access your application by opening a web browser and navigating to http://localhost:8056 (or the appropriate URL as per your configuration).


## Stopping and Cleaning Up

To stop the application and remove the containers, run the following command:

```sh
docker compose down
```

## Contributing

If you would like to contribute to this project or report issues, please follow our contribution guidelines.

## License

see [LICENSE](https://github.com/digital-botanical-gardens-initiative/Directus-prod/LICENSE) for details.