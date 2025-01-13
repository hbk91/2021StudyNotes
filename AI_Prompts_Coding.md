---
title: "AI Prompts for Coding"
author: "Aman Jindal"
description: "Notes"
---

## Summary:
 
### **Requirements & Design**

| **S No.** | **Prompt Type**            | **Overview**                                                | **Use Case**                                             |
|-----------|----------------------------|------------------------------------------------------------|----------------------------------------------------------|
| **1**     | **Requirements Simulator** | Identifies gaps in system requirements early in the development cycle. | Useful for refining and completing requirements to save cost and effort. |
| **2**     | **Specification Disambiguation** | Clarifies ambiguous or vague requirements to prevent miscommunication. | Ideal for aligning team understanding before development begins. |
| **3**     | **API Generator**          | Generates an API specification from requirements.           | Facilitates early API formalization and rapid iteration. |
| **4**     | **API Simulator**          | Simulates APIs to test usability and validate assumptions.  | Enables iterative API development and usability testing. |

---

### **Improving Code Quality**

| **S No.** | **Prompt Type**       | **Overview**                                    | **Use Case**                                             |
|-----------|-----------------------|------------------------------------------------|----------------------------------------------------------|
| **1**     | **Code Clustering**   | Separates pure logic from side effects for better modularity. | Enhances code maintainability and testability.           |
| **2**     | **Intermediate Abstraction** | Adds a layer between business logic and dependencies to reduce coupling. | Simplifies future changes and reduces risk from external libraries. |
| **3**     | **Principled Code**   | Enforces adherence to design principles like SOLID in generated or refactored code. | Ensures maintainable and well-structured code.           |

---

### **Refactoring & Maintenance**

| **S No.** | **Prompt Type**           | **Overview**                                    | **Use Case**                                             |
|-----------|---------------------------|------------------------------------------------|----------------------------------------------------------|
| **1**     | **Pseudo-code Refactoring** | Refactors code to align with user-provided pseudo-code templates. | Offers control over structure without detailed coding requirements. |
| **2**     | **Data-guided Refactoring** | Adapts code to work with new input/output formats. | Simplifies refactoring processes when data formats evolve. |
| **3**     | **Hidden Assumptions**     | Identifies implicit assumptions in code to support better decisions. | Prepares code for future changes and refactoring.        |

---

### **General Prompt Design**

| **S No.** | **Prompt Type**               | **Overview**                                                | **Use Case**                                             |
|-----------|-------------------------------|------------------------------------------------------------|----------------------------------------------------------|
| **1**     | **Combination of Patterns**   | Combines complementary patterns (e.g., Requirements Simulator + Visualization Generator) for enriched outputs. | Creates multi-faceted prompts for richer, actionable outputs. |
| **2**     | **Few-shot Examples**         | Uses examples to iteratively train the LLM for desired outputs. | Ensures precision in tasks requiring context-specific understanding. |
| **3**     | **Context-specific Prompts**  | Tailors prompts for specific goals, such as Change Request Simulation. | Facilitates focused and goal-oriented outputs.           |

--- 
            
## **Prompts Explained:**

### ***Requirements & Design***

### 1. Requirements Simulator
- **Overview:** Simulates a system to identify gaps or missing requirements early in the development process.
- **Example:**
  - Prompt: "Now, I want you to act as this system. Use the requirements to guide your behavior. I will describe a task, and you will tell me if the task is possible based on the requirements. If not, write the missing requirements in user story format."
- **Use Case:** Useful for refining and completing requirements, reducing late-stage changes, and saving cost and effort.

---

### 2. Specification Disambiguation
- **Overview:** Clarifies ambiguous or vague requirements to ensure all team members have a shared understanding.
- **Example:**
  - Prompt: "The following are system requirements. Point out any areas that could be ambiguous or lead to unintended outcomes. Suggest ways to make the language more precise."
  - Requirements: 
    1. "Allow file uploads via a web browser."
    2. "Files must be secure."
    3. "Files should not exceed 100 MB."
- **Use Case:** Ideal for ensuring precise communication, particularly when requirements are written by non-technical stakeholders.

---

### 3. API Generator
- **Overview:** Converts a list of requirements or system descriptions into an API specification for software development.
- **Example:**
  - Prompt: "Generate an OpenAPI specification for a web application with the following features: user registration, file uploads, and activity logs. Include detailed descriptions for endpoints, inputs, and outputs."
- **Use Case:** Facilitates early API formalization, enabling rapid iteration and alignment between teams.

---

