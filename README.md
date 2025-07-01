# python-selenium-robot
Utilities and test scripts for automating web interactions using Selenium and Robot Framework in Python. This repo includes sample tests, libraries, and custom keywords to help kickstart any QA automation effort.

A web automation framework using Python, Selenium WebDriver, and Robot Framework. This project
supports reusable test components, cross-browser automation, and readable test cases using Robot
Framework syntax.

# Project Structure
python-selenium-robot/
├── config/ # Robot Framework test setup configuration
│ └── config.py
│
├── tests/ # Robot Framework test cases
│ └── login_tests.robot
│
├── resources/ # Reusable keywords and variables
│ ├── keywords.robot
│ └── variables.robot
│
├── libraries/ # Custom Python libraries
│ └── utils.py
│
├── drivers/ # WebDriver executables (e.g., chromedriver)
│
├── results/ # Test output and logs
│
├── requirements.txt # Python dependencies
├── README.md # Project overview and instructions
└── run_tests.sh / .bat # Scripts to execute tests
 Setup Instructions
Clone the repository
git clone https://github.com/your-username/python-selenium-robot.git
cd python-selenium-robot
Set up a virtual environment
1. 
1. 
1
python -m venv venv
source venv/bin/activate # Windows: venv\Scripts\activate
Install required packages
pip install -r requirements.txt
 Running Tests
To execute tests:
robot tests/
Or use the shell/batch scripts:
./run_tests.sh # Unix/macOS
run_tests.bat # Windows
 Sample Test Case
*** Settings ***
Resource ../resources/keywords.robot
*** Test Cases ***
Valid Login Test
 Open Browser To Login Page
 Input Valid Credentials
 Submit Login Form
 Verify Dashboard Is Visible
 Close Browser
1. 
2

