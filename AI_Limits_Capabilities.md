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