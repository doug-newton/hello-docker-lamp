# Docker LAMP

Blank LAMP project in Docker with URL rewriting

## Usage

```
cd /path/to/project/root
```

Build the images:
```
$ sudo docker-compose build
```

Start the containers in detached mode:
```
$ sudo docker-compose up -d
```

To stop the containers:
```
$ sudo docker-compose stop
```

While the containers are running, you can access the MySQL CLI in the mariadb container like this:
```
$ sudo docker-compose exec mariadb mysql -uadmin -ppassword
```

or like this:
```
$ sudo docker-compose exec -T mariadb mysql -uadmin -ppassword < data.sql
$ sudo docker-compose exec -T mariadb mysqldump -uadmin -ppassword database > data.sql
```
