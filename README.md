## How to run backend?

- ### Install Java-17 and JavaC

- ### Setting up MySQL
	- Download MySQL
        ```
        sudo dnf install community-mysql-server -y
        ```
	- Enable and start `mysqld`
        ```
        sudo systemctl enable --now mysqld
        ```
	- Install MySQL
        ```
        sudo mysql_secure_installation
        ```

- ### Edit **`src/resources/application.properties`**
  - Edit MySql Database configuration
    ```
    mysql -u root -p
    ```
    ```
    create database YOUR_DATABASE_NAME;
    ```
    ```
    show tables;
    ```
  - Paste your stripe payment gateway secret key
  - Paste your email and app password
	

- ### Start backend server locally
	```
	export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
	```
	```
	path/to/mvn spring-boot:run
	```

## How to run frontend?
```
npm i
```
```
npm start
```


> For further help: akshaymhaske2027@gamil.com
