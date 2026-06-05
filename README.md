# DVOP 400 Final Project

Personal portfolio website created for **DVOP 400 - DevOps I Final Project**.

This repository demonstrates the use of Git, GitHub, Docker, branching strategies, and containerized web application deployment.

---

## Purpose of the Repository

The purpose of this repository is to practice and demonstrate:

- Using Git to track changes to a project
- Using GitHub for repository management
- Working with feature branches and a develop branch
- Creating and managing Pull Requests
- Building and running applications with Docker
- Deploying a web application through a containerized environment
- Demonstrating DevOps concepts learned throughout the quarter

This website was developed using HTML, CSS, and JavaScript and then containerized using Docker and Nginx.

---

## Git Setup and Workflow Steps

The following steps were completed during development:

1. Created a new GitHub repository named **DVOP400-FinalProject**
2. Cloned the repository to the local machine
3. Created a local develop branch
4. Created and switched to a feature branch named **feature/final-project**
5. Added website files and project assets
6. Staged project files using:

```bash
git add .
```

7. Created commits with descriptive commit messages:

```bash
git commit -m "Complete final project website and Docker setup"
```

8. Connected the local repository to GitHub
9. Pushed local branches to GitHub
10. Created a Pull Request to merge the feature branch into the develop branch

---

## Website Features

The website includes:

- Home Page
- About Me Page
- Resume Page
- Project 1 Page
- Project 2 Page
- Project 3 Page

### Home Page

Introduces visitors to the website and provides navigation to the remaining pages.

### About Me Page

Includes:

- Personal biography
- Educational background
- AWS Certified Cloud Practitioner certification
- Professional interests
- Personal photograph

### Resume Page

Includes:

- Professional experience
- Educational history
- Certifications
- Technical skills
- Career objectives

---

## Project Files

```text
DVOP400-FinalProject
├── index.html
├── about.html
├── resume.html
├── project1.html
├── project2.html
├── project3.html
├── styles.css
├── script.js
├── Dockerfile
└── README.md
```

---

## Docker Containerization

The website was containerized using Docker and hosted using Nginx.

### Dockerfile Responsibilities

The Dockerfile performs the following actions:

- Uses the Nginx Alpine base image
- Copies website files into the Nginx web directory
- Applies proper file permissions
- Exposes port 80 for web traffic

### Build the Docker Image

```bash
docker build -t dvop400-finalproject .
```

### Run the Container

```bash
docker run -d -p 8080:80 --name dvop400 dvop400-finalproject
```

### Verify Running Containers

```bash
docker ps
```

### Access the Website

Open a web browser and navigate to:

```text
http://localhost:8080
```

---

## Manual Deployment Process

The website can be manually deployed through Docker using the command line.

### Stop the Container

```bash
docker stop dvop400
```

### Remove the Container

```bash
docker rm dvop400
```

### Rebuild the Image

```bash
docker build -t dvop400-finalproject .
```

### Launch a New Container

```bash
docker run -d -p 8080:80 --name dvop400 dvop400-finalproject
```

This process allows updates to be deployed after changes are made to the website source files.

---

## Challenges Encountered

Several challenges were encountered during development:

- GitHub authentication required the use of a Personal Access Token (PAT)
- Docker initially returned a 403 Forbidden error caused by file permission issues
- Website navigation required updates to support all project pages
- Resume content needed to be converted into HTML format
- Docker container testing was required to verify successful deployment

These issues were resolved through troubleshooting, configuration changes, and testing.

---

## DevOps Concepts Demonstrated

- Version Control with Git
- GitHub Repository Management
- Branching Strategies
- Pull Requests
- Source Control Workflows
- Docker Containerization
- Nginx Web Hosting
- Manual Deployment
- Application Packaging
- Troubleshooting and Debugging
- Continuous Integration Concepts
- Deployment Automation Concepts

---

## Author

**Jackson Hanks**

AWS Certified Cloud Practitioner

DevOps Student

Spokane Community College
