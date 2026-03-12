# Azure Automated Data Delivery Pipeline

## Overview
This project demonstrates an automated data pipeline built with Azure services that delivers hourly data updates from an SFTP server to stakeholders via email.

The solution eliminates manual intervention and ensures timely data delivery.

## Architecture

<img width="1536" height="1024" alt="architecture " src="https://github.com/user-attachments/assets/3f41b19b-c457-4849-85bd-db437ed94910" />


## Workflow

1. Data files are received from an SFTP server.
2. Azure Data Factory detects the files using the **Get Metadata** activity.
3. Files are transferred to **Azure Blob Storage** using **Copy Activity**.
4. Azure Logic Apps automatically retrieves the latest file.
5. The file is sent via **Outlook email** to stakeholders.

## Technologies Used

- Azure Data Factory
- Azure Blob Storage
- Azure Logic Apps
- SFTP
- Outlook Connector

## Key Features

- Automated hourly data pipeline
- Secure file transfer from SFTP
- Cloud storage integration
- Automated email delivery
- Scalable Azure architecture

## Use Cases

- Healthcare data delivery
- Financial reporting
- Automated file distribution
- Real-time analytics pipelines

## Learning Outcomes

- Building event-driven pipelines in Azure
- Automating workflows with Logic Apps
- Integrating SFTP with Azure services
- Designing scalable cloud data pipelines
