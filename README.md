# Rental Management App

## Overview
The Rental Management System is a Java-based application built with Maven for cross-platform compatibility. It employs Doxygen for documentation and unit testing, providing a console-based interface navigable via keyboard inputs.

---

## System Architecture

The system utilizes the standard Java file input/output library with custom file operation functions:

- **file_read()**: Reads data from a file.
- **file_write()**: Deletes all data and writes new data to a file.
- **file_edit()**: Edits a specified record line.
- **file_line_delete()**: Deletes a specified record line.
- **file_append()**: Appends a record at the end of the file.

---

## Functionalities
The application supports the following features:

### Tenant Management
- TenantID
- PropertyID
- Rent
- Birthdate
- Name
- Surname

### Property Management
- PropertyID
- PropertyAge
- Bedrooms
- Living Rooms
- Floors
- Size
- Address

### Maintenance Management
- PropertyID
- Cost
- Priority
- Maintenance Type
- Expected Finishing Date

### Rent Management
- TenantID
- Current Rent Debt
- Due Date

---

## Testing and Validation
The system has been tested and documented using JUnit 4, achieving:

- **95% Test Coverage**
- **100% Success Rate in Unit Tests**

---

## Releases

- [![GitHub release badge](https://badgen.net/github/release/ucoruh/eclipse-java-maven-template)](https://github.com/ucoruh/eclipse-java-maven-template/releases/latest)

## Platforms

- ![Ubuntu badge](assets/badge-ubuntu.svg)
- ![macOS badge](assets/badge-macos.svg)
- ![Windows badge](assets/badge-windows.svg)

## Test Coverage

[![Release](https://github.com/ucoruh/eclipse-java-maven-template/actions/workflows/release.yml/badge.svg)](https://github.com/ucoruh/eclipse-java-maven-template/actions/workflows/release.yml)

**Coverage:**

- ![All](assets/badge_combined.svg)

**Branch Coverage:**

- ![Branch Coverage](assets/badge_branchcoverage.svg)

**Line Coverage:**

- ![Line Coverage](assets/badge_linecoverage.svg)

**Method Coverage:**

- ![Method Coverage](assets/badge_methodcoverage.svg)

---

## Install Requirements

### Required Tools

1. **Eclipse**  
   [Eclipse Downloads | The Eclipse Foundation](https://www.eclipse.org/downloads/)

2. **Maven**  
   [Maven – Download Apache Maven](https://maven.apache.org/download.cgi)

3. **JDK**  
   [Download JDK](https://www.eclipse.org/downloads/)

4. **LCOV**  
   [Installation Instructions](https://fredgrott.medium.com/lcov-on-windows-7c58dda07080)

5. **Coverxygen**  
   [coverxygen · PyPI](https://pypi.org/project/coverxygen/)
   [GitHub - psycofdj/coverxygen](https://github.com/psycofdj/coverxygen)

6. **ReportGenerator**  
   [ReportGenerator Official Website](https://reportgenerator.io/)
   ```bash
   dotnet tool install -g dotnet-reportgenerator-globaltool
   ```
