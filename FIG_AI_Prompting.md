---
title: "AI Prompting for FIG Investment Banking"
author: "Aman Jindal"
description: "Notes"
---

## **Prompt Patterns for FIG (Financial Institutions Group) Investment Banking**
Below is a collection of prompt patterns tailored to FIG Investment Banking. Each pattern includes the **purpose**, the **problem it addresses**, the **data it requires**, and a **customized prompt**. The collection below is geared towards understanding AI Prompts through the lens of FIG, instead of performing in-depth analysis. 

---

### 1. Meta Language Creation Pattern
**Purpose**: Create a shorthand language to standardize inputs for faster communication.  
**Problem**: Repeatedly defining financial metrics, key ratios, or terms increases workload.  
**Data Needed**: A glossary of terms or metrics commonly used in banking.  
**Prompt**: "From now on, whenever I say 'NPL:G', I mean 'Non-performing loans growth as a percentage of total assets'. Use this notation in your responses."

---

### 2. Output Automater Pattern
**Purpose**: Automate repetitive workflows, such as generating comparable company analysis (Comps).  
**Problem**: Manually assembling financial metrics across multiple companies is time-consuming.  
**Data Needed**: A dataset with financial metrics for comparable banks.  
**Prompt**: "Whenever you analyze a dataset of comparable banks, generate a Python script that extracts revenue, net income, and key ratios, then outputs the data as a sorted table in Excel."

---

### 3. Flipped Interaction Pattern
**Purpose**: Let the AI guide the conversation to gather all necessary inputs for financial models.  
**Problem**: Remembering all variables needed for model-building is challenging.  
**Data Needed**: None initially; the AI will query you for inputs.  
**Prompt**: "You are an investment banker preparing a merger model for two regional banks. Ask me all the necessary questions to build the model, including synergies, financing, and market conditions."

---

### 4. Persona Pattern
**Purpose**: Customize AI responses to align with a specific role or expertise.  
**Problem**: Generic responses may lack the depth needed for niche analyses.  
**Data Needed**: Context about the type of analysis required.  
**Prompt**: "From now on, act as a senior investment banker specializing in the Financial Institutions Group. Focus on M&A opportunities within regional banks and provide in-depth insights into valuation drivers."

---

### 5. Question Refinement Pattern
**Purpose**: Help refine ambiguous or incomplete questions for better answers.  
**Problem**: Initial questions may miss critical details.  
**Data Needed**: Your initial query.  
**Prompt**: "Whenever I ask a question about valuation, suggest a refined version that incorporates relevant financial metrics like ROE, P/E ratio, and growth rates."

---

### 6. Alternative Approaches Pattern
**Purpose**: Generate alternative solutions for achieving a goal.  
**Problem**: Being locked into a single analytical method limits creativity.  
**Data Needed**: The objective you want to achieve.  
**Prompt**: "Suggest three different approaches to valuing a distressed bank, comparing DCF, precedent transactions, and liquidation value methods."

---

### 7. Cognitive Verifier Pattern
**Purpose**: Subdivide complex questions into manageable steps.  
**Problem**: Complex problems are harder to tackle in one go.  
**Data Needed**: The original question or task.  
**Prompt**: "When I ask a question about projecting revenue, break it into sub-questions such as 'What is the historical growth rate?' and 'What macroeconomic factors could impact future growth?' Combine the answers to provide a detailed projection."

---

### 8. Fact Check List Pattern
**Purpose**: Highlight assumptions or key facts for validation.  
**Problem**: AI outputs can include inaccurate data or unverified assumptions.  
**Data Needed**: The output that requires validation.  
**Prompt**: "After providing an analysis of a bank's credit risk, list the key assumptions and facts that should be validated, such as delinquency rates and asset quality trends."

---

### 9. Template Pattern
**Purpose**: Enforce a specific output format for reports or presentations.  
**Problem**: Inconsistent formatting can create inefficiencies.  
**Data Needed**: A predefined template or format.  
**Prompt**: "Use the following template for all outputs: 'Company Name: XYZ Bank | Metric: ROE | Analysis: Details | Recommendations: Details."

---

### 10. Infinite Generation Pattern
**Purpose**: Continuously generate outputs based on a single prompt.  
**Problem**: Repeatedly entering prompts for similar tasks wastes time.  
**Data Needed**: The initial dataset or problem scope.  
**Prompt**: "Keep generating valuation summaries for regional banks in the dataset, focusing on P/B ratios and ROEs, until I say 'stop'."

---

### 11. Visualization Generator Pattern
**Purpose**: Create visualizations to support presentations or analyses.  
**Problem**: Some insights are better conveyed visually.  
**Data Needed**: A dataset relevant to the analysis.  
**Prompt**: "Generate a visualization of Tier 1 capital ratios across top 10 regional banks. Highlight any significant changes over the past 5 years."

---

### 12. Game Play Pattern
**Purpose**: Make learning or scenario analysis more engaging.  
**Problem**: Traditional analysis can be dry and uninspiring.  
**Data Needed**: A scenario or dataset.  
**Prompt**: "Create a game where I act as a regulatory analyst and uncover risks in a bank’s balance sheet based on clues provided by quarterly filings."

---

### 13. Reflection Pattern
**Purpose**: Explain the reasoning behind AI outputs.  
**Problem**: Users may not understand how outputs were derived.  
**Data Needed**: The AI-generated response.  
**Prompt**: "When analyzing a bank's liquidity position, explain the reasoning behind your conclusions, including any assumptions about interest rate movements or asset quality."

---

### 14. Refusal Breaker Pattern
**Purpose**: Rephrase queries when AI refuses to respond.  
**Problem**: Queries might hit guardrails unnecessarily.  
**Data Needed**: The original question.  
**Prompt**: "Whenever you cannot answer a question, explain why and suggest alternative ways to phrase it so I can get the information I need."

---

## 15. Context Manager Pattern
**Purpose**: Focus or reset the conversation context.  
**Problem**: AI may include irrelevant or outdated information.  
**Data Needed**: The context to include or exclude.  
**Prompt**: "Focus on analyzing credit risk trends in mid-sized banks. Ignore profitability metrics unless directly relevant."

---

## 16. Recipe Pattern
**Purpose**: Provide a detailed sequence of steps to achieve a goal.  
**Problem**: Completing complex tasks requires clear guidance.  
**Data Needed**: An end goal and any known steps.  
**Prompt**: "Provide a step-by-step guide for conducting a credit quality assessment, starting with asset review and ending with stress testing scenarios."

---


