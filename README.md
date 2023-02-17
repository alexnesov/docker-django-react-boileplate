# docker-django-react-boileplate
Boilerplate for React-Django projects contained in a Docker (Compose)



## Steps to initialize the project


### Building the Backend

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



