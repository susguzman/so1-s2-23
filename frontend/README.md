# Frontend
A frontend application using reactjs.

## Get Started

``` bash
# Setting env vars
export REACT_APP_BACKEND_BASE_URL=http://localhost:3800

npm install
npm start
```

## Get Started with Docker

``` bash
# nginx version
docker build -t frontend:0.1.0-nginx-alpine -f nginx.dockerfile .
docker run -d -p 8888:80 frontend:0.1.0-nginx-alpine
```