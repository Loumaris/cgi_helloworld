cgi_helloworld
==============

Just a simple setup to run a cgi file inside a docker container with nginx.

Based on the idea of https://github.com/asssaf/markdownjs-cgi

Running with docker
===================

First build:

```
docker build . -t loumaris/cgi_helloworld
```

and then run:

```
docker run -d --name helloworld -p 127.0.0.1:80:80 loumaris/cgi_helloworld
```

Now you can access http://localhost/helloworld.cgi


Running with docker-compose
===========================

Just do a

```
docker-compose up --build
```

and have a look at http://localhost/helloworld.cgi 
