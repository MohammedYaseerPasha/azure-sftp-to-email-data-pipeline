| Step | Component | Activity / Service Used | Description |
|-----|-----------|-------------------------|-------------|
| 1 | Source System | SFTP Server | The source system places the latest data file on the SFTP server. |
| 2 | Azure Data Factory | Get Metadata Activity | Checks the SFTP folder to detect whether the required file is available. |
| 3 | Azure Data Factory | Copy Activity | Copies the file from the SFTP server to Azure Blob Storage. |
| 4 | Azure Storage | Blob Container | The file is securely stored in Azure Blob Storage for further processing. |
| 5 | Azure Logic Apps | Blob Connector | Logic Apps retrieves the file from the Blob container. |
| 6 | Azure Logic Apps | Outlook Connector | Logic Apps sends the file as an email attachment to the required recipients. |
