# selenium-automation-practice

Author: kishork163@gmail.com

Description: A comprehensive project showcasing web UI test automation using Selenium and Cucumber. This includes writing scenarios following Behavior driven methodology using Cucumber.

Note: This project has been created using:

Java: 1.8

Maven: 3.6

Spring

Chrome: Version 79.0.3945.130 (Official Build) (64-bit)

OS: Windows 8.1

Instructions to run tests:
1. Launch a command prompt. 
2. Execute command git clone https://github.com/kikumar3189/selenium-automation-practice.git OR download the zip from https://github.com/kikumar3189/selenium-automation-practice
3. Simply execute command : mvn clean test 
4. This will start executing scenarios by using chrome browser.
5. Two scenarios will be executed: Order T Shirt and Update first Name.
6. On Test completion, open file target/index.html in a browser to view test results.
7. This project also includes support to run the tests in headless mode, simply pass a maven command line property mvn clean -Dheadless=true test .
8. Project supports maintaining all application objects in an XML file src/main/resources/ObjectRepository.xml . Even non technical users can add/update application objects in XML file. These application objects can then be referenced directly in feature file and corresponding location properties are picked up by step definitions at run time.
  
Possible Enhancements:
1. More browsers support can be added to DriverFactory class and a browser can be selected at run time by passing a mvn command line property like mvn -Dbrowser=IE test.

2. A variables file can be created storing the variables which needs to be reused in multiple tests. Variables can be General or feature specific. This will allow all static test data values to be managed at a single location. E.g. If username is used in multiple features them having it stored in a central location will ease maintenance of tests. All features should refer to username from variables file.

3. Multipe maven profiles can be created where each profile will refer to a specific application environment. This way tests can be executed in any environment by passing maven profile from command line. e.g mvn clean -Pdev test.

4. An email notification can be added which will include basic test execution summary, Count of total, passed, failed, skipped scenarios. Time taken etc. This will help to intimate users when tests are running in a continous integration server like Bamboo, Jenkins.

Above list is never ending but these five enhancements would add a lot of value to users .
