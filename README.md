### Dockerfile
```
FROM docker/whalesay:latest
MAINTAINER Misa Ogura misa.ogura01@gmail.com

RUN apt-get -y update && apt-get install -y fortunes
ENV PATH $PATH:/usr/games/

CMD fortune -a | cowsay
```
-----
### Instruction
1. [Download & install Docker](https://docs.docker.com/engine/getstarted/step_one/#step-1-get-docker)

2. Pull & run the programme - whale will give you a wise advise : `$ docker run misaogura/wise-whalesay`
```
 _________________________________________
/ If women are supposed to be less        \
| rational and more emotional at the      |
| beginning of our menstrual cycle, when  |
| the female hormone is at its lowest     |
| level, then why isn't it logical to say |
| that in those few days women behave the |
| most like the way men behave all month  |
| long?                                   |
|                                         |
\ -- Gloria Steinham                      /
 -----------------------------------------
    \
     \
      \
                    ##        .
              ## ## ##       ==
           ## ## ## ##      ===
       /""""""""""""""""___/ ===
  ~~~ {~~ ~~~~ ~~~ ~~~~ ~~ ~ /  ===- ~~~
       \______ o          __/
        \    \        __/
          \____\______/
```

3. Try again for some more wise insights : `$ docker run misaogura/wise-whalesay`

```
 ________________________________________
/ Voodoo Programming: Things programmers \
| do that they know shouldn't work but   |
| they try anyway, and which sometimes   |
| actually work, such as recompiling     |
| everything.                            |
|                                        |
\ -- Karl Lehenbauer                     /
 ----------------------------------------
    \
     \
      \
                    ##        .
              ## ## ##       ==
           ## ## ## ##      ===
       /""""""""""""""""___/ ===
  ~~~ {~~ ~~~~ ~~~ ~~~~ ~~ ~ /  ===- ~~~
       \______ o          __/
        \    \        __/
          \____\______/
```
-----
### Links
- Not so wise version of whalesay: https://hub.docker.com/r/misaogura/whalesay/
- docker/whalesay repo: https://hub.docker.com/r/docker/whalesay/
-----
### Authour
Misa Ogura
