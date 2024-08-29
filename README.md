# ODSL-Jigsaw
Research Study: Improving Document Creation with ODSL and Jigsaw System
1.	Introduction
Creating documents, presentations, and spreadsheets can take a lot of time and effort, especially for people who aren’t experts with advanced software tools. This study explores how we developed the ODSL-Jigsaw system, a tool designed to make creating these documents easier. The system allows users to give commands in simple, everyday language, which are then turned into actions by the system using a combination of Domain-Specific Languages (DSLs) and program synthesis techniques.

2.	Research Question, Hypotheses, and Importance

2.1.	 Research Question: 
How can the ODSL-Jigsaw system improve the process of creating documents, presentations, and spreadsheets by using natural language commands combined with program synthesis techniques?
This question is the focus of our study. We wanted to see if combining these technologies could make document creation easier, faster, and more accurate for users.

2.2.	 Importance of the Research Question:
This research is important because it could change how people use productivity software. By allowing users to create complex documents using everyday language, the ODSL-Jigsaw system can make the process easier, reduce mistakes, and make advanced document creation tools more accessible.

2.3.	 Hypotheses:
1.	Domain-Specific Languages (DSLs):
1.	Hypothesis 1: Using a DSL made specifically for office tasks (like ODSL) will help users create complex documents with simple, natural language commands.
2.	Hypothesis 2: DSLs will help reduce mistakes and improve the accuracy of the documents generated by the system because they provide a clear way to understand user commands.
2.	Program Synthesis Techniques:
1.	Hypothesis 1: Using program synthesis techniques will improve the system’s ability to turn natural language into actions that create high-quality documents.
2.	Hypothesis 2: Program synthesis will make document creation faster and more efficient, saving users time on manual tasks.

3.	Research Methodology
3.1. Tools and Systems Developed:
•	ODSL-Jigsaw System: This is the main tool we developed to answer the research question. It combines ODSL (Office Domain-Specific Language) with program synthesis techniques to turn natural language commands into actions that create documents.
•	Python Libraries: The system uses python-docx for Word documents, openpyxl for Excel spreadsheets, and python-pptx for PowerPoint presentations. These libraries help generate and format documents based on the ODSL commands.
•	Large Language Models (LLMs): We used GPT-3.5 to help the system understand and process natural language commands from users.
3.2.  Solution Design:
•	MockNLToODSL: This part of the system translates natural language input into ODSL commands. For example, if a user says, "Create a budget report," this module turns that command into a series of steps that the system can follow.
•	ODSLParser: This component breaks down the ODSL commands into smaller tasks that the system can execute.
•	EnhancedExecutionEngine: This engine carries out the tasks, like creating a new document, inserting text, or formatting a slide.
•	DocumentGenerator: After the tasks are executed, this part of the system creates the final output files (e.g., .docx, .pptx, .xlsx).
•	QualityChecker: This component checks the generated documents to make sure they meet the specified requirements and quality standards.

3.3 Challenges and Solutions:
•	Challenge 1: Handling ambiguous user commands.
Solution: We designed the system to use predefined templates and examples to better interpret vague language.
•	Challenge 2: Managing complex, multi-step tasks.
Solution: We refined the ODSL structure to handle complex commands more effectively, ensuring accurate document formatting and content placement.

4.	How the Articles Helped Our Research
Our research and the development of the ODSL-Jigsaw system were influenced by two important articles:
4.1.  "Jigsaw: Large Language Models Meet Program Synthesis"
This article talks about combining Large Language Models (LLMs) like GPT-3 with program synthesis techniques to improve the quality of generated code. It introduced the idea of Jigsaw, a system that improves LLM outputs by adding steps before and after the main process.
•	How It Helped Our Research:
o	Inspiration for System Design: The idea of using extra steps to help LLMs was key to how we designed the ODSL-Jigsaw system. Our system’s pre-processing (MockNLToODSL) and post-processing (QualityChecker) components were inspired by this concept.
o	Program Synthesis Techniques: The article showed us the importance of program synthesis in improving LLM outputs. We used a similar approach to make sure natural language commands were accurately turned into actions in the ODSL-Jigsaw system.
4.2.  "Natural Language Commanding via Program Synthesis"
This article presented a system developed by Microsoft, which uses LLMs to translate natural language commands into actions within Office applications.
•	How It Helped Our Research:
o	Creating ODSL: The idea of creating a language specifically for Office tasks (ODSL) was inspired by this article. Our ODSL handles the unique needs of creating documents, presentations, and spreadsheets.
o	Understanding User Intent: The focus on understanding what the user wants and translating it into actions helped shape our system’s EnhancedExecutionEngine. This ensures that the user’s commands are carried out as intended.

