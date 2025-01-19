---
title: "AI Limits & Capabilities"
author: "Aman Jindal"
description: "Notes"
---

## **ChatGPT Limits**

*As of Jan 6, 2025*

| **Aspect**                  | **Details**                                                                                 |
|-----------------------------|--------------------------------------------------------------------------------------------|
| **Model**                   | GPT-4-turbo                                                                                |
| **Subscription**            | Paid version (e.g., ChatGPT Plus or API usage with GPT-4-turbo).                           |
| **Free Version Limits**     | Typically capped at **GPT-3.5** with similar token limits but less advanced capabilities.  |
| **Performance Differences** | GPT-4 offers better reasoning, contextual understanding, and overall accuracy than GPT-3.5. |   

### Input

| **Aspect**                 | **Details**                                                                                          |
|----------------------------|-----------------------------------------------------------------------------------------------------|
| **Max Tokens Per Input**   | Approximately 4,096 tokens (shared with output, includes input and output combined).               |
| **Characters Per Token**   | Average 4 characters per token (varies by text type).                                              |
| **Real Text Input**        | ~3,000 words (equivalent to ~6 pages of double-spaced text in a word processor).                   |
| **Markdown Input**         | Can handle Markdown documents up to ~4,000 characters, including detailed formatting, sections, and tables. |
| **Code Input**             | Length of a medium-size script (~150–300 lines of well-commented code).                           |
| **Constraints**            | Very long or complex input exceeding token limits will be truncated.                              |
| **Practical Translation**  | Input limit is sufficient for long documents, extensive datasets, and complex queries.            |

### Output

| **Aspect**                 | **Details**                                                                                          |
|----------------------------|-----------------------------------------------------------------------------------------------------|
| **Max Tokens Per Output**  | Approximately 4,096 tokens (includes input and output combined).                                   |
| **Characters Per Token**   | Average 4 characters per token (varies by text type).                                              |
| **Real Text Output**       | ~3,000 words (equivalent to ~6 pages of double-spaced text in a word processor).                   |
| **Markdown Output**        | Can generate detailed documents with up to ~4,000 characters of Markdown, including formatting, tables, and sections. |
| **Python Code**            | Length of a medium-size script (~150–300 lines of well-commented code).                           |
| **Constraints**            | Complex nested content or highly detailed responses may truncate earlier to meet token limits.     |
| **Practical Translation**  | Output is sufficient for detailed responses, multi-section documents, and robust code examples.    |

---

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

---

## **ChatGPT Data Analysis Capabilities**

