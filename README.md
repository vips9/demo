### Cengage Nglsync Automation

#### System Requirement:

* JDK 1.6 or above
* Maven 3.1 or above
* Eclipse IDE or any other of choice in case there is need to update the script. (optional)
* For execution of scripts on Chrome you need to have executable files for both drivers respectively and paste them at location "\src\test\resources\drivers" in project folder.

#### Execution Steps:
Please follow the instructions to execute the tests on local:

1. Checkout the code from Stash
2. To add execution parameters use following command
	mvn clean verify -DxmlFile="NameOfXMLFile.xml" -Dtier="environment" -Dbrowser="browserName" -Dseleniumserver="RemoteOrLocal" -Dseleniumserverhost="seleniumServerIP" 
	
All these parameters also have a default value present in config file, with default recipients in data YML file

#### Test Execution Result Files:	
The Test Execution Results will be stored in the following directory once the test has completed

    ./target/cucumber-html-report/index.html (for cucumber feature execution results)
