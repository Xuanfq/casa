# casa
A service for configuration and service management base on nacos.


## Usage
- directory introduce
```
compose/image: source code of the docker image
compose/env: Environment variable file for compose yaml
compose/compose: Docker compose for casa  # refer image & env
```

- example of virtual cluster (non production env)
```
cd casa-docker
docker-compose compose/casa-cluster-ip-vir-mysql5.7.yaml up
```

- single point of cluster
```
cd casa-docker
# run to start the mysql if you don't have a database
# docker-compose compose/casa-cluster-ip-singlepoint-mysql5.7.yaml up
docker-compose compose/casa-cluster-ip-singlepoint-nacos.yaml up
```

- Others reference: `cd nacos-docker-2.3.2`


## API
- [Open-API](https://nacos.io/zh-cn/docs/open-api.html)
