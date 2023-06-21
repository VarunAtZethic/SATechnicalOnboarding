# Coding standards

### Zethic’s Coding Standards apply to code within the project and its contributed modules.

Maintaining consistent coding standards is crucial for ensuring readability, maintainability, and collaboration within a project. Documenting coding standards provides guidelines for developers to follow and promotes a cohesive codebase. Here are some key points to consider when documenting coding standards within your project:

# **_Formatting and Style:_**

Specify the formatting and style conventions that developers should adhere to. This includes guidelines for indentation, line length, spacing, and naming conventions. Some common elements to consider include:

1. <u>Indentation:</u> Define the number of spaces or tabs to use for indentation.
2. <u>Line Length:</u> Specify the maximum allowed length for a line of code.
3. <u>Spacing:</u> Define guidelines for spacing around operators, parentheses, and commas.
4. <u>Naming Conventions:</u> Specify conventions for naming variables, functions, classes, and other code elements.

# **_Comments and Documentation:_**

Establish guidelines for comments and documentation within the codebase. This helps ensure code clarity and provides valuable insights for future maintenance. Include the following considerations:

1. <u>Comment Style:</u> Define the preferred style for comments, such as single-line comments (//) or block comments (/* */).
2. <u>Comment Placement:</u> Specify where comments should be placed, such as at the beginning of a function or preceding complex code sections.
3. <u>Documentation Standards:</u> Encourage the use of documentation tools like Javadoc or Doxygen for generating API documentation.
4. <u>Documentation Content:</u> Provide guidance on documenting code purpose, input/output descriptions, and any relevant examples or caveats.

# **_Error Handling and Exceptions:_**

Define how error handling and exceptions should be implemented within the codebase. This ensures consistent and reliable error handling practices. Consider the following:

1. <u>Exception Types:</u> Specify which exception types to use for specific error scenarios.
2. <u>Error Messages:</u> Define guidelines for error message formatting, including language localization if applicable.
3. <u>Exception Handling:</u> Establish best practices for exception handling, such as when to catch exceptions, when to propagate them, and when to handle recoverable errors.

# **_Code Organization and Structure:_**

Document guidelines for organizing and structuring code within the project. This promotes maintainability and helps developers quickly understand the codebase. Include considerations such as:

1. <u>File Organization:</u> Specify rules for organizing files within the project directory structure.
2. <u>Class and Function Organization:</u> Define guidelines for organizing classes, methods, and functions within files.
3. <u>Modularity and Encapsulation:</u> Encourage modular code design and the use of appropriate access modifiers.
4. <u>Code Duplication:</u> Address code duplication concerns and emphasize the importance of reusability and refactoring.

# **_Testing Standards:_**

Provide guidelines for writing tests within the project. This ensures consistent and effective testing practices. Consider the following aspects:

1. <u>Test Naming Conventions:</u> Specify conventions for naming test methods and classes.
2. <u>Test Structure:</u> Define the structure of test classes, including setup and teardown methods.
3. <u>Test Coverage:</u> Encourage developers to aim for high test coverage to ensure comprehensive testing.
4. <u>Assertions and Expectations:</u> Define guidelines for using assertions and expectations effectively.

# **_Version Control Practices:_**

Include guidelines for version control practices to promote collaboration and ensure a clean commit history. Consider the following:

1. <u>Branching Strategy:</u> Define the preferred branching strategy for feature development, bug fixes, and releases.
- feature/* : if you are working on a new feature
- fix/* : If you are working on a complex fix
- hotfix/* : If you are working on a small fix
- minor/* : Any small task or minor changes
- name of the branch

Example:

- Feature name -> add email field in the contact form
- Branch name -> feature/add-email-in-contact-form
- Feature name -> reports page crash
- Branch name -> fix/reports-page-crash
Ref: [Medium](https://medium.com/p/8fd00f66e394)

2. <u>Commit Guidelines:</u> Specify rules for writing clear and descriptive commit messages.
3. <u>Code Review Process:</u> Outline the process for conducting code reviews and providing constructive feedback.

# **_Continuous Integration and Deployment_**

If your project incorporates continuous integration and deployment, provide guidelines for setting up and configuring the CI/CD pipeline. Specify the required configuration files, testing procedures, and deployment guidelines.

By documenting coding standards within your project, you provide developers with clear guidelines to follow, leading to consistent and maintainable code. It also facilitates collaboration among team members and reduces the time spent on code reviews and refactoring. Regularly review and update the documentation to reflect any changes.