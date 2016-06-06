# Simple TOR Socks Proxy Container

Dockerfile to setup and compile tor software usgin Debian. When ran tor starts with a SOCKS5 server accessible on port 9150
(This does not set up a tor relay or exit node).

### Running

*Verbose:*
```bash
$ docker run --name tor -ti -p 9150:9150 jgamblin/tor
```
![](http://i.imgur.com/03n8NE6.png)

*As a Dameon:*
```bash
$ docker run  --name tor -tid -p 9150:9150 jgamblin/tor
```
![](http://i.imgur.com/AaV3VL6.png)

### To use, configure your browser/client to use a SOCKS server

    Server IP: 127.0.1.1
    Server port: 9150

![](http://i.imgur.com/GLWqKuV.png)

### WARNING

* Programing might be science; but that's not what I do. I'm a hacker, not a programmer.
* This is also probably a really bad idea. 
