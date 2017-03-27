# Online game infrastructure


[![Build Status](https://travis-ci.org/srebrny/online-game-infrastructure.svg?branch=master)](https://travis-ci.org/srebrny/online-game-infrastructure)

## Here is a more information about project

@todo


## Project Goals


## How to run project

1) Setup requirements
2) Setup docker images


    $ ansible-containers build
    
3) 


## Application architecture

master servers are marked as zero eg. lbs0 or dbs0
any other servers eg. dbs2, elk3 or cdn3 is a slave server. 

### Server naming convention

* lbs - is a loadbalancers for application
* whp - is a application worker - this is a flask application
* dbs - is a database server 
* elk - is a elasticsearch cluster 
* cdn - is a content delivery network servers. 
        It store and serve application assets like images, style sheet files. 

More information about my system of naming server you can see at [this address](https://www.srebniak.pl/watki-tematyczne/server-naming-conventions/)