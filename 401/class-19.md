# Read 19 - AWS: Events

## Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

both Express and Serverless can be used for writing Node.js APIs, with ExpressJS Server we can set up the routes and implement the functionality for them. With AWS API Gateway, we set up the routes and then implement the functionality with lamda functions.

## List the AWS Database offerings and talk about the pros and cons of each

Types of offers :

* Relational
* Key-value
* In-memory
* Document
* Wide column
* Graph
* Time series
* Ledger

>Pros : Automated Patching, Automated Backups, Integrated with the rest of the AWS ecosystem
>Cons: Zero data loss is not guaranteed, No root access to the server, Downtime required for scaling operations

## What’s the difference between a FIFO and a standard queue?

A FIFO queue is first in first out and a standard queue provides at least once delivery and isn’t neccessarily ordered.

## How can the server be assured a message was properly received?

Logging and using timestamps and checking whether it was delivered based on the response sent from the endpoint.
