Create a base image of Jenkins 2.7.3 with 
* SonarQube plugin installed (compatible with pipeline) and all required plugins
* Maven tool preinstalled (version 3.2.5)
* Java tool preinstalled (version 8)
* no configuration of SonarQube installation
* no installation of SonarQube scanner tools
* an empty freestyle project
* an empty pipeline project

To build this image:
```docker build -t test-sonarqube-jenkins-pipeline:jenkins2-base .```

To run:
```docker run --rm -p 2222:2222 -p 8080:8080 -p 8081:8081 -p 9418:9418 -ti test-sonarqube-jenkins-pipeline:jenkins2-base```
