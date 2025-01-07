---
title: "AI Data Analysis"
author: "Aman Jindal"
description: "Notes"
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


  