5.	Research Execution
5.1 Preprocessing and Dataset:
The system preprocesses user commands by matching them with examples stored in the finalProjectPython file. This ensures the system understands what the user wants and generates the correct ODSL commands, making the process smooth and reliable.
5.3 Conclusions Answering the Research Question:
The ODSL-Jigsaw system successfully answers the research question by demonstrating that it can simplify the document creation process. By using natural language commands combined with program synthesis techniques, the system makes it easier and faster to create high-quality documents, presentations, and spreadsheets.
     5.3.1. Internal Performance Comparison:
•	Performance Comparison: In our internal testing, we compared the ODSL-Jigsaw system’s performance with traditional document creation methods. We noticed that the ODSL-Jigsaw system made tasks like creating a report, generating a budget spreadsheet, and preparing a presentation faster and easier. The time savings were especially clear in tasks that involved repetitive formatting or complex layouts.
•	Accuracy Assessment: We reviewed the documents generated by the ODSL-Jigsaw system to see how well they matched what we wanted. In most cases, the system produced accurate results that matched our expectations. 
•	Internal Satisfaction: Based on our own use, we found the ODSL-Jigsaw system to be user-friendly, especially with its natural language interface. The ability to generate documents without needing to manually adjust formatting was a big plus.

    5.3.2 Comparative Insights:
•	Comparison with Traditional Methods: Even though we didn’t conduct a formal user study, our experience with both the ODSL-Jigsaw system and traditional methods gave us valuable insights. We found that the ODSL-Jigsaw system could reduce the amount of effort needed to create documents by automating many repetitive tasks. This was different from traditional methods, where users often need to manually format and adjust documents, making the process longer.

6.	Work Process, Challenges, and Lessons Learned
Work Process:
The development involved several stages, including designing the ODSL, integrating it with the Jigsaw framework, and ensuring that the system could handle a wide range of document creation tasks.
Challenges:
•	Handling Ambiguous Commands: The system needed to interpret vague instructions accurately.
•	Complex Document Requests: The system sometimes struggled with tasks that required multiple steps and intricate formatting.
Lessons Learned:
The importance of a well-designed DSL became clear during development. We also realized the value of user feedback in refining the system to better handle complex and ambiguous commands.

7.	Summary and Future Work
7.1 General Conclusions:
The ODSL-Jigsaw system shows significant promise in improving how documents are created by using natural language commands and program synthesis techniques. Even though our testing was internal, the system demonstrated that it could simplify and speed up the document creation process, making it more accessible to users who may not be comfortable with traditional tools.
7.2 Strengths and Limitations of the Solution:
•	Strengths:
o	User-Friendly: The system is easy to use, especially for routine tasks.
o	Accuracy: The system produces accurate documents in most cases.
o	Efficiency: The system reduces the time needed for document creation.
•	Limitations:
o	Ambiguity: The system sometimes has difficulty interpreting vague commands.
7.3 Possibilities for Expansion and Improvement:
•	Enhanced Language Support: We plan to expand the system to support additional languages and improve its handling of more complex tasks.
•	Formal User Testing: As the system improves, we may conduct formal user studies to gather more comprehensive feedback and further validate its effectiveness.
Final Thoughts
The ODSL-Jigsaw system represents a significant step forward in using natural language processing for document creation. While still in development, the system has shown that it can make the document creation process much easier, reducing the need for manual work and making advanced tools more accessible to a wider range of users. Our next steps will involve addressing the areas that need improvement and exploring the system's potential in more complex and diverse situations.


