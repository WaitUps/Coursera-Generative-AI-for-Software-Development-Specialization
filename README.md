# **Generative AI for Software Development: Prompt Reference & Guidelines**

This repository serves as a reference for the **[Generative AI for Software Development Skill Certificate](https://www.coursera.org/professional-certificates/generative-ai-for-software-development)**. It is designed to act as a structured prompting framework for AI-augmented project lifecycles, ensuring that system design, security, and documentation follow consistent, expert-level principles.

---

## **Specialization**

**Generative AI for Software Development Skill Certificate**
* **Course 1:** Introduction to Generative AI for Software Development
* **Course 2:** Team Software Engineering with AI
* **Course 3:** AI-Powered Software and System Design

---

## **Credits & License**

This project was developed as part of the **Generative AI for Software Development** Specialization on Coursera.

* **Prompt Methodology:** Provided by DeepLearning.AI/Coursera & Google Gemini.

*This repository is for educational purposes and adheres to the licensing terms provided in the original course materials.*

---

## **Development Workflow & Guidelines**

This section serves as a **structured prompting guide for every new project**. To maintain consistency across projects, follow this logical flow for every development cycle:

### **1. Environment & Dependency Foundation**
*(Course 2: Module 3)*
Before a single line of code is written, establish a clean, isolated workspace:
* **Isolation**: Utilize expert prompts to configure **Virtual Environments** (`venv`, `pip-tools`) specifically for your operating system.
* **Dependency Selection**: Audit potential libraries for community trust and maintenance history before installation.
* **Containerization**: Draft **Multi-stage Dockerfiles** to ensure the development environment matches production.

### **2. System Architecture & Data Design**
*(Course 3: Modules 1 & 2)*
Establish the "blueprint" using **AI-Powered System Design** principles:
* **Serialization Strategy**: Implement **Configuration-Driven Development (CDD)** and JSON/Pickle serialization to allow for non-technical customization.
* **Relational Modeling**: Design robust **Database Schemas** and implement CRUD operations using SQLAlchemy to ensure data integrity.

### **3. Design Patterns & Maintainability**
*(Course 3: Module 3)*
Refine the structure using industry-standard paradigms:
* **Gang of Four Patterns**: Apply **Factory**, **Singleton**, or **Template Method** patterns to make code more modular and easier to maintain.
* **Refactoring**: Identify **"Code Smells"** and consolidate redundant logic using DRY (Don't Repeat Yourself) principles.

### **4. Technical Documentation**
*(Course 2: Module 2)*
Document the intent and usage as you build to prevent technical debt:
* **Multi-Audience Docs**: Generate docstrings tailored for everyone from **Junior Developers** to **External API Consumers**.
* **Standardized Styles**: Ensure all documentation follows professional guides like **Google**, **NumPy**, or **reST**.
* **Automated Tooling**: Set up **Sphinx** or **MkDocs** to convert source code comments into professional static sites.

### **5. Security, Quality & Multi-Layer Testing**
*(Course 2: Module 1)*
Validate and protect the application through every stage:
* **Security Integration**: Proactively scan for **OWASP Top 10** vulnerabilities like SQL injection and XSS during the drafting phase.
* **Performance Auditing**: Use **Big O Analysis** and **CProfile** prompts to identify bottlenecks and memory leaks.
* **Resilience Testing**: Apply **Chaos Engineering** and **Exploratory Testing** to find edge cases before they reach production.
* **Automated Suites**: Convert manual findings into permanent **PyTest** or **Selenium** suites for continuous integration.

---


### **Curriculum Outline**

---

#### **Course 2: Team Software Engineering with AI**

* **Module 1: Testing and Debugging**
    * **Testing and Debugging Strategies**: Analytical and logical validation.
    * **Exploratory Testing**: Edge case discovery and stress testing.
    * **Memory & Mutability Analysis**: Technical evaluation of Python memory models.
    * **Functional Testing**: Verification of business requirements and flows.
    * **Automated Testing**: Scripts for PyTest, Selenium, and API mocking.
    * **Software Performance Testing**: Benchmarking, Big O analysis, and optimization.
    * **Security and Quality Assurance**: Vulnerability scanning (OWASP) and code smells.
    * **Integration and API Testing**: Multi-service contract and error handling verification.

* **Module 2: Documentation**
    * **Inline Comments**: Context-driven architectural explanations.
    * **Prompts for Different Audiences**: Audience-specific docstrings (Junior to Executive).
    * **Prompts for Specific Docstring Styles**: Formal styling (Google, NumPy, reST, JSDoc).
    * **Alternative Documentation Types**: Visualizations (Mermaid) and technical specs.
    * **Maintenance and Structural Analysis**: Deprecation notices and refactoring.
    * **Automated Documentation Tools**: Setup and CI/CD for Sphinx, MkDocs, and Doxygen.
    * **API Specification & Tooling**: OpenAPI/Swagger and Postman generation.
    * **Documentation Quality & Linting**: Terminology consistency and readability audits.

* **Module 3: Dependency Management**
    * **Virtual Environments**: Setup, shell automation, and environment cleanup.
    * **Researching and Selecting Dependencies**: Library auditing and tool comparison.
    * **Dependency Conflicts and Resolution**: Hierarchy visualization and version pinning.
    * **Security and Vulnerability Scanning**: Automated auditing and safety workflows.
    * **Dependency Management in Other Languages**: Cross-ecosystem comparisons (Go, Rust).
    * **Docker and Containerized Dependencies**: Multi-stage builds and volume mounting.

---

#### **Course 3: AI-Powered Software and System Design**

* **Module 1: Data Serialization and Configuration-Driven Development (CDD)**
    * **Design Paradigms**: High-level CDD and customization strategies.
    * **Serialization Tools**: Practical implementation of JSON and Pickle.
    * **Externalizing Parameters**: Separation of logic from API payloads and configuration.

* **Module 2: Databases**
    * **Schema Design**: Relational modeling for Social Networks and E-commerce.
    * **CRUD Operations**: Functional implementation via SQLAlchemy.
    * **Advanced Querying**: Complex joins and data aggregation.
    * **Database Optimization**: Indexing, caching, and performance logging.

* **Module 3: Software Design Patterns**
    * **Gang of Four Overview**: Conceptual framework for structural patterns.
    * **Patterns Advice**: Iterative refactoring for real-world applications.
    * **Factory Patterns**: Implementation of polymorphic object creation.
    * **Template Method Pattern**: Standardizing algorithmic structures.


---

## **Complete Prompt Reference Library**


### **Team Software Engineering with AI Course**

#### **Module 1: Testing and Debugging**

**Testing and Debugging Strategies**

```
"As an expert software tester who's teaching a new person how to write test cases, can you please analyze this code and provide a set of test cases explaining each one?"

"Analyze this code and generate a 'Dry Run' table that tracks variable states through each iteration of the loop to identify where the logic fails."

"Create a checklist of common failure points for this specific type of algorithm (e.g., recursion depth, off-by-one errors) and check this code against them."
```

**Exploratory Testing**

```
"You are a software engineer and tester who is curious and who likes to go through code looking for edge cases. There's some Python code here -- please explore it and find any issues that might cause bugs or poor functionality."

"Act as a 'Chaos Engineer.' What happens to this code if the input data is malformed, extremely large, or contains unexpected characters like emojis or null bytes?"

"Identify any 'hidden' assumptions in this code—logic that assumes a network is always up or that a database query will never return an empty set."
```

**Memory & Mutability Analysis (New Category)**

```
"Analyze this code for 'Mutable Default Argument' bugs. Does any function use a list or dictionary as a default parameter value? Explain why this is dangerous in Python's memory model."

"Check this code for 'Side Effects.' Are there functions that modify a list or dictionary passed as an argument? Suggest how to refactor these to return new objects instead of mutating the originals."

"Identify areas where 'Shallow Copies' are being used (e.g., list.copy() or [:]). Evaluate if a 'Deep Copy' is required to prevent unintended data corruption in nested structures."

"Look for instances of unnecessary string concatenation in loops. Explain the memory penalty incurred by string immutability in this context and refactor using "".join()."
```

**Functional Testing**

```
"I’m working on a simple todo list app. Here is the code. In exploratory testing, the tester came with these lines of code: [Insert Code]. As an expert software tester, write code that converts the output of the exploratory testing into functional tests using the unittest module in python."

"Given these business requirements [Insert Requirements], write a suite of functional tests that verify the application behaves correctly from the perspective of a user performing a 'Happy Path' flow."

"Generate a traceability matrix that maps these functional tests back to the specific project requirements provided."
```

**Automated Testing**

```
"You are an expert in PyTest for automated testing of python code. Please amend this code with a comprehensive set of tests in Pytest to find bugs or other issues in the code."

"Can you suggest automated testing libraries for this Python code, please?"

"Rewrite these manual test steps into a Python script using Selenium or Playwright for end-to-end browser automation."

"Show me how to use pytest.mark.parametrize to run this single test function against 10 different input datasets."

"Create a Mocking strategy for this function so I can test the logic without actually making calls to the external Stripe API."
```

**Software Performance Testing**

```
"How would I measure how long it takes to call this function in Python?"

"Rewrite the function in the code below to be more optimized. Below the code is the output from a CProfile analysis of the function."

"Analyze the Big O time complexity of this function and suggest a more efficient data structure (e.g., switching from a List to a Set) to improve lookup times."

"Write a Python script using timeit to benchmark these two different versions of the function and tell me which one is faster under heavy load."

"Identify any memory leaks or high-memory usage patterns in this code and suggest ways to reduce the heap footprint."

"Analyze the 'Object Lifecycle' in this script. Are there large objects being held in memory (Heap) longer than necessary, preventing the Garbage Collector from freeing them?"
```

#### **Security and Quality Assurance**

**Analyzing Code for Security Vulnerabilities**

```
"You are an expert in web security and in creating API endpoints. With the following code, there are likely many vulnerabilities. Can you create some test cases that test against these vulnerabilities?"

"Review this code for OWASP Top 10 vulnerabilities, specifically looking for SQL injection, Cross-Site Scripting (XSS), and insecure direct object references (IDOR)."

"Act as a penetration tester. How would you attempt to bypass the authentication logic in this specific function?"

"Explain how to sanitize the inputs in this function to prevent command injection attacks."
```

**Code Refactoring and Maintainability**

```
"Analyze this code for 'Code Smells' like long methods, duplicate logic, or overly complex conditionals. Suggest a refactored version that is easier to read."

"Break this large, monolithic function into smaller, modular functions that follow the Single Responsibility Principle."

"Apply the DRY (Don't Repeat Yourself) principle to this module and consolidate the redundant logic into a reusable utility class."

"Refactor this code to use 'Immutable Data Structures' (like Tuples instead of Lists) where data should not change, to improve thread safety and predictability."
```

**Integration and API Testing**

```
"This function relies on three different microservices. Generate a set of integration tests that verify the data contract between these services is maintained."

"Generate a Postman collection JSON or a series of curl commands to test all the CRUD operations for the following API endpoint."

"Write a test that simulates a '504 Gateway Timeout' from a dependent service to see if our error-handling logic fails gracefully."
```

#### **Module 2: Documentation**

**Inline Comments**

```
"Write a function [Insert Task] intended for an experienced Python developer. Use minimal, high-level comments that focus on architectural decisions rather than syntax."

"Update the code to make it easier to follow for a novice developer. Add detailed inline comments that explain the purpose of each variable and the logic behind each conditional statement."

"Critique the comments I've included in this code and offer suggestions for improvement. Identify which comments are redundant (stating the obvious) and which areas need more explanation."

"Review these inline comments and ensure they explain the intent of the code. Replace 'increments i by 1' style comments with context-driven explanations like 'move to the next record in the batch.'"

"Add 'TODO' and 'FIXME' comments to this code. Identify technical debt or areas that require future optimization based on these requirements: [Insert Requirements]."
```

**Documentation Comments**
**Prompts for Different Audiences**

```
"For Junior Developers: Write a docstring for this function that explains the logic step-by-step. Avoid overly technical jargon and use analogies where helpful to explain the data transformation."

"For Senior/Peer Reviewers: Generate documentation for this function focusing on edge cases, time complexity, and potential side effects. Assume the reader is familiar with the codebase architecture."

"For Non-Technical Product Managers: Summarize what this function does in plain English. Focus on the business value—what user problem does this solve, and what is the final output?"

"For Future Self (Quick Reference): Create a concise, high-level summary of this function. I just need to know the 'what' and 'how to call it' without digging into the implementation details."

"For External API Consumers: Write a formal documentation block for this public method. Include clear descriptions for all parameters, expected return types, and a list of possible exceptions it might throw."
```

**Prompts for Specific Docstring Styles**

```
"Google Style: Refactor the existing documentation for this function to follow the Google Python Style Guide. Ensure the 'Args', 'Returns', and 'Raises' sections are formatted correctly."

"NumPy/SciPy Style: Rewrite this docstring using the NumPy style. Focus heavily on the 'Parameters' and 'Attributes' sections with their respective types and descriptions."

"reStructuredText (reST): Convert this function's comments into reST (Sphinx) format. Use the :param: and :returns: directives so it can be parsed into HTML documentation."

"JSDoc Style: Generate a JSDoc comment for this JavaScript function. Include @typedef if there are complex objects involved and specify @example usage."

"Javadoc Style: Provide a Javadoc compliant comment for this method. Use @link tags to reference related classes and ensure the @see section points to the relevant module."
```

**Alternative Documentation Types**

```
"The 'Usage Example' Focus: Instead of explaining the logic, provide three different code examples of how to implement this function in a real-world scenario."

"The Mermaid Flowchart: Based on the logic in this function, generate a Mermaid.js syntax flowchart to visualize the conditional paths and loops."

"README Technical Spec: Draft a section for a README.md file based on this function. Include a 'Features' list, a 'Quick Start' snippet, and a table of configuration options."

"The 'Why' Documentation (Decision Log): Document this function focusing on the design decisions. Explain why this specific algorithm was chosen over simpler alternatives and note any constraints we faced."

"Unit Test Documentation: Write documentation for the test suite of this function. Explain what each test case is verifying (e.g., 'Verifies null handling', 'Verifies high-load performance') so a tester understands the coverage."
```

**Maintenance and Structural Analysis**

```
"Deprecation Notice: Analyze this legacy function and generate a Deprecation Notice. Explain why it is being phased out, what the new alternative is, and provide a timeline for removal."

"Change Log Entry: Create a Change Log entry for this function update. Highlight changes to input parameters to warn other developers of potential breaking changes."

"Self-Documenting Code: Suggest more descriptive names for the variables and functions in this snippet to make the code 'self-documenting' and reduce the need for extensive comments."

"Complexity Critique: Identify areas where the code is too 'clever' or obfuscated. Rewrite it for maximum readability so a developer can understand it at a glance without needing a docstring."
```

**Automated Documentation Tools**

```
"As an expert in generating automatic documentation, can you help me set up Sphinx to generate documentation for the following python code?"

"Create a configuration file (conf.py) and a standard index.rst structure for a Sphinx project that needs to include the autodoc and viewcode extensions."

"Walk me through the steps to set up MkDocs with the mkdocstrings handler for this repository. Provide the mkdocs.yml configuration required to render my Python source code as beautiful static pages."

"Generate a Doxygen configuration file (Doxyfile) optimized for a C++/Python hybrid project. Ensure it is set to extract all functions, including private members, and generate a dependency graph."

"How can I integrate documentation generation into a GitHub Actions workflow? Provide a YAML snippet that builds my documentation on every push to the main branch and deploys it to GitHub Pages."

"Compare Sphinx vs. MkDocs for a fast-growing Python API project. Which one offers better support for versioned documentation and searchable indexes?"
```

**API Specification & Tooling**

```
"Convert this Python FastAPI/Flask code into a comprehensive OpenAPI 3.0 (Swagger) specification in YAML format. Include all request parameters, response schemas, and authentication headers."

"Write a Postman Collection (JSON) for the following API endpoints. Include pre-request scripts that handle JWT token authentication for each call."

"Generate a ProtoBuf (Protocol Buffers) definition file based on these Python class structures to facilitate high-performance microservice communication."
```

**Documentation Quality & Linting**

```
"Act as a documentation linter. Scan this code and identify any functions that are missing docstrings or have parameters that don't match the current implementation."

"Evaluate the 'Readability Score' of this README file. Suggest improvements to the structure to make it more scannable for developers who are in a hurry."

"Check this documentation for consistency in terminology. Ensure that we aren't using multiple different terms (e.g., 'user', 'client', 'account') to describe the same entity."
```

#### **Module 3: Dependency Management**

**Virtual Environments**

```
"You're an expert in Python virtual environment setup. What steps can I follow to set up a virtual environment on my Mac using venv?"

"You're an expert in python programming and dependency management. Please guide me on how to install pip-tools and compile my first set of dependencies."

"Show me how to configure my shell (Zsh/Bash) to automatically activate a virtual environment when I cd into this project directory."

"I accidentally installed packages globally instead of in my virtual environment. How can I identify which packages are global and clean them up without breaking my system Python?"

"Explain the difference between bin/python inside a virtual environment and the system /usr/bin/python3. How does the PATH variable change when I run source bin/activate?"
```

**Researching and Selecting Dependencies**

```
"I am working on a simple web application in Python. Below are the dependencies currently listed for that project. For each one write me a short summary of what it does and whether I should trust it."

"Act as a Senior Python Software Engineer specializing in DevOps and project architecture. I am starting a new project and need a comprehensive guide on the best practices for managing dependencies and virtual environments. Please compare several options—such as Poetry, UV, and pip-tools with venv—and provide a recommendation based on project scale, performance, and ease of use in a CI/CD pipeline."

"Analyze this library's GitHub repository [Insert Link]. Based on its recent commit activity, issue count, and maintenance history, would you recommend using it for a production-grade enterprise application?"

"I need a library for [Task, e.g., Image Processing]. Compare the top three Python libraries for this, focusing on performance, community support, and licensing (e.g., MIT vs. GPL)."
```

**Dependency Conflicts and Resolution**

```
"I am working on a simple web application in Python. Below are the dependencies currently listed for that project. Are there any known dependency conflicts between the versions of the libraries I am using?"

"I am getting a VersionConflict error when trying to install [Library A] and [Library B]. Can you analyze their dependency trees and suggest a specific version for both that satisfies all constraints?"

"Explain how to use pip deptree to visualize my current environment's hierarchy and identify which nested dependency is forcing an outdated version of a core library."

"Help me write a 'Constraints File' to force specific versions of sub-dependencies across my entire development team without explicitly adding them to my main requirements.txt."
```

**Security and Vulnerability Scanning**

```
"How can I check that the packages in my current Python environment are secure?"

"I’m working on a simple web application in Python. Below are the dependencies currently listed for that project. Are there any known security issues for these libraries?"

"Show me how to integrate Safety or pip-audit into a GitHub Actions workflow to automatically block pull requests that introduce vulnerable packages."

"Explain the risks of 'Dependency Confusion' attacks and how I can configure my package manager to prioritize our private internal PyPI server over the public one."
```

**Dependency Management in Other Languages**

```
"How can I check the following package.json file for known dependency issues?"

"I am moving from Python to Go. Compare how Go handles dependencies via go mod versus how Python handles them with pip and virtual environments."

"Analyze this Gemfile (Ruby) or Cargo.toml (Rust) and explain the equivalent 'lockfile' concept in those ecosystems. How do they handle reproducible builds compared to Python's requirements.txt?"
```

**Docker and Containerized Dependencies**

```
"Write a multi-stage Dockerfile for this Python project that ensures the build-time dependencies (like compilers) are not included in the final production image to keep the size small."

"How should I handle virtual environments inside a Docker container? Is it better to create one inside the container or just install packages to the system level since the container is already isolated?"

"Create a docker-compose.yaml file that mounts my local code as a volume but keeps the site-packages inside the container's filesystem to avoid OS-mismatch errors between my Mac and the Linux container."
```

---

### **AI-Powered Software and System Design Course**

#### **Module 1: Data Serialization and Configuration-Driven Development**

```
"You are an expert on software design paradigms. I am working on building a simple Python-based app that will make calls to the DALL-E API and generate images for users. The application will be deployed in many different contexts and configurations depending on the end users, and I want my less technical colleagues to be able to do some customization without editing the code itself. What high level software design paradigms should I consider for this project?"

"Help me weigh the pros and cons of using Configuration-Driven Development (CDD) on this project?"

"Which file formats should I consider for using in my configuration files. For each one share the pros and cons of using it."

"How do I write data to a file in Python?  I'm an experienced developer, so just give me the sample code."

"If I'm going to be reading and writing configuration files in JSON,  which commands should I be familiar with, and can you show me some examples?"

"You are an expert Python develop who intimately understands the language and its ecosystem. You are also an excellent explainer that helps people understand whatever you tell them, whether they are a novice or expert. Please answer this question: Explain what Pickle is, and why it is useful in Python. Be very succinct."

"What are the most useful commands for me to know in Pickle? Show me an example of pickling a more complex object."

Code to call DALL-E: "You are a deep expert on the OpenAl ecosystem, including the client libraries, REST endpoints, and any other way of accessing functionality of GPT, DALL-E, and other models. Please create easy to read, easy to follow code that will call DALL-E to generate an image. The code should be in Python, and all parameters should be in an external file that the Python code reads. Please use the most up-to-date design pattern."

"You are a deep expert on the Google Gemini ecosystem, including the google-genai client libraries, REST endpoints, and all methods of accessing functionality for the Gemini 3 Flash and Veo models. Please create easy-to-read, easy-to-follow code that will call the Gemini image generation model (Nano Banana 2) to generate an image. The code should be in Python, and all parameters should be in an external file that the Python code reads. Please use the most up-to-date design pattern."

"Can you create code that accesses the OpenAI endpoint at: [https://platform.openai.com/docs/api-reference/images/create](https://platform.openai.com/docs/api-reference/images/create) directly to create an image?"

"Can you create code that accesses the Gemini endpoint via the google-genai REST interface directly to create an image?"

Externalizing parameters: "I have this code that calls the REST endpoint for DALL-E to generate an image. The code has the parameter for the calls hardcoded in it. Can you externalize the parameters in a separate file? Please also provide an exhaustive list of the parameters in the API docs here: [https://platform.openai.com/docs/api-reference/images/create](https://platform.openai.com/docs/api-reference/images/create)"

Externalizing parameters: "Can you modify this code to fix two issues: First, regardless of how many images we ask for, you only parse out 1 image from the response data. Second, can you download the images from the URL and save them locally. Add the desired filename to the JSON file, and save them as < filename>1.PNG, ‹filename> 2.PNG etc."

Adding parameters and serializing results: "Can you make 2 more modifications: First can you add the style and quality parameters to the payload configuration, and load them to pass to the backend?Then, after the files are downloaded, can you pickle them up along with the configuration file?"
```

#### **Module 2: Databases**

**Design and implement a database schema**

```
Design database schema: "I need to develop a database for a social network. The database will track individual people, and store information about them including their name, age, hometown, and hobbies. The database will also store relationships between people, including family relationships, friendships, work colleagues, and schoolmates. Suggest a schema that would work for this."

Creating the e-commerce schema: "Design a database schema for an e-commerce application with tables for users, products, orders, and order_items."

Design database schema: "I have a sqlite database set up in Python using SQLAlchemy. Help me implement tables for the following schema: … "
```

**Implementing CRUD operations**

```
The create operation: "What are the things to consider when you implement the create operation for a database?"

The create operation: "How to create a function to add a new user to the users table of this database?"

Implementing read functionality: "Generate code that implements a read function for this database. It should return a list of all users currently in the database: "

Update operation: "Generate  code that implements an update function for this database. I want to use it to update the email address of a user."

Checking for vulnerabilities: "I'm using this code in a SQL database. Is there a chance that it's vulnerable to SQL injection attack as SQLAlchemy appears to use SQL under-the-hood?"
```

**Advanced querying**

```
Write SQL queries: "Write a SQLAlchemy query to find all orders placed by a specific user in the e-commerce database."
More complex SQL queries: "Write a SQLAlchemy query to find the total quantity of each product sold in this database."
```

**Databaset optimization**

```
General: "What are some of the best practices to improve the performance of this database?"
Follow up: "What are the best practices for indexing a SQL database?"
Caching: "How can I implement basic query caching in SQLALchemy?"
Best Data Types: "What are the best practices for choosing data types in a SQL database?"
Debug Database Errors: "How do I handle database connection errors in SQLAlchemy?"
Handling edge cases: "How do I handle duplicate entry errors in SQLAlchemy?"
Tracking down bugs with logging: "How do I enable SQL query logging in SQLAlchemy?"
Logging to a file: "Modify the logging setup to save the log output to a file on disk."
Handling transaction errors: "How do I handle transaction errors in SQLAlchemy?"
Debugging queries: "How do use the EXPLAIN feature in SQLAlchemy to debug queries?"
```

#### **Module 3: Software Design Patterns**

**Gang of Four patterns overview**

```
Exploring design Patterns: "Give me a high-level overview of the Gang of Four design patters."
```

**Patterns advice**

```
Building a financial services app: "You are an expert Python developer who builds readable code. Together we will work on an application that has a database to store information, code to retrieve data from the database, and analytics that will run on the retrieved data. First, let's create the database, which has a table for companies. The table will have three columns, the first is an id, the second the ticker for the company, the third is the name of the company. Create this, and synthesize data for 10 companies, adding that to the database."

Loading and processing company data: "Now create code that when given a company ticker or an ID that it will extract the data for that company, and the time series data and load it into an company object. This object should have fields for high_bollinger which is the same data type as the time series, low_bollinger which is the same, moving_average which is the same, and a grade field which is a string."

Requesting design pattern advice: "You are an expert in software design patterns, particularly those from the Gang of Four, designed to make coding and maintenance more efficient. Please analyze the following code and suggest some changes that I could make based on good software engineering practice with these design patterns."

Requesting design pattern advice iteratively: "Instead of making all the changes at once, please do them one at a time, going in order from Singleton to Factory to template Method to Strategy, and explain in detail why you made the changes and what impact they may have."

"Enhance the following code  to use the Gang of Four patterns.  Strictly follow the common conventions  for any patterns that you choose."
```

**Factory Patterns**

```
Implementing the Factory Pattern: "Enhance the following code to use the Factory gang-of-four pattern. Strictly follow the common conventions for the pattern. Start by explaining the conventions for the Factory pattern and why it makes sense to use it here. Then describe how the code modifications you made strictly follow the conventions of the pattern. YOUR CODE HERE..."

Multiple company types using the Factory Pattern: "Go back to the code that adds data to the database and synthesize some foreign companies (which will have a unique ID, but the ticker is always 'ZZZZ') and the data for them, both in the companies table and in the time series table. Then fully explain the Factory pattern by having multiple company types -- a Domestic Company that is denoted by its ticker, and a Foreign Company that is denoted by its ID. Create code that shows how."
```

**Template Method Pattern**

```
Requesting Information on the Template Pattern: "Great - the third pattern you mentioned was the Template Method pattern. Can you demonstrate where, how, and why you would use it in this code? What advantages would it provide?"
```
