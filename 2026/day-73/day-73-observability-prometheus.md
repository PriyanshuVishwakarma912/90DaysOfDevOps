## Task 1: Understand Observability
## 1. What is observability? How is it different from traditional monitoring?
  - Observability is a concept in DevOps & SRE that tell you what is happening,why it is happened and how it is happened inside a system/application/server by looking at its output like metrices,logs & traces.
  - Monitoring is a concept that tell you something is going on in your application/system/server.
  - In past we have monolithic apps (one big piece of software on one server). Today, we have Microservices and Cloud (hundreds of small pieces running across many servers/containers).Traditional monitoring was built for the old way; Observability was built for the new way.
## 2. What are the three pillars of observability?
  - The three pillars of observability are :
  - (a): **Metrices**: Metrice tells ' what ' is happend in your application/server.
    - Like CPU is at 80% usage, 500 requests/sec , Memory increased by 10%.
    - Tools Used: Prometheus, Datadog, CloudWatch
  - (b): **Logs**: Logs tells you why it is happened in your application/server.
    -   