| **Data Type**          | **Examples**                                  | **Capabilities**                                                                                               | **Technologies/Libraries Used**                       |
|-------------------------|----------------------------------------------|----------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| **Text Data**          | Word documents, PDFs, plain text files       | Text summarization, translation, editing, formatting, extracting key information, creating reports or outlines | Python libraries like **NLTK**, **spaCy**, **PyPDF2**, **docx**, **re** |
| **Spreadsheet Data**   | Excel files, CSV files                       | Data cleaning, formatting, analysis, visualization, pivot tables, formula creation, trend analysis            | **Pandas**, **openpyxl**, **xlrd**, **matplotlib**, **numpy** |
| **Numerical Data**     | Financial data, statistical datasets         | Perform calculations, create charts/graphs, statistical analysis, forecasting, and optimization                | **Numpy**, **scipy**, **statsmodels**, **matplotlib**, **pandas** |
| **Categorical Data**   | Survey results, sales records                | Data categorization, frequency analysis, segmentation, and clustering                                         | **Pandas**, **scikit-learn**, **seaborn**, **matplotlib** |
| **JSON/XML Data**      | API responses, structured data files         | Parsing, reformatting, extracting specific fields, and converting between formats                             | **JSON**, **xml.etree.ElementTree**, **BeautifulSoup** |
| **Geospatial Data**    | Location coordinates, GIS files              | Mapping, route optimization, clustering, distance calculations                                                | **Geopandas**, **folium**, **shapely**, **matplotlib** |
| **Time-Series Data**   | Stock prices, weather data                   | Trend analysis, forecasting, seasonal decomposition, anomaly detection                                        | **statsmodels**, **pandas**, **scipy**, **numpy**, **matplotlib** |
| **Images**             | PNG, JPG, SVG                               | OCR (text extraction), analysis of content (e.g., tags), resizing, basic processing                           | **Pillow (PIL)**, **OpenCV**, **Tesseract**, **matplotlib** |
| **Audio Files**        | MP3, WAV                                    | Transcription, summarization of speech content, keyword extraction                                            | **SpeechRecognition**, **pydub**, **wave**, **nltk**  |
| **Video Files**        | MP4, MOV                                    | Analyzing subtitles, summarizing content, extracting key frames                                               | **MoviePy**, **OpenCV**, **ffmpeg**                   |
| **Code Files**         | Python, Java, HTML, JSON, YAML, etc.         | Code review, debugging, refactoring, generating documentation, code conversion                                | **regex (re)**, **Black**, **PyLint**, **HTMLParser**, **pyyaml** |
| **Log Files**          | Server logs, error logs                     | Anomaly detection, pattern recognition, summarization                                                         | **Pandas**, **regex (re)**, **ElasticSearch**, **matplotlib** |
| **Scientific Data**    | Research datasets, experimental data        | Statistical analysis, hypothesis testing, visualizations, and report generation                               | **SciPy**, **NumPy**, **matplotlib**, **seaborn**, **statsmodels** |
| **Survey Data**        | Questionnaires, Google Form exports         | Aggregation, visualization, response analysis, and trend identification                                       | **Pandas**, **matplotlib**, **seaborn**, **scipy**    |
| **Health Data**        | Patient records, fitness tracker data       | Data anonymization, trend analysis, progress tracking                                                         | **Pandas**, **NumPy**, **matplotlib**, **scikit-learn** |
| **Natural Language Data** | Chat transcripts, customer feedback        | Sentiment analysis, topic modeling, keyword extraction                                                        | **NLTK**, **spaCy**, **TextBlob**, **Gensim**, **Pandas** |

---

## **ChatGPT Data Programming Language Capabilities**

| **Programming Language** | **Capabilities**                                                                                     | **Libraries/Tools**                                                                 |
|---------------------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Python**               | Data analysis, machine learning, web development, automation, API interaction, scripting, etc.      | **Pandas**, **NumPy**, **scikit-learn**, **Flask**, **Django**, **Matplotlib**, **TensorFlow** |
| **JavaScript**           | Web development, front-end frameworks, server-side scripting, API development                       | **Node.js**, **React**, **Vue.js**, **Express.js**, **D3.js**                     |
| **Java**                 | Android development, backend development, desktop applications, enterprise software                 | **Spring**, **Hibernate**, **JUnit**, **Maven**                                   |
| **HTML**                 | Structuring web pages, creating the content layer for web applications                              | Not applicable                                                                    |
| **CSS**                  | Styling web pages, animations, and layouts                                                         | **Bootstrap**, **TailwindCSS**, **Sass**                                          |
| **C++**                  | Game development, performance-critical applications, system programming                             | **OpenGL**, **Boost**, **Qt**                                                    |
| **C#**                   | Game development (Unity), Windows applications, web services                                       | **.NET Framework**, **Unity**                                                    |
| **SQL**                  | Database queries, data manipulation, reporting                                                     | **MySQL**, **PostgreSQL**, **SQLite**, **SQLAlchemy**                             |
| **R**                    | Statistical analysis, data visualization, machine learning                                         | **ggplot2**, **dplyr**, **caret**, **shiny**                                      |
| **MATLAB**               | Numerical analysis, simulations, data visualization                                               | MATLAB toolboxes                                                                 |
| **Bash/Shell**           | Scripting, automation, managing servers                                                           | Standard shell commands, **AWK**, **Sed**, **grep**                               |
| **PHP**                  | Web development, server-side scripting                                                             | **Laravel**, **CodeIgniter**, **WordPress**                                       |
| **Ruby**                 | Web development, scripting                                                                         | **Ruby on Rails**, **Sinatra**                                                   |
| **Go (Golang)**          | Cloud-native applications, APIs, concurrent programming                                           | **Gin**, **Echo**, **GORM**                                                      |
| **Kotlin**               | Android development, backend development                                                          | **Ktor**, **Spring Boot**                                                        |
| **Swift**                | iOS/macOS app development                                                                         | **SwiftUI**, **UIKit**                                                            |
| **TypeScript**           | Large-scale JavaScript applications with type safety                                              | **Angular**, **React**, **NestJS**                                               |
| **Scala**                | Functional programming, distributed systems, data processing                                      | **Akka**, **Play Framework**, **Spark**                                          |
| **Perl**                 | Text processing, scripting, bioinformatics                                                       | Standard libraries                                                               |
| **Rust**                 | Systems programming, web assembly, high-performance applications                                  | **Rocket**, **Tokio**, **Cargo**                                                 |
| **Haskell**              | Functional programming, academic projects                                                         | **GHC**, **Cabal**                                                               |
| **Dart**                 | Cross-platform development (Flutter)                                                             | **Flutter**                                                                      |
| **Lua**                  | Game scripting, lightweight applications                                                          | **LOVE2D**, **Torch**                                                            |
| **Julia**                | High-performance numerical computing, machine learning                                            | **Flux.jl**, **Plots.jl**, **DataFrames.jl**                                     |
| **Assembly**             | Low-level programming, system performance optimization                                            | Platform-specific assemblers                                                     |
| **YAML/JSON**            | Configuration management, data serialization                                                     | **PyYAML**, **JSON libraries**                                                   |

