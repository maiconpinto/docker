# CakePHP

```bash
docker run --rm -v "$(pwd):/cakephp" maiconpinto/cakephp:create-project -e APP_NAME=app
```

Change directory to your APP_NAME and run:

```bash
docker run --name cakephp -d --rm -v "$(pwd):/var/www/html" -p 8080:80 maiconpinto/cakephp:0.1
```

With database:

```bash
docker run --name mysql -d --rm -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=cakephp -p 3306:3306 mysql:5.7
```
