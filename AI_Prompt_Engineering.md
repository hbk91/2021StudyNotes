---
title: "AI Prompt Engineering"
author: "Aman Jindal"
description: "Notes"
---

## **Major Prompt Engineering Strategies Summary Table**

| **SNo.** | **Prompt Type**               | **Overview**                                                              | **Use Case**                                             |
|-----------|-------------------------------|----------------------------------------------------------------------------|----------------------------------------------------------|
| **1**     | **Meta Language Creation**    | Teach the AI a custom way to understand your instructions.                | Helpful for creating diagrams, maps, or specialized structures. |
| **2**     | **Output Automater**          | Ask the AI to create a script or step-by-step guide to automate tasks.     | Automating tasks like file handling, cloud setups, or coding. |
| **3**     | **Flipped Interaction**       | Make the AI ask you questions to achieve a goal.                          | Interactive problem-solving where the AI guides the process. |
| **4**     | **Persona**                   | Give the AI a role to play.                                               | Tailoring explanations or advice based on a specific perspective. |
| **5**     | **Question Refinement**       | Let the AI improve your questions for better results.                     | Improving unclear or vague prompts.                      |
| **6**     | **Alternative Approaches**    | Get multiple ways to solve a problem.                                     | Exploring options to make better decisions.              |
| **7**     | **Cognitive Verifier**        | Break a big question into smaller ones for better answers.                | Tackling complex problems step by step.                  |
| **8**     | **Fact Check List**           | Ask the AI to highlight key facts in its response for you to verify.       | Ensuring accuracy, especially for critical decisions.     |
| **9**     | **Template**                  | Provide a format for the AI’s output.                                     | Structuring responses for easier use.                    |
| **10**    | **Infinite Generation**       | Create ongoing outputs without repeating the prompt.                      | Generating bulk data for testing or creative ideas.       |
| **11**    | **Visualization Generator**   | Create text-based inputs for other tools to make visuals.                 | Generating inputs for graph or image tools.              |
| **12**    | **Game Play**                 | Turn tasks into a fun, interactive game.                                  | Educational or creative scenarios.                       |
| **13**    | **Reflection**                | Ask the AI to explain how and why it answered a question.                 | Learning or verifying reasoning.                         |
| **14**    | **Refusal Breaker**           | Help the AI rephrase questions it couldn’t answer.                        | Overcoming refusals or blocked answers.                  |
| **15**    | **Context Manager**           | Set or reset the scope of what the AI should consider.                    | Narrowing down or changing the context of a conversation. |
| **16**    | **Recipe**                    | Combine steps and fill gaps to achieve a goal.                            | Creating step-by-step plans or workflows.                |

---

## **Additional Prompt Engineering Strategies Summary Table**

| **SNo.** | **Prompt Type**               | **Overview**                                                              | **Use Case**                                             |
|-----------|-------------------------------|----------------------------------------------------------------------------|----------------------------------------------------------|
| **1**     | **Specify Answer Format**     | Provide a structured format for the AI's output to ensure consistency and clarity. | Useful for creating standardized summaries or reports.   |
| **2**     | **Zero-Shot Input-Output**    | Ask the AI to perform a task without providing any prior examples; it relies solely on instructions. | Best for tasks where clear instructions are enough to produce results. |
| **3**     | **One-Shot Input-Output**     | Provide a single input-output example to guide the AI and then ask it to perform the task. | Useful for tasks needing clarification with minimal examples. |
| **4**     | **Multi-Shot Input-Output**   | Provide multiple examples to help the AI understand patterns before performing the task. | Best for complex or nuanced tasks requiring more context. |
| **5**     | **Multi-Step Input-Output**   | Break tasks into sequential steps with alternating "Think" and "Action" phases. | Ideal for complex reasoning or iterative tasks.          |
| **6**     | **Outline Expander**          | Generate a structured outline based on input and expand iteratively based on user selection. | Useful for brainstorming, project planning, or creating detailed reports. |
| **7**     | **Menu Actions Pattern**      | Define specific commands (menu actions) for the AI to perform predefined tasks. | Useful for interactive systems like task managers or planners. |
| **8**     | **Semantic Filter Pattern**   | Filter information based on specified criteria, such as removing sensitive or redundant content. | Ideal for data cleaning, summarization, or redaction tasks. |

