# POC5_TDD_Jacoco_sonarQube
Test Driven development, Code coverage, Jacoco - Java Code coverage, Overview of Sonarqube - and hand-on basic implementation

# Resources - 
1. https://github.com/in28minutes/clean-code
2. https://argusoft.udemy.com/course/learn-tdd-in-java/learn/lecture/6669834#overview

# SonarQube - install and run

##  Option 1 - worked for me - Try Out SonarQube
As latest sonarQube version supports on java 11 for java 8 use sonarqube-6.7 
sudo docker run -d --name sonarqube -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube:6.7
---Opt2 - Install SonarQube using Docker on Ubuntu 18.0.4

## Working with SonarQube
---If required add maven dependency
---start oracle container - 
---sudo docker run -d --name sonarqube -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube:6.7
-sudo docker start sonarqube
---Open  - http://localhost:9000/projects/create
---Login to site- id-admin , pass- admin

## mvn clean verify sonar:sonar 
token - 2ef672a0462be6cfa62208b2489bac126859fd93
maven command - mvn sonar:sonar \-Dsonar.host.url=http://localhost:9000 \-Dsonar.login=2ef672a0462be6cfa62208b2489bac126859fd93
sudo docker stop sonarqube
