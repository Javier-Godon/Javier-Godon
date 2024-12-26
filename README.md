### About Me ➡️

As someone passionate about programming since childhood, I love dedicating part of my free time to exploring new languages, architectures, and fields within software development.
In my repositories, you will find projects in various programming languages, proof-of-concept implementations, and configurations for continuous delivery.


### My Goals 
I hope this can be a useful resource for working with and configuring projects in various programming languages or platform engineering tools. My repositories are intended to serve as a reference for anyone facing challenges while building with these technologies.

Additionally, collaboration is always welcome—whether through feedback, suggestions, or contributing new developments!

### Technologies I Use

#### Platforms and Tools
<img src="./images/crossplane-logo.png" alt="Dagger Logo" width="20" height="20"> ![Crossplane](https://img.shields.io/badge/Crossplane-Managed%20Resources-blue)
![ArgoCD](https://img.shields.io/badge/ArgoCD-GitOps-orange?logo=argo)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-blue?logo=githubactions)
<img src="./images/sealed-secrets-logo.png" alt="Dagger Logo" width="20" height="20">![Sealed Secrets](https://img.shields.io/badge/Sealed_Secrets-Encrypted_Secrets-green)
<img src="./images/tekton-logo.png" alt="Dagger Logo" width="20" height="20"> ![Tekton](https://img.shields.io/badge/Tekton-CI%2FCD-orange)
![Docker](https://img.shields.io/badge/Docker-Container-blue?logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue?logo=kubernetes)
<img src="./images/kcl-logo.jpeg" alt="KCL Logo" width="20" height="20"> ![KCL](https://img.shields.io/badge/KCL-constraint%20based%20record%20&%20functional%20language%20-green)
<img src="./images/dagger-favicon.png" alt="Dagger Logo" width="20" height="20"> ![Dagger](https://img.shields.io/badge/Dagger-Pipelines-black)


#### Programming Languages and Frameworks
<img src="./images/openjdk-logo.png" alt="Kafka Logo" width="20" height="20">![Java](https://img.shields.io/badge/Java-Programming-red)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-Microservices-green?logo=springboot)
![Python](https://img.shields.io/badge/Python-Scripting-yellow?logo=python)
![Go](https://img.shields.io/badge/Go-Programming-blue?logo=go)
![Elixir](https://img.shields.io/badge/Elixir-Functional-purple?logo=elixir)
<img src="./images/phoenix-logo.png" alt="Phoenix Logo" width="20" height="20">![Phoenix](https://img.shields.io/badge/Phoenix-Web_Framework-orange)

#### Infrastructure
![PostrgreSQL](https://img.shields.io/badge/PostgreSQL-SQL-blue?logo=postgresql)
![Java](https://img.shields.io/badge/MongoDB-No%20SQL-green?logo=mongodb)
<img src="./images/kafka_White on Transparent.png" alt="Kafka Logo" width="20" height="20">![Kafka](https://img.shields.io/badge/Apache%20Kafka-distributed%20event%20streaming-white)
<img src="./images/questdb-logo.png" alt="Questdb Logo" width="20" height="20">![Questdb](https://img.shields.io/badge/Questdb-time%20series-purple)

### How to use it 📘

There is a repository dedicated to deploying some of the services on Kubernetes: [Cluster Continuous Delivery](https://github.com/Javier-Godon/cluster-continuous-delivery). 

This repository demonstrates how to implement a CI/CD pipeline using Dagger, GitHub Actions, and ArgoCD, utilizing KCL as a configuration and policy language. It provides an example of how to integrate and combine all these technologies, making it easier to understand their use in a global context. 

- **Dagger** simplifies the design of pipelines, enabling execution with any tool (Jenkins, GitHub Actions, Tekton, etc.) without requiring modifications or adaptations. You can even run them locally—yes, you can test them on your local machine! A program written in your favorite language abstracts away the tooling concerns, avoiding migration issues.  

- **KCL** replaces Helm/Kustomize, offering dynamic configurations ([KCL Documentation](https://www.kcl-lang.io/docs/user_docs/getting-started/intro)). For example, changing the tag of your image in the deployment repositories becomes straightforward and doesn't rely on any specific framework.

Although I use GitHub Actions for my CI/CD, the repository includes a fully functional example of a Tekton pipeline without Dagger. The proposed solution generates Kubernetes manifests directly in YAML, allowing you to use any GitOps tool without issues or additional adaptations. Forget plugins—you won't need to adjust the tool to work with KCL!

This repository also contains all the infrastructure necessary for various projects to run on Kubernetes. It is deployed using [Crossplane](https://www.crossplane.io/), and you'll find the required manifests and CRDs for each deployment.


### Proofs of Concept

This section highlights some of the proofs of concept I’ve developed to explore different architectures, frameworks, and use cases.

- **[ERP System in Go](https://github.com/Javier-Godon/erp-back)**  
  A proof of concept demonstrating how to implement an ERP system using Go. This project explores different architectures and frameworks within the Go ecosystem.

- **Video Streaming with Apache Kafka**  
  This proof of concept tackles the challenge of streaming videos from multiple sources continuously, ensuring reliable delivery. The solution includes three Python-based components:  
  - [**Video Server**](https://github.com/Javier-Godon/kafka-video-server-python): Splits videos into chunks and sends them to Apache Kafka.  
  - [**Consumer with MongoDB**](https://github.com/Javier-Godon/kafka-video-consumer-mongodb-python): Receives chunks and stores them as JSON documents in a MongoDB database, leveraging MongoDB's flexible design.  
  - [**Video Collector**](https://github.com/Javier-Godon/video-collector-mongodb-python): Reconstructs a specific video from stored chunks and generates the requested video.  

- **[Java/Spring Boot](https://github.com/Javier-Godon/ddd-hexagonal-vertical-slice-cqrs-reactive-kubernetes)**  
  A proof of concept designed to experiment with different architectures and reactive programming styles. This project implements a simple Pokédex and includes instructions for running it locally. Additionally, it can be used to test the proposed CI/CD pipeline for a Java/Spring Boot project.




