## CHALLENGE COMPONENT TESTS

## Dependencies

* Ruby 2.5
* Bundler 2.1.4


## WEBDRIVERS

* https://github.com/mozilla/geckodriver/releases
* https://chromedriver.chromium.org/downloads

---

## Installation Instructions

### Install bundler

### Configure gemset


```shell
rvm gemset list
```

If not created, you can do it manually

```shell
rvm gemset use ${folder_name} --create
```

Or if gemset was created but you need to set it, you can do it manually

```shell
rvm gemset use ${folder_name}
```

### Install bundler

To get started, install the bundler in version 2.1.4:

```shell
gem install bundler:2.1.4
```

If you not authenticated on Nexus using bundle, do it:

```shell
bundle config 10.129.178.173 yourVivoUser:password
```

Install dev libs

```shell
bundle config set --local with development 
```

and then

```shell
bundle install --full-index --binstubs 
```



## TSHIELD
TSHIELD é um MOCK-SERVER, ou seja, permite simulações de API para desenvolvimento e testes

https://mock-server.com/images/expectation_response_action.png
https://mock-server.com/images/expectation_forward_action.png

### DOCUMENTATION

https://github.com/diegorubin/tshield

### VCR 
https://github.com/diegorubin/tshield#config-options-for-http-vcr



## CHALLENGES

1) Utilizando VCR do tshield crie os mocks para seguintes endpoints da [pokeapi](https://pokeapi.co/)

- https://pokeapi.co/api/v2/pokemon/ditto
- https://pokeapi.co/api/v2/pokemon?limit=100000&offset=0
- https://pokeapi.co/api/v2/pokemon/1