# kafka-demo-app

## overview

![image](/docs/image/image.png)

This project is mock-up project for testing apm-instrument-operator.

## Project Structure

- `/docs` : project documentation
- `/app/$(app-name)` : application source code
- `/app/$(app-name)/Dockerfile` : application dockerfile
- `/deploy` : kubernetes deployment helm chart

## Components

- `kafka` : kafka cluster
- `kafka-demo-app` : kafka producer python application producing fake stock data to kafka
- `kafka-stream` : kafka stream application generating moving average of stock data
- `kafka-connector` : kafka connector to redis
- `redis` : redis (destination of kafka-connector)
