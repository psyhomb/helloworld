Hello World
===========

This is a simple image that just gives a response on port 8000

```bash
$ docker images | grep helloworld
REPOSITORY        TAG       IMAGE ID        CREATED          VIRTUAL SIZE
helloworld        latest    1cae431873e4    23 seconds ago   1.13MB
```


Sample Usage
------------

### Starting a web server on port 8000

```bash
$ docker run -d --name helloworld -p 8000:8000 helloworld
```

You can now interact with this as if it were a dumb web server:
```
$ curl localhost:8000
<pre>
Hello World => build #1


                                       ##         .
                                 ## ## ##        ==
                              ## ## ## ## ##    ===
                           /""""""""""""""""\___/ ===
                      ~~~ {~~ ~~~~ ~~~ ~~~~ ~~ ~ /  ===- ~~~
                           \______ o          _,/
                            \      \       _,'
                             `'--.._\..--''
</pre>
```