---

## **ChatGPT Software Capabilities**

| **Software**             | **Capabilities**                                                                                          | **Examples of Usage**                                                                           |
|---------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Microsoft Excel**      | Data analysis, cleaning, formatting, pivot tables, charts, advanced formulas, VBA scripting              | Automating reports, performing financial modeling, creating dashboards                         |
| **Microsoft Word**       | Document editing, formatting, template creation, mail merge                                             | Drafting reports, formatting templates, generating large documents with consistent styles      |
| **Microsoft PowerPoint** | Slide design, formatting, content creation, animations                                                  | Designing professional presentations, creating visual aids for pitches or lectures             |
| **Google Sheets**        | Online collaborative spreadsheets, data analysis, formula creation                                      | Live collaboration on datasets, data cleaning, creating shared dashboards                      |
| **Google Docs**          | Document editing, collaboration tools, formatting                                                      | Co-authoring reports, creating content drafts with comments or suggestions                     |
| **Google Slides**        | Slide creation, collaborative presentations                                                            | Team presentations, brainstorming sessions, interactive visuals                                 |
| **Adobe Acrobat**        | PDF editing, annotation, form creation, document conversion                                            | Filling forms, combining PDFs, extracting text/images                                          |
| **Visual Studio Code**   | Code editing, debugging, extensions for programming in multiple languages                              | Writing Python, JavaScript, HTML, or other code, debugging, and version control integration    |
| **Jupyter Notebook**     | Interactive Python coding, data visualization, and exploration                                         | Data analysis, machine learning experiments, tutorial creation                                 |
| **Tableau**              | Data visualization, dashboards, analytics                                                              | Creating interactive dashboards, presenting trends, sharing insights                           |
| **Power BI**             | Business intelligence, data modeling, visualization                                                    | Connecting to data sources, building reports, analyzing key metrics                            |
| **MATLAB**               | Numerical computing, algorithm development, visualization                                              | Running simulations, analyzing data, creating technical reports                                |
| **SPSS**                 | Statistical analysis, survey data analysis                                                             | Hypothesis testing, regression analysis, descriptive statistics                                |
| **RStudio**              | Statistical computing, data visualization, R programming                                               | Running R scripts, creating reports, conducting advanced data analysis                         |
| **Notepad++**            | Text editing, code editing, scripting                                                                  | Writing and editing configuration files, small code snippets                                   |
| **GIMP**                 | Image editing, graphic design                                                                          | Retouching images, creating banners, resizing or cropping visuals                              |
| **Canva**                | Graphic design, templates for social media posts, presentations                                        | Creating marketing materials, designing custom social media graphics                           |
| **Adobe Photoshop**      | Advanced image editing, graphic design                                                                 | Photo editing, compositing, creating professional visuals                                      |
| **Adobe Illustrator**    | Vector graphics design, logo creation, illustration                                                    | Designing logos, creating infographics, custom vector artwork                                  |
| **LaTeX (via Overleaf)** | Document preparation, academic writing, formatting for research papers                                 | Writing theses, academic papers, or creating professional-looking resumes                     |
| **Postman**              | API testing, integration debugging                                                                     | Testing RESTful APIs, sending requests, viewing responses, generating API documentation        |
| **Git**                  | Version control, collaboration on coding projects                                                      | Managing repositories, tracking changes, coordinating with teams using **GitHub** or **GitLab** |
| **Anaconda**             | Python data science environment, package management                                                   | Running Python scripts for data analysis, managing Python libraries                            |
| **SAP**                  | ERP software for finance, procurement, and HR tasks                                                   | Running financial reports, managing supply chain data                                          |
| **SQL Server Management Studio (SSMS)** | Database management, running queries, optimizing databases                                  | Writing SQL queries, creating databases, managing stored procedures                            |
| **AWS Console**          | Cloud service management, deployment of applications                                                   | Managing EC2 instances, configuring S3 storage, setting up Lambda functions                    |
| **Azure Portal**         | Cloud services, virtual machine and storage management                                                | Hosting apps, configuring VMs, managing Azure services                                         |
| **Slack**                | Communication, integrations with other software                                                       | Organizing team discussions, integrating project management tools                              |
| **Trello**               | Task management, project organization                                                                 | Creating boards for task tracking, managing workflows for teams                                |
| **Monday.com**           | Project management, timeline tracking, workflow automation                                            | Creating project plans, assigning tasks, tracking progress                                     |

