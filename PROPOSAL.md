# CLC3 Project: OpenTelemetry & Jaeger Showcase

authors: Heckmann & Niederländer

## PROPOSAL

The goal is to implement a sample application consisting of three microsservices and one webUI (python with django) instrumenting them with openTelemetry in order to be able to retrieve tracing information on how the services communicate with each other. The microservices will be written in Node.js (two services) and python (one service) to be able to display a variety of openTelemetry-language-sdks and then will be deployed using Kubernetes in Azure. In order to retrieve "interesting" results the microservices will have to be written so that they call each other and therefore different scenarios (e.g. certain service currently not available) should generate different results.

In order to display the gathered tracing information jaeger will be deployed with Kubernetes as well and then utilized to show the communication results of microservices. The application/ microservices will be implemented to support a variety of scenarios like different REST-Responses, failed method calls/ exceptions, long response times etc. which will then presented in the final live demo utilizing the jaeger ui.

## MILESTONES & RESPONISIBILITIES

### Milestones

1. Set up Azure Kubernetes Service
2. Write dummy micoservices in Node.js and Python with openTelemetry Instrumenation
3. Deploy microservices in Azure Kubnetes Service
4. Deploy up jaeger in AKS
5. Setup live demo

### Responsibilities

Heckmann - Write and Deploy Microservice + WebUI Python, Deploy Jaeger

Niederländer - Set up AKS, Write and Deploy Microservices Node.js


## ARCHITECTURE



Note: We won't be covering anything in terms of user authorization etc. since it is clearly not part of scope of the course.

