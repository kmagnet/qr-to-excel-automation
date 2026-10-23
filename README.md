\# QR-to-Excel Automation



A working automation that allows users to scan a QR code, complete a Microsoft Form, and automatically save their responses to an Excel Online table.



\## How It Works



1\. A user scans the QR code using their phone.

2\. The QR code opens a Microsoft Form.

3\. The user completes and submits the form.

4\. Power Automate retrieves the submitted responses.

5\. Excel Online automatically receives a new row containing the submission details and a New Zealand timestamp.



\## Technologies Used



\- Microsoft Forms

\- Microsoft Power Automate

\- Excel Online (Business)

\- OneDrive for Business



\## Workflow



\*\*QR Code → Microsoft Forms → Power Automate → Excel Online\*\*



Power Automate uses three steps:



1\. \*\*When a new response is submitted\*\* — detects new form submissions.

2\. \*\*Get response details\*\* — retrieves the submitted form fields.

3\. \*\*Add a row into a table\*\* — saves the data to Excel.



\## Excel Output



| Submitted At | Name | Email | Request Type | Details |

|---|---|---|---|---|

| NZ date/time | Example User | example@example.com | General Inquiry | Sample request |



\## Testing



Successfully tested the complete workflow from a mobile QR code scan through to an automatically populated Excel row.



Verified that:



\- The QR code opens the form.

\- Form submissions trigger Power Automate.

\- Submitted fields are mapped to the correct Excel columns.

\- The submission timestamp is recorded in New Zealand local time.

\- New responses are added without manually editing the workbook.



\## Screenshots



Screenshots in the `screenshots` folder demonstrate the QR code, mobile form, Power Automate workflow, successful execution, and Excel results.



\## Deployment Notes



This demonstration was built in a Microsoft 365 educational environment. For a client deployment, the flow, form, workbook, and connections should be configured within the client's authorized Microsoft 365 environment.



Form-sharing permissions and connector availability depend on the organization's Microsoft 365 configuration.



\## Project Status



\*\*Completed — End-to-end workflow tested successfully.\*\*

