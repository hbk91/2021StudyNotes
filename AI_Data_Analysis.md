---
title: "AI Data Analysis"
author: "Aman Jindal"
description: "Notes"
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

#### **Prompt**

Let's create a traceability document to ensure that others can:

1. **Know what data was used.**
2. **Understand how the analysis was performed.**
3. **Identify threats to validity.**

We want a guide for someone else to be able to replicate and understand the limitations of the analysis.

#### **Prompt**

Save the traceability information as a `README.md`

#### **Prompt**
For each analysis and visualization:

1. **Create a single Python script** that performs the analysis and produces the visualization.
   - The script can assume that the files used are in the same directory as the script.

2. **Save each Python file** with a prefix identifying the analysis it is related to.

3. **Output a table** listing:
   - The analysis,
   - The file name of the Python script,
   - A one-sentence description of what it does.

#### **Prompt**
Create a file named **SCRIPTS.md** that includes:

1. A **table** listing:
   - Each script file,
   - A summary of the analysis associated with it.

2. **A section for each script** that explains:
   - How to run the script,
   - How it works.

#### **Prompt**
Create a file called **SOURCES.md** that indicates that all of the data can be downloaded from: "our link"

#### **Prompt**
Now, combine the README.md, SOURCES.md, SCRIPTS.md, the scripts, and the original data into a zip file that I can download and that would allow others to replicate this analysis.

---

### **Data Analysis Approaches**

- AI knowledge/reasoning based
- Programmatic


