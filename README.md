# Trab-nuvem-Containers-e-K8s

* [Alexandre Cunha C.Oliveira](@alexandreceti)
* [Henrique franzoni keppel](@HenriqueKeppel)
* [Lucas Medeiros](@bylucasxdx)
* [Prince Sanis](@princesanis)


Trabalho de Arquitetura em Nuvem.    
Curso/Oferta: Arquitetura de Software Distribuído – Oferta 10 Disciplina: Arquitetura de Nuvem.   
Professor: Marco Aurélio S. Mendes

## Imagem das apis publicadas no hub docker
https://hub.docker.com/u/alexandreceti   

---
### IdentityApi = dotnet
Api Source:
https://github.com/alexandreceti/IdentityApi  

imagem: alexandreceti/identity  
``` 
docker run -it --rm --name ident01 -p 5001:5001 alexandreceti/identity
```
http://localhost:5001/swagger/index.html

### docker-compose
Url Teste:
http://localhost:8080/IdentityApi/v1/Identity/tokenvalido/1

### Kubernetes
Url teste:
http://localhost:30080/IdentityApi/v1/Identity/tokenvalido/1

---

### OrderingApi = Node.js   

Api Source:
https://github.com/alexandreceti/OrderingApi  

image: alexandreceti/ordering   
```
docker run -it --rm --name ordering01 -p 8080:8080 alexandreceti/ordering 
```

Url teste:
http://localhost:8080/OrderingApi/v1/orders

### docker-compose
Url teste:
http://localhost:8080/OrderingApi/v1/orders


### Kubernetes
Url teste:
http://localhost:30081/OrderingApi/v1/orders

---

### BasketApi = Node.js

Api Source:
https://github.com/alexandreceti/BasketApi

image: alexandreceti/basketapi   
```
docker run -it --rm --name basket01 -p 8080:8080 alexandreceti/basketapi   
```

Url teste:
http://localhost:8080/basketapi/v1/basket
http://localhost:8080/swagger

### docker-compose
Url teste:
http://localhost:8080/basketapi/v1/basket


### Kubernetes
Url teste:
http://localhost:30080/basketapi/v1/basket

----
### CatalogApi = Python

Api Source:
https://github.com/bylucasxdx/CatalogApi

image: alexandreceti/catalog   
```
docker run -it --rm --name catalog01 -p 8080:8080 alexandreceti/catalog 
```

Url teste:
http://localhost:8080/bylucasxdx/CatalogApi/1.0.0/ui/

### docker-compose
Url teste:
http://localhost:8080/bylucasxdx/CatalogApi/1.0.0/ui/


### Kubernetes
Url teste:
http://localhost:30080/bylucasxdx/CatalogApi/1.0.0/ui/

----

###  Marketing = Python 
Api Source:
https://github.com/bylucasxdx/MarketingApi

Image: alexandreceti/marketing
```
docker run -it --rm --name marketing01 -p 8080:8080 alexandreceti/marketing
```
Url teste:
http://localhost:8080/bylucasxdx/MarketingApi/1.0.0/ui/

### docker-compose
Url teste:
http://localhost:8080/bylucasxdx/MarketingApi/1.0.0/ui/


### Kubernetes
Url teste:
http://localhost:30080/bylucasxdx/MarketingApi/1.0.0/ui/

----

### Locations = php

Api Source:
https://github.com/bylucasxdx/MarketingApi   

Imagem: alexandreceti/locationsapi   
```
docker run -it --rm --name location01 -p 8080:80 alexandreceti/locationsapi   
```

Url teste: http://localhost:8080/index.php/bylucasxdx/LocationsApi/1.0.0/localizacoes


### docker-compose
Url teste:
http://localhost:8080/index.php/bylucasxdx/LocationsApi/1.0.0/localizacoes


### Kubernetes
Url teste:
http://localhost:30080/index.php/bylucasxdx/LocationsApi/1.0.0/localizacoes

