---
title: "AI Data Analysis"
author: "Aman Jindal"
description: "Notes"
---


# **Ten Strategies for ChatGPT Advanced Data Analysis**

| **SNo.** | **Strategy**                              | **Description**                                                                         | **Example**                                                                                                                                                                                                                                                                                                         |
|-------|-------------------------------------------|-----------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **1** | **Save Progress at Milestones**           | Prevent loss of work and maintain flexibility for changes.                              | Save intermediate files at key stages. Use these to restart, combine outputs, or explore alternative approaches. Request a zip file for easy management of generated files.                                                                                                 |
| **2** | **Create Detailed Plans**                 | Ensure consistency and simplify task repetition.                                        | Work with ChatGPT to outline actionable steps. Save these plans to reuse for similar tasks or to restart a process seamlessly.                                                                                                                                               |
| **3** | **Maintain Status Summaries**             | Keep track of progress and remaining tasks.                                             | Generate files summarizing the workflow, current step, and completed actions. These summaries help resume work or clarify context for ChatGPT.                                                                                                                              |
| **4** | **Align Understandings**                  | Ensure mutual clarity on provided documents or data.                                    | Ask ChatGPT to explain data or documents, then test its understanding by requesting examples or hypothetical applications.                                                                                                                                                   |
| **5** | **Test for Accuracy**                     | Validate outputs to ensure reliability.                                                 | Use identifiers or specific references to verify results. Simulate processes with synthetic data to test accuracy and workflows.                                                                                                                                            |
| **6** | **Explore Backup Methods**                | Overcome challenges when a method fails.                                                | Request ChatGPT to outline alternative strategies, providing context or suggestions for improvement if needed.                                                                                                                                                               |
| **7** | **Set Clear Goals**                       | Focus outputs to meet specific needs effectively.                                       | Clearly define objectives, constraints, and requirements. Be precise to guide ChatGPT in producing the most relevant solutions.                                                                                                                                              |
| **8** | **Fix Issues Promptly**                   | Avoid compounding errors during tasks.                                                  | Correct mistakes immediately by editing problematic inputs and regenerating outputs. Maintain a clean history for better results.                                                                                                                                           |
| **9** | **Provide Complete Context**              | Strengthen problem-solving with shared understanding.                                   | Include all relevant information in conversations to ensure ChatGPT has the full context needed for accurate reasoning and solutions.                                                                                                                                       |
| **10**| **Leverage Manual Analysis**              | Optimize results for unstructured text tasks.                                           | Direct ChatGPT to analyze or summarize text without Python when coding isn’t necessary. This approach avoids overcomplicating textual tasks.                                                                                                                                |

---

## **Data Analysis Approaches**

- Knowledge based
- Reasoning based
- Programmatic based

---

## **Traceability of Analysis/Chats**

### **Goal**

| **File Name**         | **Purpose**                                                                                                  |
|------------------------|------------------------------------------------------------------------------------------------------------|
| **README.md**          | Serves as the primary documentation for the project. Includes details about data sources, analysis methods, threats to validity, and instructions for replication. |
| **SCRIPTS.md**         | Lists all Python scripts with summaries of their functionality and includes sections explaining how to run and understand each script. |
| **SOURCES.md**         | Provides links to the data sources used in the project, ensuring transparency and easy access for replication.                     |
| **Python Scripts**     | Each script performs a specific analysis or visualization and is designed to work with data files in the same directory.            |
| **Data Files**         | Includes the raw data used in the analysis to allow others to replicate the results.                                             |
| **Project Zip File**   | Combines all files (README.md, SOURCES.md, SCRIPTS.md, scripts, and data files) into a single archive for easy downloading and replication. |

### **AI Prompts**

#### **Documenting the work**

Let's create a traceability document to ensure that others can:

1. **Know what data was used.**
2. **Understand how the analysis was performed.**
3. **Identify threats to validity.**

We want a guide for someone else to be able to replicate and understand the limitations of the analysis.

#### **Converting document to Markdown**

Save the traceability information as a `README.md`

#### **Prompting to output Python scripts used**

For each analysis and visualization:

1. **Create a single Python script** that performs the analysis and produces the visualization.
   - The script can assume that the files used are in the same directory as the script.

2. **Save each Python file** with a prefix identifying the analysis it is related to.

3. **Output a table** listing:
   - The analysis,
   - The file name of the Python script,
   - A one-sentence description of what it does.

#### **Markdown Summary of Scripts**

Create a file named **SCRIPTS.md** that includes:

1. A **table** listing:
   - Each script file,
   - A summary of the analysis associated with it.

2. **A section for each script** that explains:
   - How to run the script,
   - How it works.

#### **Summary of Data Sources in Markdown**

Create a file called **SOURCES.md** that indicates that all of the data can be downloaded from: "our link"

#### **Zip  of all the files**

Now, combine the README.md, SOURCES.md, SCRIPTS.md, the scripts, and the original data into a zip file that I can download and that would allow others to replicate this analysis.

---

## **Data Creation:**

#### **Structured Data from Unstructured Data**

- You can paste any randomly formatted data, and then can say something like: Please convert this into CSV Format: 
  - Name, Description, Topic (1-word)
  - Next row...
  
---

## **Content for PowerPoint:**

Step 1: Create your narrative/story for all the slides, typically broken down into sections
Step 2: Ask AI for, "Save each element of the narrative that is separated by a horizontal rule as a separate text file."
Step 3: Upload your Powerpoint template, and ask, "Now, read each file in one by one and insert the text as a slide in the attached PowerPoint template. Put the text into a Title and Content slide as the Content. Populate the title as well"

---

## **Creating Spreadsheet Templates from Scratch**

- We can upload any document and ask AI to create a spreadsheet model to track it. It is useful for procedural things like Expense/Travel Policies
- We can ask for the spreadsheet structure, and then ask AI to actually create one.
- We can then ask it to populate it with sample data.
- We can turn the spreadsheet into a checklist as well.

---

## **Excel Charts**

To create a chart in Excel from a Chart that AI has created in Python/or a screenshot you posted

### Full-Proof Approach:

Break the process in two steps: Putting the data together in a convenient format in Excel, and then plotting the data.
- For replicating this in Excel, what columns are required to make it as easy as possible to visualize/plot? Guide me on creating those columns.
- Then, give me step by step process of creating the visual in Excel.

### Short-cut:

Again, two steps. But in the first step directly ask AI to output the data required for plotting as a CSV/Excel file.
- Give me the data required to create this, visual as a CSV/Excel File. **(This step may result in errors - Need to verify what AI is giving us)**
- Then, give me step by step process of creating the visual in Excel.

### Checking your Excel Chart:

Suppose you want to compare two charts, or check your work. For example: One chart was produced by AI with Python, and you created the same chart in Excel
- Paste screenshots of both the pictures in the Prompt, and ask, "Other than legend, layout, color, fonts, any formatting, etc, Do you see any differences in the two charts, such that, the two charts may be materially different or based on different data"

