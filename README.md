# takeHomeWebDriverTest
This repository contains tests and framework created specifically for https://github.com/Dotdashcom/take-home-webdriver-test

1. This is a Maven Project which contains TestNG annotations
2. Use 'mvn test' to run all tests in command line from the project path

Note :
1. test7_DynamicContent : This test not always pass. This is because the webpage does not always change the images when refreshed. This results in an actualy failure. If the image checking is not required, please comment the Assert for the same.
2. test5_DragAndDrop : The dragAndDrop functionality from Selenium Actions does not work on HTML5. This is a known issue and no amount of workaround is working here from Selenium. Hence the test uses JavaScript to move the objects.
3. test8_DynamicControls : This test does not explicitly wait for the loading symbol to disappear when checking for enable and disable. There is a bug in the application where 2 loading images are displayed at a time. Hence for Enable and Disable, the test uses the explicit wait on Alert Message instead.