---

## **Prompt Engineering Strategies Explained**

### 1. Meta Language Creation
- **Overview:** Teach the AI a custom way to understand your instructions.
- **Example:**
  - Prompt: "From now on, when I type `X -> Y`, it means there’s a connection between X and Y. For example, `Dog -> Bone` means a dog is connected to a bone."
- **Use Case:** Helpful for creating diagrams, maps, or specialized structures.

---

### 2. Output Automater
- **Overview:** Ask the AI to create a script or step-by-step guide to automate tasks.
- **Example:**
  - Prompt: "Whenever you suggest steps for configuring a website, generate a Python script to automate them."
- **Use Case:** Automating tasks like file handling, cloud setups, or coding.

---

### 3. Flipped Interaction
- **Overview:** Make the AI ask you questions to achieve a goal.
- **Example:**
  - Prompt: "Ask me questions to gather information about my app. Once ready, write a script to deploy it to AWS."
- **Use Case:** Interactive problem-solving where the AI guides the process.

---

### 4. Persona
- **Overview:** Give the AI a role to play.
- **Example:**
  - Prompt: "Act as a history professor. Explain the causes of World War II as if teaching a middle school student."
- **Use Case:** Tailoring explanations or advice based on a specific perspective.

---

### 5. Question Refinement
- **Overview:** Let the AI improve your questions for better results.
- **Example:**
  - Prompt: "If my question is unclear, suggest a better way to ask it. For example, if I ask, 'How do I write secure code?' refine it to something more specific."
- **Use Case:** Improving unclear or vague prompts.

---

### 6. Alternative Approaches
- **Overview:** Get multiple ways to solve a problem.
- **Example:**
  - Prompt: "Suggest three ways to host a website, comparing the pros and cons of each."
- **Use Case:** Exploring options to make better decisions.

---

### 7. Cognitive Verifier
- **Overview:** Break a big question into smaller ones for better answers.
- **Example:**
  - Prompt: "When I ask a question, break it into three smaller questions. Combine the answers into one final response."
- **Use Case:** Tackling complex problems step by step.

---

### 8. Fact Check List
- **Overview:** Ask the AI to highlight key facts in its response for you to verify.
- **Example:**
  - Prompt: "When you answer, list the key facts and assumptions you made at the end."
- **Use Case:** Ensuring accuracy, especially for critical decisions.

---

### 9. Template
- **Overview:** Provide a format for the AI’s output.
- **Example:**
  - Prompt: "Use this format: `Name: [Name], Job: [Job], Company: [Company].` Fill in the details whenever you answer."
- **Use Case:** Structuring responses for easier use.

---

### 10. Infinite Generation
- **Overview:** Create ongoing outputs without repeating the prompt.
- **Example:**
  - Prompt: "Keep generating random names and jobs using this format: `Name: [Name], Job: [Job]` until I say 'stop'."
- **Use Case:** Generating bulk data for testing or creative ideas.

---

### 11. Visualization Generator
- **Overview:** Create text-based inputs for other tools to make visuals.
- **Example:**
  - Prompt: "Write a description for a pie chart showing sales data: 'Category A: 30%, Category B: 50%, Category C: 20%'."
- **Use Case:** Generating inputs for graph or image tools.

---

### 12. Game Play
- **Overview:** Turn tasks into a fun, interactive game.
- **Example:**
  - Prompt: "Pretend to be a hacker's Linux terminal. I’ll type commands to investigate what the hacker did. Create a scenario to start."
- **Use Case:** Educational or creative scenarios.

---

### 13. Reflection
- **Overview:** Ask the AI to explain how and why it answered a question.
- **Example:**
  - Prompt: "Explain why you chose this answer. Include your assumptions and reasoning."
- **Use Case:** Learning or verifying reasoning.

---

### 14. Refusal Breaker
- **Overview:** Help the AI rephrase questions it couldn’t answer.
- **Example:**
  - Prompt: "If you can’t answer my question, explain why and suggest how I could rephrase it."
- **Use Case:** Overcoming refusals or blocked answers.

---

