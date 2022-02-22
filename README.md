# Docker aws-cli

[![Project Status](https://img.shields.io/static/v1?label=project%20status&message=complete&color=success&style=flat-square)](#)

Proof of concept to demonstrate how to use aws-cli and localstack with docker.

## Requirements

[![docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)

## Installation

```bash
$ docker network create localstack
$ docker-compose up -d
```
    
## Usage

```bash
alias aaws='docker run --network localstack --env-file ./aws.env --rm -it amazon/aws-cli --endpoint-url=http://localstack:4566'
aaws s3 mb s3://poc
aaws s3 ls
```

## Tech Stack

[![docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![aws](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/)

## Reference

- https://localstack.cloud/
- https://hub.docker.com/r/amazon/aws-cli
- https://github.com/localstack/localstack/issues/3088

## Feedback

If you have any feedback, please contact me at raphaeldias.ti@gmail.com

[![github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/raphaelbh)
[![linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raphaelbh/)
