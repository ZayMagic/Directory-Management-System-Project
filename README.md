# Directory Management System

## Overview

The Directory Management System is a C++ project that implements dynamic arrays and copy control mechanisms to manage a directory of personnel within a company. This project focuses on memory management, resource allocation, and object-oriented programming concepts such as composition, encapsulation, and operator overloading.

## Features

- **Dynamic Arrays**: Utilizes dynamic memory allocation to manage arrays of personnel entries.
- **Copy Control Mechanisms**: Implements copy constructor and assignment operator to enable seamless copying of Directory objects.
- **Nested Classes**: Defines nested Position and Entry classes to encapsulate data and functionality.
- **Operator Overloading**: Overloads operators such as << (output operator) for convenient printing of Directory objects.
- **Flexible and Extensible**: Designed to be flexible and extensible, allowing for easy integration into larger systems or future enhancements.

## Usage

To use the Directory Management System in your project:

1. Include the necessary header files in your C++ source files.
2. Create a Directory object by providing the company name.
3. Add personnel entries using the `add()` method, providing name, room number, phone number, and position details.
4. Access personnel information using the [] operator, providing the name of the personnel.

Example usage:

```cpp
// Create a Directory object
Directory d("CompanyXYZ");

// Add personnel entries
Position boss("CEO", 100000.00);
d.add("John Doe", 101, 1234567890, boss);

// Access personnel information
unsigned phoneNumber = d["John Doe"];



