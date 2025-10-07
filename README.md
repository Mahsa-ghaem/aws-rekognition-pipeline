AWS Rekognition Pipeline
Overview
This project demonstrates a serverless machine learning workflow built entirely on AWS. It uses Amazon S3, AWS Lambda, Amazon Rekognition, and DynamoDB to automatically analyze uploaded images and store the results in a structured database. The solution highlights my experience in Python-based cloud automation, AI integration, and data architecture design.

Architecture
Amazon S3 – Hosts the input bucket where users upload images.
AWS Lambda – Automatically triggered by S3 events; processes image metadata and invokes Rekognition.
Amazon Rekognition – Performs image analysis and object detection on the uploaded files.
DynamoDB – Stores analysis results such as detected objects, labels, and confidence scores.
(Optional) CloudWatch Logs – Monitors and logs the entire pipeline for debugging and performance tracking.

Key Features
Event-driven serverless architecture
Fully automated image analysis pipeline
Integration of AI service (Rekognition) with Lambda functions
DynamoDB persistence layer for structured results
Easily extendable for new ML use cases

Technologies Used
Languages & Tools: Python, Boto3, JSON
AWS Services: S3, Lambda, Rekognition, DynamoDB, CloudWatch
Infrastructure Concepts: Event-driven workflows, IAM Roles, Triggers, and Permissions
Version Control: Git, GitHub

How It Works
Upload an image to the S3 bucket.
S3 event triggers the Lambda function.
Lambda calls Rekognition API and receives analysis results.
Lambda writes results (labels, confidence levels, timestamps) to DynamoDB.
Logs and metrics can be viewed in CloudWatch.

Future Enhancements
Add REST API Gateway endpoint for remote image upload.
Integrate visualization dashboard using Power BI or Streamlit.
Extend model analysis to facial recognition or text detection.

Author
Dr. Mahsa Ghaempanah
Data Scientist & Software Engineer (Python, SQL, ML, Cloud/AWS)

