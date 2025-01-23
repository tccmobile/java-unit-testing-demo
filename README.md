# Java Unit Testing Demo

This repository demonstrates unit testing in Java using JUnit. It includes a simple `Calculator` class and corresponding unit tests to validate its functionality.

## Project Structure
```
java-unit-testing-demo/
├── src/
│ ├── main/
│ │ └── java/
│ │ └── com/
│ │ └── example/
│ │ └── Calculator.java
│ └── test/
│ └── java/
│ └── com/
│ └── example/
│ └── CalculatorTest.java
├── .devcontainer/
│ ├── devcontainer.json
│ └── Dockerfile
├── pom.xml
└── README.md
```

## What are Unit Tests?

Unit tests are automated tests written and run by software developers to ensure that a section of an application (known as the "unit") meets its design and behaves as intended. In this project, the unit tests are written using JUnit, a popular testing framework for Java.

### Calculator Class

The `Calculator` class has two methods:
- `add(int a, int b)`: Adds two integers and returns the result.
- `subtract(int a, int b)`: Subtracts the second integer from the first and returns the result.

### CalculatorTest Class

The `CalculatorTest` class includes the unit tests for the `Calculator` class:
- `testAdd()`: Tests the `add` method to ensure it correctly adds two integers.
- `testSubtract()`: Tests the `subtract` method to ensure it correctly subtracts one integer from another.

## Using GitHub Codespaces

This repository is configured to use GitHub Codespaces for development. The `.devcontainer` directory contains the necessary configuration files.

### Steps to Use GitHub Codespaces

1. **Create a new Codespace**:
   - Click on the `Code` button in the repository and select `Create codespace on main`.

2. **Run the tests in the Codespace terminal**:
    ```sh
    mvn test
    ```
### Expected Output

If the tests are successful, you should see output similar to the following:
```
[INFO] Scanning for projects...
[INFO]
[INFO] -----------------< com.example:java-unit-testing-demo >-----------------
[INFO] Building java-unit-testing-demo 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:3.1.0:resources (default-resources) @ java-unit-testing-demo ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /path/to/your/project/src/main/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ java-unit-testing-demo ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /path/to/your/project/target/classes
[INFO]
[INFO] --- maven-resources-plugin:3.1.0:testResources (default-testResources) @ java-unit-testing-demo ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /path/to/your/project/src/test/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ java-unit-testing-demo ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /path/to/your/project/target/test-classes
[INFO]
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ java-unit-testing-demo ---
[INFO]
[INFO] -------------------------------------------------------
[INFO] T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.example.CalculatorTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.021 s - in com.example.CalculatorTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 3.123 s
[INFO] Finished at: 2025-01-23T17:52:51Z
[INFO] ------------------------------------------------------------------------
```
This indicates that the tests were successfully executed and no tests failed.

## Conclusion

This project demonstrates the basics of setting up and running unit tests in a Java project using JUnit and Maven. Feel free to explore and extend the functionality of the `Calculator` class and add more tests to further validate its behavior.
