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

## Prompts Explained:

