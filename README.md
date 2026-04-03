# Smart Complaint Management Email Automation System
# ProjectBackground
Customer support teams often face high volumes of repetitive email requests, including information inquiries and invoice-related complaints. These processes are typically manual, time-consuming, and prone to human error, leading to inefficiencies and inconsistent service quality.

This project was developed to address these challenges by leveraging automation and AI-powered classification to streamline the handling of customer emails. The solution integrates tools such as AI Builder, Power Automate, Excel, and OneDrive to create a structured, scalable workflow.

As shown in the workflow diagram, the system automates the full lifecycle of a request—from email reception to classification, validation, task creation, and resolution, ensuring improved operational efficiency and service consistency.

<img width="1920" height="1080" alt="Modern Pitch Deck Presentation Template" src="https://github.com/user-attachments/assets/96f96aa7-25e0-49f7-8abf-4595e4d2d5db" />

# ExecutiveSummary

This project presents an end-to-end automated workflow designed to manage customer support emails, specifically focusing on information requests and invoice complaints.

The system is triggered whenever a new email is received and uses Natural Language Processing (NLP) to classify the request type, detect sentiment, identify urgency, extract key data (e.g., TIN), and generate a structured summary.

Key functionalities include:

* Automated email classification (Request Type, Sentiment, Language, Urgency);
* Intelligent request summarization for operator support;
* Automatic storage and processing of invoice attachments;
* Validation rules for complaints (e.g., invoice within 12 months);
* Integration with Excel for structured data logging;
* Task creation for operational tracking;
* Urgency-based alerts via Microsoft Teams;
* Approval workflow with customer feedback loop (including satisfaction survey).

The solution significantly reduces operational workload, minimizes human error, and accelerates response times, ultimately improving customer satisfaction

<img width="488" height="460" alt="imagem" src="https://github.com/user-attachments/assets/cdd3e977-865c-4353-9dfc-06d7fc730bc9" />

<img width="580" height="456" alt="imagem" src="https://github.com/user-attachments/assets/709dac8d-fe4d-43cf-a879-0381a6cdb3e1" />

## Mail Classification
Prompt used:
You are a natural language processing assistant. Your task is to analyze the text of a received email and identify the following information:
Request Type Classification: Determine whether the email is an **"Information Request"** or a **"Complaint"**.

Use the following criteria:
* If the text contains questions, requests for details, or explanations, classify it as an "Information Request".
* If the text contains dissatisfaction, criticism, reported issues, or complaints, classify it as a "Complaint".

Sentiment Analysis:
Classify the overall sentiment of the email as **"Positive"**, **"Negative"**, or **"Neutral"**.
* Positive: The text shows satisfaction, gratitude, or praise.
* Negative: The text shows dissatisfaction, frustration, or complaints.
* Neutral: The text has no clear emotions or uses objective language.

Language Identification: Identify the language in which the email was written. Return the language in ISO 639-1 format (e.g., "pt" for Portuguese, "en" for English, "es" for Spanish).

Tax Identification Number (TIN) Identification: Search for the Tax Identification Number in the email text.
* If found, return the identified number.
* If not found, set it as "N/A".

Urgency: Yes or No: Determine whether the email indicates urgency.
 Use the following criteria:
If the text contains words such as "urgent", "immediate", "priority", or mentions tight deadlines, set it as "Yes".
Otherwise, set it as "No".

Input:

Expected Output: the following fields in the format:
* RequestType: "Information Request" or "Complaint".
* Sentiment: "Positive", "Negative", or "Neutral".
* Language: ISO 639-1 code of the identified language and the language name in European Portuguese.
* TIN: Identified number or "N/A" if not found.
* Urgent: "Yes" or "No".

# Recommendations

Based on the implementation and identified limitations, the following improvements are recommended:

* Fully integrate AI Builder outputs into the workflow to enable automated validation of invoice data (e.g., Issue Date filtering);
* Enhance data consistency by including all extracted invoice fields (especially Invoice Date) in the Excel database;
* Improve system robustness by adding error-handling mechanisms for missing or invalid attachments.

# Additional Resources  

You can consult the full project presentation here:  

🔗 [Project Presentation PDF](https://github.com/JoaoSaraiva99/Smart-Complaint-Management-Email-Automation-System/blob/main/Modern%20Pitch%20Deck%20Presentation%20Template-3.pdf)

