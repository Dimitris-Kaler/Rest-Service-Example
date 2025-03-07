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

## Updating Submodules
If you want to update all of your submodules to their last commits from the remote repositorie,use the following commnad:
```bash
git submodule update --remote --recursive
```

This command updates all the submodules to their latest version available from the remote repository. The --remote option fetches the latest commit from the remote origin of each submodule, while `--recursive` ensures that submodules within submodules are also updated, if any.

- `--remote`: This tells Git to fetch the latest changes from the remote repository for each submodule, rather than just checking out the commit specified in your main repository.

- `--recursive`: This flag makes sure that any nested submodules (submodules within submodules) are also updated to the latest version.

This is useful when you want to ensure all submodules in the repository are up to date with the latest changes from their respective remote sources.