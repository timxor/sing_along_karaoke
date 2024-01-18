# sing_along_karaoke

### project details


name: sing_along_karaoke

description: sing along with your favorite song. all you need is a youtube url!

url: https://example.com

repo: https://github.com/timxor/sing_along_karaoke



### project structure

#### frontend

The frontend is accessible on port 3000.

```
frontend/
    - TypeScript
    - React
```

#### backend

The backend is accessible on port 8000.

```
backend/
    - Python
    - FastAPI
    - PostgreSQL
    - Docker  
```


### build and run the docker containers

build and run the frontend container:
```
cd /frontend
docker build -t my-frontend .
docker run -d -p 3000:3000 --name frontend-container my-frontend
```

build and run the backend container:
```
cd /backend
docker build -t my-backend .
docker run -d -p 8000:8000 --name backend-container my-backend
```


### start docker compose

start docker compose:
```
cd sing_along_karaoke/
docker-compose up
```





### issues

```
    - typescript build system
    - docker file
```
