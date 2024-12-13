# Rental Management Console Application

This is a console-based application for managing rental properties, tenants, maintenance tasks, and rent payments. The project is structured to use Java (with Maven), ensuring cross-platform compatibility and robust functionality.

---

## Functionalities

### Menu Options
- **View, Register, Update, or Delete Records**: Manage tenants, properties, maintenance tasks, and rent records.
- **Search and Sort**: Features for easy navigation and organization.

### Data Categories

#### 1. Tenant Management:
- TenantID
- PropertyID
- Rent
- Birthdate
- Name
- Surname

#### 2. Property Management:
- PropertyID
- PropertyAge
- Bedrooms
- Living Rooms
- Floors
- Size
- Address

#### 3. Maintenance Management:
- PropertyID
- Cost
- Priority
- Maintenance Type
- Expected Finishing Date

#### 4. Rent Management:
- TenantID
- Current Rent Debt
- Due Date

---

## Platforms

- ![Ubuntu badge](assets/badge-ubuntu.svg)
- ![macOS badge](assets/badge-macos.svg)
- ![Windows badge](assets/badge-windows.svg)

---

## Testing and Validation

- **Unit Testing**: Comprehensive testing using gtest and CTest, achieving 95% test coverage and 100% success rate.
- **Validation**: Ensures all functionalities operate correctly under different scenarios and data sizes.

---

## Installation and Setup

### Prerequisites
1. **CMake**: For building the C modules.
2. **Maven**: For managing Java dependencies and builds.
3. **JDK**: Java Development Kit.
4. **LCOV**: For code coverage reports.
5. **Coverxygen**: For parsing Doxygen documentation.

### Clone the Repository
```bash
git clone https://github.com/username/rental-management-app.git
cd rental-management-app
```

### Build the Project
#### For C Modules:
```bash
cmake .
make
```
#### For Java Modules:
```bash
mvn clean install
```

### Run the Application
#### For C Modules:
```bash
./rental_management_app
```
#### For Java Modules:
```bash
java -jar target/rental-management-app-1.0.jar
```

---

## Test Coverage and Reports

### Code Coverage
- **LCOV**: Use to generate coverage reports for C modules.
- **JaCoCo**: Integrated for Java modules with Maven.

### Generate Reports
- **HTML Coverage Reports**:
```bash
reportgenerator "-reports:target/site/jacoco/jacoco.xml" "-sourcedirs:src/main/java" "-targetdir:coveragereport" -reporttypes:Html
```

- **Documentation Coverage**:
```bash
python -m coverxygen --xml-dir ./docs/xml --src-dir ./src --format lcov --output ./coverage.info
```

---

## Documentation and Code Formatting

### Doxygen Setup
1. Install Doxygen and Graphviz.
2. Generate the default configuration file:
   ```bash
   doxygen -g
   ```
3. Update the `Doxyfile` to output documentation in the `./docs` directory.

### Code Formatting with AStyle
1. Install AStyle:
   ```bash
   choco install astyle
   ```
2. Format code:
   ```bash
   astyle --options=astyle-options.txt --recursive *.c *.h *.java
   ```

---

## License
This project is licensed under the [MIT License](LICENSE).

For any issues or feature requests, please open a ticket on the [GitHub Repository](https://github.com/username/rental-management-app/issues).

