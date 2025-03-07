# REST Services Examples

This repository contains multiple examples of RESTful services using different frameworks and languages. Each project is stored as a **Git submodule**, so you can clone only the one you need.

## **Projects Included**
Each of these subdirectories is a separate project:

| Project Name | Description |
|-------------|------------|
| [Liberty-Microprofile-Rest-Service-Example](https://github.com/Dimitris-Kaler/Liberty-Microprofile-Rest-Service-Example) | REST service using Liberty and MicroProfile |
| [Node-Express-Example](https://github.com/Dimitris-Kaler/Node-Express-Example) | Example REST service using Node.js with Express |
| [Quarkus-Microprofile-REST-service-example](https://github.com/Dimitris-Kaler/Quarkus-Microprofile-REST-service-example) | RESTful service with Quarkus and MicroProfile |
| [Simple-Spring-Boot-REST-Service-Example](https://github.com/Dimitris-Kaler/Simple-Spring-Boot-REST-Service-Example) | REST API using Spring Boot |
| [simple-node-rest-example](https://github.com/Dimitris-Kaler/simple-node-rest-example) | Another example of a simple Node.js REST service |

---

## **How to Clone This Repository**
Since this repository uses **Git submodules**, you need to initialize them when cloning.

### **Clone Everything (Main Repo + Submodules)**
Run the following command:
```bash
git clone --recurse-submodules https://github.com/yourusername/main-repo.git
```
If you've already cloned the main repository without submodules, initialize them manually:

```bash
git submodule update --init --recursive
```

--- 

## How to Work with Individual Submodules
If you only want a specific project, navigate into that folder and initialize just that submodule.

```bash
cd Node-Express-Example
git submodule update --init
```
Each submodule is a separate Git repository, so you can navigate into it and work with it normally:
```bash
cd Node-Express-Example
git pull origin main  # Update to the latest version of the submodule
```