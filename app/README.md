# hello_http
Hello world with a webserver in C


## How to build
```gcc -o dummyserv dummy_serv.c```

Steps to build the Dev Container:
1.  Use this,
    $ git clone https://github.com/clanda20/hello_http/tree/main/app 
    to clone dummy_serv.c
2.  Run the image:  docker build -t homework1 .  ( don't forget the . )
3.  Run the docker container:
    $ docker run -dp 12344:12344 homework1
4.  Copy the ID or the name of the container by typing  
    $docker  container ls -all
    For example: suspicious_turing, or quirky_hodgkin




## How to run
The port argument is optional and when not included the service will default to port 8080

1.  Get to the directory inside docker container by typing:
    $ docker exec -it container-name /bin/sh
    For example:  $ docker exec -it quirky_hodgkin /bin/sh
2.  Check the directory:  ls -l
3.  Run:  $ ./dummyserv 12344
4.  open: http://localhost:12344