---

## **ChatGPT Applications across Domains:**

### **Education**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Lesson Plan Template**        | A structured template with sections for objectives, activities, and evaluations.                     | Word, PDF            |
| **Student Progress Tracker**    | A tool to monitor grades, attendance, and performance over time.                                     | Excel, CSV           |
| **Interactive Learning Presentation** | A presentation with quizzes, animations, and visuals to engage students.                           | PowerPoint           |
| **Educational Ebook**           | A subject-specific ebook for self-paced learning.                                                    | ePub, PDF            |
| **Worksheet Generator**         | Automatically generates practice worksheets for math, science, or grammar.                          | Word, PDF            |
| **Visual Study Guide**          | A guide with diagrams and summaries to aid learning.                                                 | Images, PowerPoint   |
| **Assignment Tracker**          | A tracker for students to organize their deadlines and priorities.                                   | Excel, PDF           |
| **Flashcards**                  | Printable or digital flashcards for memorization of key concepts.                                   | Images, Word         |
| **Step-by-Step Lab Manual**     | A detailed manual for science experiments, with illustrations.                                       | Word, PDF            |
| **Certificate of Achievement**  | A customizable template for recognizing student accomplishments.                                    | Word, PDF            |

---

### **Finance**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Personal Budgeting Tool**     | A spreadsheet to automate expense tracking and monthly budgets.                                      | Excel                |
| **Financial Statement Template**| A template for income, expenses, and balance sheets.                                                 | Word, Excel          |
| **Investment Portfolio Tracker**| A tracker with visual graphs for asset allocation and performance monitoring.                        | Excel, PowerPoint    |
| **Financial Planning Guide**    | A written guide for personal or small business financial planning.                                   | Word, ePub, PDF      |
| **Tax Calculator**              | A tool with fields for deductions, credits, and tax liability calculations.                         | Excel, PDF           |
| **Loan Repayment Calculator**   | A schedule calculator to break down payments into principal and interest.                           | Excel                |
| **Monthly Financial Report**    | A report template with key financial metrics for stakeholders.                                      | PowerPoint, Word     |
| **Expense Tracker Template**    | A simple tracker for categorizing and monitoring expenses.                                           | Excel, CSV           |
| **Financial Ratios Guide**      | A visual guide explaining key financial ratios for business analysis.                               | Images, PowerPoint   |
| **Cash Flow Forecast Template** | A forecasting template for managing business cash flow.                                             | Excel, Word          |

---

