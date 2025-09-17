# Docker Setup Instructions

## Prerequisites
- Docker
- Docker Compose

## Running the Application

1. **Build and start the containers:**
   ```bash
   docker-compose up --build
   ```

2. **Access the application:**
   - Open your browser and go to: `http://localhost:5000`

3. **Stop the application:**
   ```bash
   docker-compose down
   ```

4. **Stop and remove volumes (clean reset):**
   ```bash
   docker-compose down -v
   ```

## Services

- **Web Application**: Flask app running on port 5000
- **Database**: MySQL 8.0 running on port 3306
  - Database: `ecommerce`
  - User: `shopuser`
  - Password: `password`
  - Root password: `rootpassword`

## Database

The database is automatically initialized with the schema and sample data from `ecommerce.sql` when the container first starts.

## Development

For development, you can mount your local code directory and enable hot reloading by modifying the docker-compose.yml volumes section.