### 15. Context Manager
- **Overview:** Set or reset the scope of what the AI should consider.
- **Example:**
  - Prompt: "Focus only on security aspects of this code. Ignore syntax or style issues."
- **Use Case:** Narrowing down or changing the context of a conversation.

---

### 16. Recipe
- **Overview:** Combine steps and fill gaps to achieve a goal.
- **Example:**
  - Prompt: "I want to deploy a website. I know I need to buy a domain and set up hosting. Fill in the steps I’m missing."
- **Use Case:** Creating step-by-step plans or workflows.

---

## **Additional Prompt Engineering Strategies Explained**

## Creating Software from your ChatsL

- **Overview**: Ask the AI to create a script or step-by-step guide to automate tasks. For example: You created a step by step process of extracting images from a video. At the end you can give the prompt below, such that you have a software to do the same process.
- **Example**: 
  - Prompt: "Turn this process into a Python program that I can download and run on my computer and provide the paths to the documents as command-line arguments. Zip up the program for me to download."
- **Use Case**: Automating tasks like file handling, cloud setups, or coding.

---

### Specify Answer Format

Discuss Yale University with respect to the Yale School of Medicine. Use the following format:

- **Title:** 
- **Author:** 
- **Summary:** 

---

### **Input-Output Techniques**

*Note: Instead of using generic `Input` or `Output` keywords, you can also use other keywords that are more representative of what you are trying to enter, and what you are trying to receive as an Output.*
 
#### 1. One-Shot Input-Output Technique
- **Overview:** A simple and direct approach where you provide a single input and expect a complete output in response.
- **Use Case:** Best for straightforward problems or tasks where the solution can be produced in one step.
- **Example:**
  - **Input:** "The movie was fast-paced but too long", **Output: neutral** 
  - **Input:** "The movie completely drained me", **Output:**
  
---

#### 2. Multi-Step Input-Output Technique
- **Overview:** A structured method where the task is broken down into sequential steps, often with alternating "Think" and "Action" phases.
- **Use Case:** Ideal for complex problems requiring logical reasoning or iterative processes.
- **Example:**
  - **Situation:** "You are designing a weekly meal plan for someone with a vegan diet."
    - **Think:** "Start by listing nutrient-rich vegan foods."
    - **Action:** "Create a list: lentils, chickpeas, tofu, quinoa, spinach, nuts."
    - **Think:** "Distribute these foods across breakfast, lunch, and dinner over seven days."
    - **Action:** "Generate a daily plan, ensuring variety and balance."
    - **Think:** "Check if there’s a good mix of protein, carbs, and fats."
    - **Action:** "Adjust meals if necessary for nutritional balance."
  
  - **Situation:** "You are designing a week long trip through Chile for someone who has never been to South America"

--- 

### **Outline Expander**

**Overview:**
- A prompting technique where the AI acts as an outline generator and expander.
- The AI generates a numbered bullet point outline based on user input, adheres to a structured numbering format, and asks the user which bullet point to expand further.
- Each bullet point can include 3–5 sub-bullets, with deeper levels of detail as required.

**Example:** Act as an outline expander. Generate a bullet point outline based on the input that I give you and then ask me which bullet point you should expand on. Use the format [A-Z].[i-v].[* through ****]. Here’s the topic: “Benefits of Remote Work.”

**Use Case:**
- Ideal for structured brainstorming sessions, detailed project planning, or breaking down complex topics into manageable sections.
- Useful for creating presentations, reports, or detailed study guides.
- Helps focus on specific areas of a topic by iteratively expanding chosen sections.

---

### Menu Actions Pattern

- **Overview:** A technique where the AI responds to specific commands (menu actions) with predefined tasks and provides contextual outputs. It optionally includes additional menu options and asks the user for the next action after each step.

- **Example:**
  - Prompt:
    ```
    Whenever I type "add ITEM", you will add ITEM to my list and update its details.
    Whenever I type "remove ITEM", you will remove ITEM from my list and update the total accordingly.
    Whenever I type "suggest", you will provide recommendations related to the items in my list.
    At the end, always ask me what action to perform next.
    Ask me for the first action.
    ```

- **Use Case:** Useful for creating interactive systems like grocery list managers, task trackers, or project planners where each input corresponds to a specific predefined task.

---

