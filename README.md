# [LocalStack](https://localstack.cloud/) Playground

## Start a local stack 

* Provision a local aws stack with SQS service, and create two SQS queues

    ```bash
    docker-compose up setup-resources-localstack
    ```


* List all queues created

    ```bash
    docker exec -it foo-app-localstack /bin/sh -c 'aws sqs list-queues --endpoint-url http://localstack:4566'
    ```