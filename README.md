# API Template MongoDB

by Nathan Wall

## Description

Template for FastAPI/MongoDB projects

## Installation 

### Manual
From root folder of project: <br/>
`pip install poetry`<br/>
`poetry install`

### Docker
From root folder of project: <br/>
`docker build --no-cache -t api_template_mongodb -f .docker/Dockerfile .`<br/>

## Execution

### Manual
`uvicorn api:app --host 0.0.0.0 --port 8080`<br/>

### Docker Compose
`docker-compose -f .docker/docker-compose.yml up -d --build`<br/>

### Docker
`docker run -it --rm -p 8080:8080 -e SERVER_HOST=0.0.0.0 -e SERVER_PORT=8080 --name api_template_mongodb api_template_mongodb:latest`<br/>

## API Documentation

OpenAPI (Swagger) docs comes as standard with FastAPI applications. To access simply navigate to `localhost:8080/docs`