### **Sales**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Sales Tracking Dashboard**    | A dashboard to monitor sales performance by product, region, or salesperson.                         | Excel, CSV           |
| **Product Catalog**             | A detailed catalog with product descriptions and visuals for customers.                              | Word, PDF            |
| **Sales Pitch Presentation**    | A polished presentation to pitch products or services to clients.                                    | PowerPoint           |
| **Sales Training Manual**       | A comprehensive manual for onboarding new sales team members.                                        | Word, PDF            |
| **Commission Calculator**       | A tool to calculate salesperson earnings based on performance.                                       | Excel                |
| **Monthly Sales Report**        | A report template summarizing sales achievements and trends.                                         | PowerPoint, PDF      |
| **Customer Contact Tracker**    | A tracker for managing leads, follow-ups, and sales pipelines.                                       | Excel, CSV           |
| **Sales Comparison Chart**      | A visual chart comparing sales performance over different periods.                                   | Excel, PowerPoint    |
| **ROI Analysis Template**       | A tool for evaluating the profitability of products or campaigns.                                   | Excel, Word          |
| **Client Brochure**             | A professional brochure highlighting product features and benefits.                                  | Word, PDF            |

---

### **Marketing**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Marketing Campaign Planner**  | A planner with timelines and milestones for executing campaigns.                                     | Excel, PowerPoint    |
| **Content Calendar Template**   | A template for scheduling and organizing social media posts.                                         | Excel, PDF           |
| **Campaign Presentation**       | A presentation to pitch and showcase marketing campaign ideas.                                       | PowerPoint           |
| **Infographic**                 | A visual representation of campaign results or customer demographics.                                | Images, PDF          |
| **Digital Marketing Guide**     | A guide on strategies and best practices for digital marketing.                                      | Word, ePub           |
| **Conversion Tracker**          | A tool to monitor website and email campaign conversions.                                            | Excel, CSV           |
| **Customer Persona Template**   | A document template to define and describe target audiences.                                         | Word, PDF            |
| **Social Media Dashboard**      | A visual dashboard with KPIs and performance metrics for social media.                              | Excel, PowerPoint    |
| **Monthly Marketing Report**    | A report summarizing marketing metrics and outcomes for stakeholders.                               | PowerPoint, Word     |
| **Promotional GIF or Video**    | A dynamic visual asset for product launches or campaigns.                                            | GIFs, Movies         |

---

### **Leadership**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Leadership Guide**            | A guide with effective leadership techniques and strategies.                                         | Word, ePub           |
| **Team Goal-Setting Template**  | A structured template for setting SMART goals for teams.                                             | Word, PDF            |
| **Team Performance Tracker**    | A tracker to monitor team progress and accomplishments.                                              | Excel, CSV           |
| **Leadership Workshop Slides**  | A presentation for training teams on leadership best practices.                                      | PowerPoint           |
| **Conflict Resolution Guide**   | A manual for resolving team conflicts effectively.                                                   | Word, PDF            |
| **Organizational Chart Template**| A visual representation of team structures and roles.                                               | Word, PowerPoint     |
| **Feedback Tracker**            | A tool for collecting and organizing employee feedback during reviews.                              | Excel, PDF           |
| **Collaboration Guide**         | A guide with strategies for improving team collaboration and synergy.                               | Word, PDF            |
| **Goal-Setting Workbook**       | A workbook with exercises to develop leadership goals.                                              | Word, ePub           |
| **Leadership Success Dashboard**| A dashboard tracking key leadership metrics and progress.                                           | PowerPoint, Excel    |

---

### **Management**

| **Idea**                        | **Description**                                                                                       | **File Type**        |
|----------------------------------|-------------------------------------------------------------------------------------------------------|----------------------|
| **Project Timeline Template**   | A Gantt chart for planning and tracking project milestones.                                           | Excel, PDF           |
| **Resource Allocation Tracker** | A tool for assigning and managing resources across projects.                                          | Excel, CSV           |
| **Task Management Dashboard**   | A dashboard to manage workflows and tasks for team projects.                                         | Excel, PowerPoint    |
| **Manager’s Handbook**          | A written guide on management policies and best practices.                                           | Word, ePub, PDF      |
| **Risk Assessment Template**    | A template for identifying and evaluating project risks.                                             | Word, PDF            |
| **Meeting Agenda Template**     | A structured agenda for effective team meetings.                                                     | Word, PDF            |
| **Project Status Report**       | A template for summarizing key project metrics and updates.                                          | PowerPoint, PDF      |
| **Decision-Making Matrix**      | A tool to evaluate and compare decision options.                                                     | Excel, Word          |
| **Performance Improvement Plan**| A template for creating structured plans to help underperforming employees.                         | Word, PDF            |
| **Time Management Workbook**    | A workbook with trackers and exercises to improve time management.                                  | Word, PDF            |

---