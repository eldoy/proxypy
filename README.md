# Proxypy

Proxy DNS requests. This is perfect if you need wildcard domains support in your hosts file for local development.

Taken from [Marlon Tools.](https://github.com/hubdotcom/marlon-tools)

### Install

This package requires python2 to run:

```
brew install pyenv
pyenv install 2.7
pyenv global 2.7.18
```
The `python2` command should then be available.

### Config

Add your wildcard domain in `/etc/hosts/`:

```
127.0.0.1 *.firmalisten.test
```

### Start server

```
sudo python2 scripts/dns-proxy.py -s 8.8.8.8
```

Use in combination with [skilt](https://github.com/eldoy/skilt) for the perfect dev environment for your subdomain enabled apps.

Enjoy!
