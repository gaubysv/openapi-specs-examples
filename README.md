## Swagger UI
#### Start WEB server
```console
python3 -m http.server 8080
```

#### Links:
- [FarmStall API](http://localhost:8080/FarmStall/swagger-ui.html)
- [PetSitter API](http://localhost:8080/PetSitter/swagger-ui.html)


## Mock APIs
#### HTTP Mock Server
An open-source HTTP mock and proxy server - [Prism](https://stoplight.io/open-source/prism).

#### Requirements:
1. Node.js v17+
2. npm

#### Install Prism
```console
npm install --global @stoplight/prism-cli
```

#### Mock FarmStall API
> **Note:** update **servers.url** value in [FarmStall API definition file](FarmStall/farmstall-api.yaml) to point to the mock server.
```console
prism mock -p 9090 ./FarmStall/farmstall-api.yaml
```

#### Mock PetSitter API
> **Note:** update **servers.url** value in [PetSitter API definition file](PetSitter/petsitter-api.yaml) to point to the mock server.
```console
prism mock -p 9090 ./PetSitter/petsitter-api.yaml
```