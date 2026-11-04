# SimpleCalculator Maven Project

A simple Java calculator demonstrating Maven build automation and JUnit 5 unit testing.

## Requirements
- JDK 17 or later
- Apache Maven 3.6 or later

## Project structure
```text
SimpleCalculator/
├── pom.xml
└── src/
    ├── main/java/com/calculator/Calculator.java
    └── test/java/com/calculator/CalculatorTest.java
```

## Run from the project root

Compile:
```bash
mvn clean compile
```

Run JUnit tests:
```bash
mvn test
```

Package:
```bash
mvn package
```

Run the calculator after packaging:
```bash
java -cp target/SimpleCalculator-1.0-SNAPSHOT.jar com.calculator.Calculator
```

The test suite contains five tests: addition, subtraction, multiplication, division, and division by zero.

## Import into Eclipse
1. Extract the ZIP file.
2. Open Eclipse.
3. Select **File → Import → Maven → Existing Maven Projects**.
4. Browse to the extracted `SimpleCalculator` folder.
5. Select the `pom.xml` and click **Finish**.
