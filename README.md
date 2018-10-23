# docker-wso2am

Build a docker image for run a fully operational instance of WSO2 API Manager.

## Tags
- latest
- 260

## How to use
### docker run
`docker run -it \
-p 9443:9443 \
-p 8243:8243 \
-p 8280:8280 \
hackwish/wsoam:latest`

### docker-compose
``docker-compose -f docker-compose_dev.yml up``

##How to works
### Develop
*(Based on info: https://wso2.com/api-management/install/docker/get-started/)*

Once the container is started, access the following URLs on your favorite web browser using the credentials username: admin and password: admin.

**Publisher** - https://localhost:9443/publisher
**Store** - https://localhost:9443/store
**Admin console** - https://localhost:9443/admin
**Carbon console** - https://localhost:9443/carbon

Please note that the **WSO2 API Manager Gateway** will be available on the following ports.

https://localhost:8243
http://localhost:8280

