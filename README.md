# Office Portal Main

This repository, **office-portal-main**, serves as the main repository for the Office Portal project. It includes the following submodules:

- **Frontend**: `office-portal-ui`
- **Backend**: `office-portal-api`

The application is designed to run using Docker Compose for streamlined deployment.

---

## Prerequisites

Before proceeding, ensure the following tools are installed on your system:

- **Git**: To clone the repository and manage submodules.
- **Docker**: To build and run the application containers.
- **Docker Compose**: Comes bundled with Docker Desktop.

---

## Clone the Repository

To properly clone the `office-portal-main` repository along with its submodules, follow these steps:

### Clone with Submodules

Use the `--recurse-submodules` flag to clone the repository along with the submodules:

```bash
git submodule update --init --recursive
```

## Run the Application

The application is containerized and uses Docker Compose for deployment. Follow these steps to build and run it:

### 1. Build and Run Containers

Run the following command from the root of the `office-portal-main` repository:

```bash
docker-compose up --build
```

This command will:

- Build the frontend `(office-portal-ui)` and backend `(office-portal-api)` Docker images.
- Start the containers for both services.

### 2. Access the Application

- **Frontend:** Visit http://localhost:3000 in your browser.
- **Backend API:** Access the API at http://localhost:3001.
- **Swagger documents:** Visit http://localhost:3001/api-docs in your browser.
