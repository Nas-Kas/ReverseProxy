
# Reverse Proxy

Reverse proxy that redirects traffic from node.js webapp on localhost:3000 to localhost

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Apache2

```
Install using (sudo apt-get install apache2)
```

Nodejs

```
Install using (sudo apt install nodejs)
```

EJS

```
Install using npm install ejs
```
### Installing
Update conf files in your local sites-available directory to conf files found in git repository directory in most apache2 setups below
```
file directory: (/etc/apache2/sites-enabled)
```

Enable proxy and proxy_http using the following commands
```
a2enmod proxy
a2enmod proxy_http
```
Cd to directory containing server.js to run server locally

```
nodejs server.js
```

To start up apache server

```
sudo /etc/intit.d/apache2 start
```
if you run into error here something else could possibly be running on port 80 like nginx turn off other services







