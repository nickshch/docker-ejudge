Docker image with ejudge contest management system
==================================================

This image contains [ejudge contest management system](https://ejudge.ru).

System login and password are `ejudge:ejudge`.

Data stored in `/home/ejudge`

Image without external volume for ejudge contests.

**There are issues with running PHP, Ruby and Go solutions.**

Building
========

    $ docker build -t ejudge .
    
Running
=======

    $ docker run -d \
        --name ejudge \
        -p 80:80
        ejudge
		
Installation check
==================

You can check ejudge here http://localhost/cgi-bin/serve-control

Login and password are `ejudge:ejudge`.

License
=======

BSD, see `LICENSE`
