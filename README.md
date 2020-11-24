## Welcome to apiPot project
![logo.apipot.com](https://logo.apipot.com/4/default.png)

+ [www.apipot.com](https://www.apipot.com)
+ [logo.apipot.com](https://logo.apipot.com)


## install on VPS

    git clone https://github.com/apipot/www.git
    cd www
    
    sh install.sh
    
    sh ssl.sh
    
    sh status.sh
    
    sh start.sh
    
    

## Data processing
Data from folder: "data/in" are used to generate the content in folder: "repo/"     
    
    sh data.sh

## Tests    

https://apipot.com
https://foo.apipot.com
http://user.auth.apipot.com/
    
    sh test.sh
    
![firefox_2020-11-24_19-50-23.png](docs/firefox_2020-11-24_19-50-23.png)
    
## What it's apiPot?

Platforma prezentacji mediów z róznych platform

## How it work's?

### stworzenie projektu, konfiguracja
podaj 2 parametry:
+ url repozytorium
+ nazwa projektu (domyslna pochodzi z formatu: [repozytorium].[organisation].apipot.com) 

### zarządzanie projektami
+ dodawanie
+ edycja grupowa wszystkich mediów jednocześnie na jednej stronie

### routing
jakie technologie pozwolą szybko tworzyć routing dla subdomen?

### deployment
Projekt jest wystawiany jako statyczny projekt
deployment w wersji darmowej nie obejmuje własnego środowiska.
Dopiero w wersji płatnej jest własny numer IP serwera.


## Nodejs libraries

subdomains
https://www.npmjs.com/package/wildcard-subdomains


## Node + Express + LetsEncrypt : Generate a free SSL certificate and run an HTTPS server in 5 minutes or less 
https://itnext.io/node-express-letsencrypt-generate-a-free-ssl-certificate-and-run-an-https-server-in-5-minutes-a730fbe528ca

# you can create one certificate with a lot of domain names.
But *.*.xyz isn’t possible.
That’s not a Letsencrypt limit. That’s a general DNS limit.
A * is only allowed as first label.

Stworzyć listę subdomen i dodawać je do tworzenia certyfikatów

http://apipot.com/.well-known/acme-challenge/Nmg6X_QPTUf3aIahAIRIyI2nk01PdXNPbwfvzKEKlfU