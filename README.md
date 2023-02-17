# docker-django-react-boileplate
Boilerplate for React-Django projects contained in a Docker (Compose)



## Steps to initialize the project
```django-admin startproject api``` <br>
```cd api/```

Do a ```python manage.py runserver``` in ```api``` to test. <br><br>



### Building the Frontend
```npm install -g create-react-app``` if ```npm ERR! cb.apply is not a function``` <br>
```npx create-react-app frontend``` <br>


Do a ```npm start``` in ```frontend``` to test. <br>
<br>




### Stop the containers
```docker-compose down```

### Build the containers

```docker-compose build```


### Start the containers
```docker-compose up```




### Project tree structure

<code>
</code>

### docker-compose.yml explanation:

```docker-compose.yml``` file defines two services: frontend and backend. <br>
The frontend service builds a Docker image from the ./frontend directory, maps port 3000 in the container to port 3000 on the host, mounts the ./frontend directory as a volume in the container, sets the NODE_ENV environment variable to development, and runs the npm start command. The backend service does the same thing for the ./backend directory, mapping port 8000 in the container to port 8000 on the host, setting the DEBUG environment variable to True, and running the python manage.py runserver command.