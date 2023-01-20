# Welcome to json-rpc-jmeter test suite
[![CircleCI](https://circleci.com/gh/rsksmart/json-rpc-jmeter/tree/master.svg?style=svg)](https://circleci.com/gh/rsksmart/json-rpc-jmeter/tree/master)



# About
Based on [jmeter-maven-plugin](https://github.com/jmeter-maven-plugin/jmeter-maven-plugin), this is a Test Suite for JSON RPC compatibility validation of [RSKj](https://github.com/rsksmart/rskj).

It's implemented using Apache JMeter and test [every JSON RPC method](https://developers.rsk.co/rsk/node/architecture/json-rpc/) validating response format and content.

This is still a BETA but it's fully functional and tests can be incorporated.


# Getting Started
Prerequisites:
- Maven 

Instructions to run the tests:
- Clone this repository
- mvn verify

Detailed results report will available in ./Results/JSON-RPC/index.html
This repository also includes CircleCI configuration for workflows on commit/builds and daily job.


Running the GUI
-----

To create or update new jmeter test cases, open the file ```src/test/jmeter/JSON-RPC.jmx``` in the JMeter GUI.

To invoke the JMeter GUI, use the following command:

```
mvn jmeter:configure jmeter:gui
```

See the associated [Wiki](https://github.com/jmeter-maven-plugin/jmeter-maven-plugin/wiki/Basic-Configuration#running-the-jmeter-gui) entry for more information.