# Flask CI/CD Pipeline using Jenkins

## Overview

This project demonstrates the implementation of a CI/CD pipeline for a simple Flask application using Jenkins. The pipeline automates the process of building, testing, and deploying the application whenever changes are pushed to the repository.

Since no repository was provided, a minimal Flask application was created for this implementation.

---

## Repository

https://github.com/ARthakkar92/flask-cicd-app

---

## Jenkins Pipeline

The pipeline is defined using a Jenkinsfile in the root directory and consists of the following stages:

* Build: Creates a virtual environment and installs dependencies using pip
* Test: Executes unit tests using pytest
* Deploy: Runs the Flask application if tests pass

---

## Trigger Configuration

The pipeline is configured using Poll SCM.

Jenkins checks the repository at regular intervals and automatically triggers a build when changes are detected in the main branch.

---

## Email Notifications

Email notifications are configured using SMTP settings.

Notifications are sent on:

* Successful builds
* Failed builds

---

## Testing

Unit tests are written using pytest.
The deployment stage is executed only if all tests pass successfully.

---

## Deployment

The application is deployed locally and can be accessed at:

http://192.168.56.101:8081/

---

## Screenshots

Include the following:

<img width="1414" height="667" alt="image" src="https://github.com/user-attachments/assets/00c10754-6e8f-4d1e-a899-f896e8757161" />


<img width="1366" height="537" alt="image" src="https://github.com/user-attachments/assets/d0ec8900-b603-43fc-a7bb-01e3d36aaa6f" />


<img width="1913" height="797" alt="image" src="https://github.com/user-attachments/assets/0656a30a-a205-4cce-93f1-14f7ad67d442" />


<img width="1856" height="816" alt="image" src="https://github.com/user-attachments/assets/00d8ff8d-652e-4e7c-867c-0b12345282a0" />


<img width="1884" height="818" alt="image" src="https://github.com/user-attachments/assets/38439c50-beaa-49d2-a24c-678a6268e970" />


<img width="1903" height="821" alt="image" src="https://github.com/user-attachments/assets/4defdf25-0b3e-4be4-b637-11a556ea175b" />


---

## Conclusion

This project demonstrates a complete CI/CD workflow using Jenkins, including automated build, test, deployment, and notifications.
