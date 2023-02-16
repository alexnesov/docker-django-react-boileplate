# docker-django-react-boileplate
Boilerplate for React-Django projects contained in a Docker (Compose)



## Steps to initialize 




### Start the containers
```docker-compose up```

### Stop the containers
```docker-compose down```


### Project structure


myproject/
├── backend/
│   ├── Dockerfile
│   └── requirements.txt
├── frontend/
│   ├── Dockerfile
│   ├── package-lock.json
│  


### docker-compose.yml explaination

```docker-compose.yml``` file defines two services: frontend and backend. <br>
The frontend service builds a Docker image from the ./frontend directory, maps port 3000 in the container to port 3000 on the host, mounts the ./frontend directory as a volume in the container, sets the NODE_ENV environment variable to development, and runs the npm start command. The backend service does the same thing for the ./backend directory, mapping port 8000 in the container to port 8000 on the host, setting the DEBUG environment variable to True, and running the python manage.py runserver command.