### 4. API Simulator
- **Overview:** Simulates APIs based on a specification, enabling developers to test usability, validate assumptions, and refine designs.
- **Example:**
  - Prompt: "Act as this API based on the provided OpenAPI specification. I will send HTTP requests in plain text, and you will respond with the appropriate HTTP responses. Update state based on interactions where necessary."
- **Use Case:** Enables iterative API development, allowing developers to validate and refine designs through interactive testing.

---

### ***Improving Code Quality***

### 1. Code Clustering
- **Overview:** Separates pure logic from side effects, such as file system access or network calls, to improve modularity and maintainability.
- **Example:**
  - Prompt: "Whenever you write code, separate functions with side effects (e.g., database queries, file I/O) from pure functions. Ensure the pure functions handle all business logic independently."
- **Use Case:** Enhances code maintainability, facilitates testing, and improves overall modularity.

---

### 2. Intermediate Abstraction
- **Overview:** Adds an intermediate layer between business logic and dependencies (e.g., third-party libraries) to reduce tight coupling.
- **Example:**
  - Prompt: "Separate the business logic from any third-party libraries by creating an abstraction layer. For example, replace direct API calls with a wrapper function or class that acts as an intermediary."
- **Use Case:** Simplifies future changes, reduces dependency risks, and ensures flexibility for replacing external libraries.

---

### 3. Principled Code
- **Overview:** Ensures that generated or refactored code adheres to well-known design principles, such as SOLID or DRY (Don't Repeat Yourself).
- **Example:**
  - Prompt: "Whenever you write, refactor, or review code, make sure it adheres to the SOLID design principles: single responsibility, open-closed, Liskov substitution, interface segregation, and dependency inversion."
- **Use Case:** Produces maintainable, scalable, and well-structured code by aligning with established best practices.

---

### ***Refactoring & Maintenance***

### 1. Pseudo-code Refactoring
- **Overview:** Refactors code to align with user-provided pseudo-code templates, giving users control over the structure without needing to provide detailed code.
- **Example:**
  - Prompt: 
    ```
    Refactor the following code to match this pseudo-code:
    files = scan_files()
    for file in files:
        print(file name)
    ```
    "Ensure the structure closely matches the provided pseudo-code."
- **Use Case:** Offers flexibility in reshaping code while maintaining control over the overall structure and flow.

---

### 2. Data-guided Refactoring
- **Overview:** Refactors code to adapt to new input/output formats or schema changes by using examples of the new data structure.
- **Example:**
  - Prompt: 
    ```
    Refactor the `process_data` function to handle the following new data format:
    {
      "graph": {...},
      "nodes": ["A", "B", "C"]
    }
    ```
    "Update the function to process this new schema."
- **Use Case:** Simplifies the process of adapting existing code to new data structures or formats, reducing manual effort.

---

### 3. Hidden Assumptions
- **Overview:** Identifies implicit assumptions in the code to make them explicit, enabling better decisions for future changes or refactoring.
- **Example:**
  - Prompt: "Analyze the following code and list any assumptions it makes about data, environment, or dependencies. For each assumption, estimate how hard it would be to modify."
- **Use Case:** Helps uncover hidden risks and prepares the codebase for flexibility and easier future modifications.

---

### ***General Prompt Design***

### 1. Combination of Patterns
- **Overview:** Combines complementary patterns, such as Requirements Simulator and Visualization Generator, to produce enriched and actionable outputs.
- **Example:**
  - Prompt: 
    ```
    Simulate the system using the requirements provided and generate a textual description of each screen. Additionally, provide a DALL-E prompt to create a wireframe for each screen.
    ```
- **Use Case:** Creates multi-faceted prompts to achieve richer outputs by combining simulations, visualizations, and refinements.

---

### 2. Few-shot Examples
- **Overview:** Uses examples to iteratively train the LLM to produce more accurate and context-specific results.
- **Example:**
  - Prompt: 
    ```
    Examples:
    Input: "The movie was thrilling but had a predictable ending."
    Output: Neutral sentiment.
    
    Input: "The movie was a waste of time."
    Output: Negative sentiment.
    
    Now classify the sentiment: "I enjoyed the acting but disliked the pacing."
    ```
- **Use Case:** Ensures precision in tasks requiring nuanced understanding by providing examples as a learning base.

---

### 3. Context-specific Prompts
- **Overview:** Tailors prompts to focus on specific goals or areas, such as simulating change requests or evaluating architectural designs.
- **Example:**
  - Prompt: 
    ```
    My software system uses the architecture you designed earlier. Simulate a change where we replace the database layer with a NoSQL database. List impacted modules and describe necessary changes.
    ```
- **Use Case:** Facilitates goal-oriented outputs, ensuring the LLM delivers focused and actionable results for specific scenarios.

---
