# todo-app
## Pr 4: Manual Docker Setup

### Frontend
1. **Build the Docker image** for the frontend:
   ```bash
   docker build -t node-server .
   ```
2. **Run the container** on port 3300:
   ```bash
   docker run -p 3300:3300 node-server
   ```

### Backend
1. **Build the Docker image** for the backend:
   ```bash
   docker build -t node-server .
   ```
2. **Run the container** on port 5555:
   ```bash
   docker run -p 5555:5555 node-server
   ```

## Pr 5: Docker Compose Setup

### Build and Run

1. **Build the Docker image**:
   ```bash
   docker build -t node-server .
   ```

2. **Run the container** on port 3000:
   ```bash
   docker run -p 3000:3000 node-server
   ```

3. Use Docker Compose to **build and run** the services:
   ```bash
   docker-compose up --build
   ```

4. To **stop the services**, run:
   ```bash
   docker-compose down
   ```

5. To **restart the services**:
   ```bash
   docker-compose up
   ```

## New Steps

### Setup with Docker Compose

1. **Build the services**:
   ```bash
   docker-compose build
   ```

2. **Install dependencies** for the backend:
   ```bash
   docker-compose run backend sh
   npm install
   ```

3. **Build the services** again:
   ```bash
   docker-compose build
   ```

4. **Check Vite version** for the frontend:
   ```bash
   docker-compose run frontend sh
   npx vite --version
   ```

5. **Run the containers**:
   ```bash
   docker-compose up --build
   ```
