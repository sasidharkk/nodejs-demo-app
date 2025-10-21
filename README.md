# Node.js CI/CD Pipeline using GitHub Actions

This repo demonstrates a simple CI/CD pipeline that:
- Installs dependencies
- Runs tests
- Builds a Docker image
- Pushes the image to DockerHub

## How it works
- GitHub Actions workflow located at `.github/workflows/main.yml`
- On push to `main`, the pipeline runs and pushes `youruser/nodejs-demo-app:latest`

## Local test
1. `npm install`
2. `npm start` (app runs on http://localhost:3000)
3. `docker build -t nodejs-demo-app .`
4. `docker run -p 3000:3000 nodejs-demo-app`

## Secrets (GitHub)
- DOCKERHUB_USERNAME
- DOCKERHUB_TOKEN (DockerHub access token)
