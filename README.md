### Tech Stack of Web Automation

1. Programming - Java ( JDK > 22, IntelliJ)
2. User Interactions, browser Automation Selenium
3. Test Framework -> TestNG
4. Build Management ->  Maven
5. Reporting - Allure Report, Extent Report.
6. Data Driven - DDT Apache POI.
7. CI / CD -> GIT, Jenkins
8. Coding Best Practice-  SonarLint
9. Logs - Log4j





## How to add Log4J in the Project ?
- Add this to the pom.xml
```<dependency>
      <groupId>org.apache.logging.log4j</groupId>
      <artifactId>log4j-core</artifactId>
      <version>3.0.0-beta2</version>
    </dependency>

    <!-- https://mvnrepository.com/artifact/org.apache.logging.log4j/log4j-api -->
    <dependency>
      <groupId>org.apache.logging.log4j</groupId>
      <artifactId>log4j-api</artifactId>
      <version>3.0.0-beta2</version>
    </dependency> 
```
- Add log4j2.xml in the main folder -> resource
- To your Code
```
-     private static final Logger logger = LogManager.getLogger(TestVWOLogin_PF_DM.class);
    
file
logger.info("Starting Test");

```
