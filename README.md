# Example
This is for example project
Playwright Testing Framework (Tpescript + Cucumber)
----------------------------------------------------
#What is it?#
This is Automated testing framework using Playwright and written in Typescrpit. It has been created to automate both API Testing and UI Testing.

#Approach#
The framework has been developed using Typescript and Cucumber. This has been developed BDD principles via cucumber using Gherkin format. Using Shared page object/Page Object model (POM) design principles. 

## 🧪 Tech Stack
- Playwright Test Runner
- TypeScript
- Cucumber - HTML reporting
- BDD Gherkin using Cucumber
- Axios

Step 1: Create Folder (Playwright)
Step 2: Install pre requisite softwares Node js, vs code
Step 3: Open folder in VS Code
Step 4: Install playwright -> npm init playwright@latest
Step 5: Adding Cucumber plugin Extension
Step 6: delete non related files (tests folder, playwright config)
Step 7: Install cucumber plugin -> npm i @cucumber/cucumber -D
Step 8: Cucumber to dynamically transpile TypeScript to JavaScript before running -> npm i ts-node -D

Step 9: Cucumber HTML Report -> Install npm install multiple-cucumber-html-reporter --save-dev

Folder structure:
---------------------
src\tests folder contains below,

cucumber.json -> This is  the configuration file for Cucumber in your project. It tells Cucumber how to find your feature files, step definitions, what modules to load, how to format reports, and other runtime options.













#Install Pre-Requisite Softwates#

Node.js - The framework requires Node.js version v22.17.0 and above
VS Code - Preferred IDE V1.101.2
Chrome Version: Version 137.0.7151.120
Version Control: Git
npm version: 

Install playwright using -> npm init playwright@latest
and choose below options while installing,
 Typescript

 Setup procedure in Local Machine:
 -------------------------------------

 Step 1: Check the pre requisite softwares in your local machine and install if anything is missing from the list.

 Step 2: Clone the project to your local system.

 Step 3: Open the project with IDE.

 Step 4: Install node module dependencies using 



#Create Project Folder and Open in VS Code:#

-> Create an empty project folder on your local machine.
-> Open VSCode in admin mode.
-> Go to File -> Open Folder and select the empty folder(Ex:Playwright)you created
-> Open a new terminal from the menu bar.
-> Select the GitBash or Command Prompt terminal

Git clone: 

Install playwright

#Navigation to step definitions directly from the feature file#

-> We can achieve this by clickin on any of the steps in feature file and then selecting one of these three options
        1. Holding Ctrl + Click
        2. Right clicking and selecting Go to Definition
        3. Pressing F12

    #### To make it enable this feature we need to install the Cucumber (Gherkin) Full Support Extension.    








File Structure and it's purpose:
-------------------------------------
src -> Library which contains feature files, Page objects, step definitons, utilities.

test-result -> Output library for screenshots and html-cucumber reports post run of test cases.

tsconfig.json -> It configures how TypeScript compiles and code, ensuring project runs smoothly with TypeScrip.

cucumber.json file -> This is Cucumber config file. Using this cucumber finds feature files, step definitions, what modules to load, how to format reports, and other runtime options.

package.json file -> Manages project dependencies, scripts and metadata which is essential for installing, running framework.

package-lock.json -> Works together with package.json to manage project dependencies reliably. 

Key Files:
-----------
pageObjects: A .ts file has been created for both UI (saucedemo) and API (petstore). Within the file it holds a central repository for all the web elements and methods.
Location: .\src\test\pageObjects

feaures: A .feature file has been created for both UI and API tests as per BDD Gherkin format
Location: .\src\test\features\api -> for api feature file,
          .\src\test\features\ui -> for ui feature file

steps: This contains step definition files which are glue between Gherkin feature files and actual test code.
Location: .\src\test\steps

utilities: It contains shared helper functions or modules to reuse across tests, step definitions, page objects. (DRY Principle)
Location: .\src\test\utilities

reports: Once the test execution completes a html-cucumber report will be generates within this folder.
Location: .\src\test-result\reports

screenshot: To take screenshots once the test case execution completes and stores here.
Location: .\src\test-result\screenshots




See `test-explanation.md` for test design and reasoning.

Author: Sivaramakrishna Perla
