Create a running multi-container Docker applications with
* Jenkins 2.7.3 (available at http://localhost:8080) with 
  * SonarQube plugin installed (compatible with pipeline) and all required plugins
  * Maven tool preinstalled (version 3.2.5)
  * Java tool preinstalled (version 8)
  * 2 SonarQube installations
  * 2 SonarQube scanner tools installations
  * 2 SonarQube scanner for MSBuild tools installations
  * an empty freestyle project
  * an empty pipeline project
  * a pipeline project: ```SONARJNKNS-253``` to validate [SONARJNKNS-253 - Make Inject SonarQube environment (SonarBuildWrapper) compatible with pipeline](https://jira.sonarsource.com/browse/SONARJNKNS-253)
  * a pipeline project: ```SONARJNKNS-252``` to validate [SONARJNKNS-252 - Make SonarQube Scanner step compatible with pipeline](https://jira.sonarsource.com/browse/SONARJNKNS-252)
  * a pipeline project: ```SONARJNKNS-254``` to validate [SONARJNKNS-254 - Make MSBuild Scanner steps compatible with pipeline](https://jira.sonarsource.com/browse/SONARJNKNS-254)
* an empty SonarQube 6.0 (available at http://localhost:9000)
* an empty SonarQube 6.0 (available at http://localhost:9001)

To use it you need to [install Docker Compose](https://docs.docker.com/compose/install/)

To run:
```docker-compose up```