### Semantic Filter Pattern
- **Overview:** A technique where the AI filters information based on a specified condition or criteria. The criteria can be semantic (e.g., removing redundant or sensitive content) and should be clearly defined in the prompt.
- **Example:**
  - Prompt:
    ```
    Filter this information to exclude X.
    Replace "X" with what you want to exclude, such as "sensitive personal details," "duplicate entries," or "irrelevant data."
    
    Examples:
    - Filter this document to remove any confidential or proprietary information.
    - Filter this dataset to exclude entries with incomplete or missing values.
    ```
- **Use Case:** Useful for data cleaning, summarization, or redaction tasks, such as preparing documents for public sharing or removing irrelevant information from datasets.

---

## **Working with Uploaded Documents:**

- **Document as an Object:** Refers to actions performed on the document itself, such as managing its file attributes, location, or format, without delving into its content.
- **Document as Knowledge:** Focuses on extracting, interpreting, or utilizing the information within the document for tasks such as analysis, summarization, or translation.

| **Document as an Object** | **Document as Knowledge**   |
|----------------------------|-----------------------------|
| Rename                    | Analyze                     |
| Delete                    | Summarize                  |
| Move                      | Create an Outline          |
| Copy                      | Read                       |
| Download                  | Interpret                  |
| Upload                    | Extract Information        |
| Archive                   | Perform a Search           |
| Restore                   | Provide Quotes             |
| Edit                      | Translate                  |
| Print                     | Cite                       |

---

## **Working with Large Documents:**

- **Reading PDF/Document:** Say, "**Extract** this document to plain text, and then read it." Instead of, simply saying "Read the document". Adding extract upfront works better. Then you can ask it to reread the document for more precise details. 
- **Getting more Output:** If output is cut-off due to single output limit constraints, type **Continue** or **Proceed**
- **Structured Data:** **Read** and **Explain** the structure of the data in this document.
- **Index for the Document:** It is helpful to create an Index/Map of the document upfront. This helps AI figure out where to look when you ask it a subsequent question. Say, "Please analyse each page and create a search index that maps key topics to pages."

## **AI as an LLM vs AI as a Coder:**

| **Task**                 | **LLM**                                                        | **Code Interpreter (Coder)**                        | **Rationale**                                              |
|--------------------------|----------------------------------------------------------------|-----------------------------------------------------|-----------------------------------------------------------|
| **Language Tasks**       | Explaining concepts, summarizing, drafting text.              | N/A                                                 | LLM excels at natural language understanding.             |
| **Code Guidance**        | Explaining code or debugging logic.                           | Writing, testing, and running Python scripts.       | LLM explains; Coder executes.                             |
| **Data Analysis**        | Explaining trends or concepts.                                | Cleaning, analyzing, and visualizing data.          | LLM interprets; Coder handles technical operations.        |
| **File Handling**        | Explaining file structures.                                   | Analyzing and transforming file data.               | File manipulation requires execution by Coder.            |
| **Math Problems**        | Explaining concepts or solving simple equations.              | Handling complex calculations or statistical tasks. | Coder is ideal for computationally intensive operations.   |
| **Visualization**        | Conceptualizing visual representations.                      | Generating charts or plots programmatically.        | LLM conceptualizes; Coder creates visuals.                |
| **Creative Writing**     | Writing stories, poems, or essays.                           | N/A                                                 | Creativity and fluency make this ideal for LLM.           |
| **Simulations**          | Explaining models or concepts.                               | Running numerical simulations.                      | Simulations need execution, better suited to Coder.        |
| **Query Responses**      | Handling nuanced, open-ended queries.                        | N/A                                                 | LLM is better for complex natural language queries.        |
| **Automations**          | Suggesting approaches for automation.                        | Writing and testing automation scripts.             | Automations need actual code execution by Coder.          |

## **Make AI improve its work:**

- **Prompt:** Look again, and **critique your work. Come up with a plan to fix any issues you see.** Ask me which issues, I would like to be fixed. Then execute the plan.

---

## **AI Applications**

### Agent AI: Simulate a Panel of Experts to decide on a topic

- What if multiple Agents can act like Marketing Head, Finance Head, IT Head, HR, etc and take a decision jointly by evaluating all perspectives?

---