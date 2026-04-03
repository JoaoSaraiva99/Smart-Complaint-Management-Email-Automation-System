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


# Recommendations

Based on the implementation and identified limitations, the following improvements are recommended:

* Fully integrate AI Builder outputs into the workflow to enable automated validation of invoice data (e.g., Issue Date filtering);
* Enhance data consistency by including all extracted invoice fields (especially Invoice Date) in the Excel database;
* Improve system robustness by adding error-handling mechanisms for missing or invalid attachments.
