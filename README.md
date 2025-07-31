## Urban Routes Project

Daniela Malagon, Sprint 8

##Description

This project automates functional tests for the Urban Routes application using Python, Selenium, and Pytest under the Page Object Model (POM) pattern. The goal is to cover the complete flow for requesting a taxi in the application, ensuring that each step works correctly and that the user experience is stable and reliable.

Locators, methods, and automated tests were developed to simulate the actual process a user would follow. All tests were run in PyCharm, and the data.py file was used to manage configuration and test data, including the server URL, which must be updated before each run.

##Requirements
- Selenium
- Python
- pytest
- Servidor de Urban Routes

##Installation
1. Install Python
2. Download it from python.org and install it on your system.
3. Clone the repository: git clone <repository-URL>  cd <repository-name>
4. Install dependencies (Run in the terminal): pip install selenium pytest requests
5. Install ChromeDriver: Download it from chromedriver.chromium.org (Make sure it is in your PATH or in the project directory)
6. Configure the server URL: Open data.py and update the variable urban_routes_url with the active server URL, for example:
    urban_routes_url = "https://cnt-35bd9ac8-d7a6-43a8-a508-444759dd0ac3.containerhub.tripleten-services.com?lng=es"

##Included Automated Tests
1. Set the address
2. Select the Comfort fare
3. Enter the phone number
4. Add a credit card
5. Write a message for the driver
6. Request a blanket and tissues
7. Request 2 ice creams
8. Modal appears to search for a taxi
9. Wait for driver information to appear in the modal

##Instructions to Run the Tests
1. Make sure the server URL in data.py is updated and active.
2. Ensure ChromeDriver is installed and accessible.
3. Open a terminal in the root folder of the project.
4. Run the following command to execute all tests:
pytest main.py
   #If your tests are in a specific folder, use:
     pytest ruta/a/tu/test_file.py
   #For detailed results, add the -v option:
     pytest -v main.py

##Final Considerations
- If the web application changes its structure or language, review and update the selectors and expected values in the asserts.
- If a test fails, review the error messages and make sure the test data is valid and the server URL is available.
- It is recommended to verify other functionalities not covered before releasing the application to production.
