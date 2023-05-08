# SERN setup

### My SQL Setup

Installation
```python
sudo apt update
sudo apt install mysql-server
```

Server Status
```python
sudo service mysql status
sudo service mysql stop
sudo service mysql start
```

Configuration
```python
# login to mysql
sudo mysql

# Setup root to use password
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';

exit;

# run following for security configuration
sudo mysql_secure_installation

# login to mysql using
sudo mysql -u root -p
```

Creating users
```python
CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';
```

Granting access to user
```python
GRANT CREATE, ALTER, DROP, INSERT, UPDATE, INDEX, DELETE, SELECT, REFERENCES, RELOAD on *.* TO 'sammy'@'localhost';
```

### Node js Installation
Install node using NVM(node version manager)

NVM Installation
```python
sudo apt install curl 

curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

Node Installation
```python
nvm install node 
```

### React Setup
```python
npm create vite@latest
```

### Express Setup
```python
npm init
npm install express mysql2 cors
```