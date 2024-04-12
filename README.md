# [JSL08] Submission: Singleton Pattern for Bank Branch Management

Overview: https://www.youtube.com/watch?v=sJ-c3BA-Ypo

Practice challenges on Scrimba here: https://scrimba.com/playlist/pKJewwyu4

Design patterns like Singleton, Factory, and Observer can significantly improve the structure and maintainability of your JavaScript projects, making your code cleaner and more efficient. By understanding and applying these patterns, you'll be well-equipped to tackle complex design challenges in your projects, just as a well-organized bank efficiently manages its operations and services.

## Overview:
A Singleton pattern ensures that a class has only one instance and provides a global point of access to it. For our banking system, we used the Singleton pattern to manage the bank's branch information. The core class `BankBranch` encapsulates branch information and provides methods for managing and accessing it.

## Reflections & Code choices:
Implementing a singleton pattern ensures that only one instance exists throughout the application lifecycle. This design choice simplifies managements and prevents duplication of data. By utilizing a class-based approach, the code maintains a clear structure and facilitates code organization.

- **Singleton Instance:** A variable named `bankBranchInstance` is used to store the singleton instance of the bank branch. This variable ensures that only one instance exists at any given time.
- **BankBranch Class:** The `BankBranch` class is responsible for managing branch information. It includes a `constructor` to initialize branch data and methods for accessing and manipulating branch details.
- **Constructor:** The `constructor` of the `BankBranch` class takes `branchInfo` as a parameter. It checks if the `bankBranchInstance` variable is null, indicating whether an instance exists or not. If no instance exists, a new instance is created with the provided branch information, and the bankBranchInstance variable is assigned to it.
- **Methods:** The BankBranch class includes methods such as `getBranchInfo` to retrieve branch details. These methods facilitate interactions with branch data and ensure encapsulation of branch-specific functionalities.
- **Usage:** In the usage section, instances of the `BankBranch` class (branchA and branchB) are created with different branch information. The `getBranchInfo` method is then used to retrieve branch details from these instances.



