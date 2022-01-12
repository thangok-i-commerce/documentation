# I-Commerce system documentation

## 0/ Introduce
We planned to build an e-commerce system that play as a market role, 
where Customer and Shop meet each others, and shopping experience happen

Shop Administrator can log-in, manage their product, brand, category, price

Customer can search for needed product, add to cart, and place an order

We build this system using Micro-Service Architecture approach.

In order to easily scale our system, we use Saga Orchestration pattern, 
with Spring Web Flux to provide a Reactive-Base Order Management Service,
which optimize computing resource, and easily scale when more and more customer come day by day.

## 1/ Overview

![](i-commerce-system-component.drawio.png)

In this system, whole back-end is a large heart where the business happen.

Back-end system provide the world capability to interact with it, by expose Open API Restful specification.

Also, we integrated with 3rd party to use the online payment capability in the future.

##