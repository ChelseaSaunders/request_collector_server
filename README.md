# Request Bin Backend

### Install Request Collector
download the code by cloning the repository
```
git clone https://github.com/ChelseaSaunders/request_collector_server
```

also download the **frontend** by cloning the repository and following installation instructions in corresponding README file.
```
git clone https://github.com/ChelseaSaunders/request_collector_frontend
```

### Create and initialize database
Initializing the PSQL database
```
createdb endpoints
psql -d endpoints < schema.sql
```

### Set up environment file with database information
to ensure that this connects correctly add the file `.env` to the `requestbin` folder
this file will have the following content:
```
PORT = 4000
MONGODB_URI= "##URI from setting up Mongo database"

PG_DATABASE: endpoints
```

### Starting Request Collector Backend
enter into the respository, download dependancies, and run the applciation
```
cd request_collector_server
npm install
npm start
```
