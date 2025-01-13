---
title: "AI Prompts Typology"
author: "Aman Jindal"
description: "Notes"
---

## **Prompt Engineering Strategies**

### 1. Meta Language Creation
- **What It Is:** Teach the AI a custom way to understand your instructions.
- **Example:**
  - Prompt: "From now on, when I type `X -> Y`, it means there’s a connection between X and Y. For example, `Dog -> Bone` means a dog is connected to a bone."
- **Use Case:** Helpful for creating diagrams, maps, or specialized structures.

---

### 2. Output Automater
- **What It Is:** Ask the AI to create a script or step-by-step guide to automate tasks.
- **Example:**
  - Prompt: "Whenever you suggest steps for configuring a website, generate a Python script to automate them."
- **Use Case:** Automating tasks like file handling, cloud setups, or coding.

---

### 3. Flipped Interaction
- **What It Is:** Make the AI ask you questions to achieve a goal.
- **Example:**
  - Prompt: "Ask me questions to gather information about my app. Once ready, write a script to deploy it to AWS."
- **Use Case:** Interactive problem-solving where the AI guides the process.

---

### 4. Persona
- **What It Is:** Give the AI a role to play.
- **Example:**
  - Prompt: "Act as a history professor. Explain the causes of World War II as if teaching a middle school student."
- **Use Case:** Tailoring explanations or advice based on a specific perspective.

---

### 5. Question Refinement
- **What It Is:** Let the AI improve your questions for better results.
- **Example:**
  - Prompt: "If my question is unclear, suggest a better way to ask it. For example, if I ask, 'How do I write secure code?' refine it to something more specific."
- **Use Case:** Improving unclear or vague prompts.

---

### 6. Alternative Approaches
- **What It Is:** Get multiple ways to solve a problem.
- **Example:**
  - Prompt: "Suggest three ways to host a website, comparing the pros and cons of each."
- **Use Case:** Exploring options to make better decisions.

---

### 7. Cognitive Verifier
- **What It Is:** Break a big question into smaller ones for better answers.
- **Example:**
  - Prompt: "When I ask a question, break it into three smaller questions. Combine the answers into one final response."
- **Use Case:** Tackling complex problems step by step.

---

### 8. Fact Check List
- **What It Is:** Ask the AI to highlight key facts in its response for you to verify.
- **Example:**
  - Prompt: "When you answer, list the key facts and assumptions you made at the end."
- **Use Case:** Ensuring accuracy, especially for critical decisions.

---

### 9. Template
- **What It Is:** Provide a format for the AI’s output.
- **Example:**
  - Prompt: "Use this format: `Name: [Name], Job: [Job], Company: [Company].` Fill in the details whenever you answer."
- **Use Case:** Structuring responses for easier use.

---

### 10. Infinite Generation
- **What It Is:** Create ongoing outputs without repeating the prompt.
- **Example:**
  - Prompt: "Keep generating random names and jobs using this format: `Name: [Name], Job: [Job]` until I say 'stop'."
- **Use Case:** Generating bulk data for testing or creative ideas.

---

### 11. Visualization Generator
- **What It Is:** Create text-based inputs for other tools to make visuals.
- **Example:**
  - Prompt: "Write a description for a pie chart showing sales data: 'Category A: 30%, Category B: 50%, Category C: 20%'."
- **Use Case:** Generating inputs for graph or image tools.

---

### 12. Game Play
- **What It Is:** Turn tasks into a fun, interactive game.
- **Example:**
  - Prompt: "Pretend to be a hacker's Linux terminal. I’ll type commands to investigate what the hacker did. Create a scenario to start."
- **Use Case:** Educational or creative scenarios.

---

### 13. Reflection
- **What It Is:** Ask the AI to explain how and why it answered a question.
- **Example:**
  - Prompt: "Explain why you chose this answer. Include your assumptions and reasoning."
- **Use Case:** Learning or verifying reasoning.

---

### 14. Refusal Breaker
- **What It Is:** Help the AI rephrase questions it couldn’t answer.
- **Example:**
  - Prompt: "If you can’t answer my question, explain why and suggest how I could rephrase it."
- **Use Case:** Overcoming refusals or blocked answers.

---

### 15. Context Manager
- **What It Is:** Set or reset the scope of what the AI should consider.
- **Example:**
  - Prompt: "Focus only on security aspects of this code. Ignore syntax or style issues."
- **Use Case:** Narrowing down or changing the context of a conversation.

---

### 16. Recipe
- **What It Is:** Combine steps and fill gaps to achieve a goal.
- **Example:**
  - Prompt: "I want to deploy a website. I know I need to buy a domain and set up hosting. Fill in the steps I’m missing."
- **Use Case:** Creating step-by-step plans or workflows.

---

## **Other Unique Strategies:**

### Specify Answer Format

Discuss Yale University with respect to the Yale School of Medicine. Use the following format:

- **Title:** 
- **Author:** 
- **Summary:** 

---

### **Input-Output Techniques**

*Note: Instead of using generic `Input` or `Output` keywords, you can also use other keywords that are more representative of what you are trying to enter, and what you are trying to receive as an Output.*
 
#### 1. One-Shot Input-Output Technique
- **What It Is:** A simple and direct approach where you provide a single input and expect a complete output in response.
- **Use Case:** Best for straightforward problems or tasks where the solution can be produced in one step.
- **Example:**
  - **Input:** "The movie was fast-paced but too long", **Output: neutral** 
  - **Input:** "The movie completely drained me", **Output:**
  
---

#### 2. Multi-Step Input-Output Technique
- **What It Is:** A structured method where the task is broken down into sequential steps, often with alternating "Think" and "Action" phases.
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

**What It Is:**
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

- **What It Is:** A technique where the AI responds to specific commands (menu actions) with predefined tasks and provides contextual outputs. It optionally includes additional menu options and asks the user for the next action after each step.

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
- **What It Is:** A technique where the AI filters information based on a specified condition or criteria. The criteria can be semantic (e.g., removing redundant or sensitive content) and should be clearly defined in the prompt.
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

## **AI Applications**

### Agent AI: Simulate a Panel of Experts to decide on a topic

- What if multiple Agents can act like Marketing Head, Finance Head, IT Head, HR, etc and take a decision jointly by evaluating all perspectives?