# Examples

This directory contains examples of how to use the Docker Compose file format.

## Getting Started

To run the examples, you need to install Docker and Docker Compose.

### Installing Docker

To install Docker, follow the instructions on the [Docker website](https://docs.docker.com/install/).

### Installing Docker Compose

To install Docker Compose, follow the instructions on the [Docker Compose website](https://docs.docker.com/compose/install/).

## Running the examples

To run the examples, you need to clone the repository and run the following command:

``` bash
docker-compose -f <file-example> up
```

## Examples

| Logo   | Type       | docker-compose                           |
| :---------- | :--------- | :---------------------------------- |
| <p align="center"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Logo-redis.svg/1200px-Logo-redis.svg.png" alt="redis" width="130"/></p> | `database` | [redis-compose.yaml](redis-compose.yaml) |
| <p align="center"><img src="https://devtools.com.br/blog/wp-content/uploads/2013/06/MySQL-Logo.wine_.png" alt="mysql" width="130"/></p> | `database` | [mysql-compose.yaml](mysql-compose.yaml) |
| <p align="center"><img src="https://connectoricons-prod.azureedge.net/releases/v1.0.1597/1.0.1597.3005/amazonsqs/icon.png" alt="sqs" width="80"/></p> | `queue`,`localstack` | [sqs-compose.yaml](sqs-compose.yaml) |
| <p align="center"><img src="https://miro.medium.com/max/300/0*tp2NggIKEiYbXd7o.png" alt="dynamodb" width="80"/></p> | `database`,`localstack` | [dynamodb-compose.yaml](dynamodb-compose.yaml) |
| <p align="center"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQaZpxLWLXFq5S3_hH5mP9GGhmMuPw0LMJGAMRqODQx5oeLSNNSig8BlQ5gYBXlBE43Od0&usqp=CAU" alt="kafka" width="100"/></p> | `messaging system` | [kafka-compose.yaml](kafka-compose.yaml) |
| <p align="center"><img src="https://g.foolcdn.com/art/companylogos/square/mdb.png" alt="mongodb" width="100"/></p> | `database`, `nosql` | [mongodb-compose.yaml](mongodb-compose.yaml) |

## Projects using Docker Compose

- [Twitter Microservices](https://github.com/jjeanjacques10/twitter-microservices)
- [Hibredu App](https://github.com/hibredu/hibredu-app)
- [Single Table Design + Spring Boot](https://github.com/jjeanjacques10/spring-dynamodb-single-table-design)