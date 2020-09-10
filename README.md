# gostack-desafio06

This project works as the backend of a react application that you can find [here](https://github.com/Eurynomee/desafio-fundamentos-reactjs).


To make this project work on your computer be sure to:

run
```
yarn
```
to install all dependencies.

Then you'll need to create a postgres image on your docker and inside that image create the gostack_desafio06 database

to do that first run this script:
```
docker run --name gostack_desafio06 -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```
also run the migrations to create tables and stuff needed into the database you just created
```
yarn typeorm migration:run
```

and now you'll just need to hit

```
yarn dev:server
```
to start the server!!

have fun!
