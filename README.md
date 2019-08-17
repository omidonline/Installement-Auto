# Installment_Auto_

A lite framework to run Installment Plan REST api automation scripts created by Postman.

## Getting Started

This lite framework allows the user to run the Postman Collections from a command line. The input to the framework is a configuration file where you can define your test cases, variables and where to send the email.

### Prerequisites

You need to have the following installed:
 1) npm
 2) newman (npm install -g newman)
 3) newman-report-htmlextra (npm install -g newman-report-htmlextra)

Once you finished writing your test scripts in Postman, you need to export the "Collections", "Global Variables" and "Local Variables" to "Tests/Collections" and "Tests/Environment" directories.

### Installing

This script doesn't required any installation.

## Running the tests

cd scripts
python runTest.py --config=../Tests/Config/myconfig.json --testcase=SMOKETEST

### How does it work

Once your run the test, the script will:
  1) Verifies the format of the Configuration file
  2) Replaces Variables
  3) Selects the TestCase
  5) Runs newman script
  6) Create .html, .log, .xml files in Test/Reports/<date> directory
  7) If sendMail is set to True, then it will email the HTML report to the contacts.

## Deployment

git clone <>


## Authors

[contributors]
  1) Omid Fatehi (ofatehi@visa.com)
  2) Far.....

## License

This project is licensed under the Visa License 

## Acknowledgments

* Thanks for everyone who helped. *

