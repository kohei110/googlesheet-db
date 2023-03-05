# googlesheet_db

## Disclamer 
Using Google Sheets as a database can have some risks and limitations. Here are a few potential risks to consider:

Security: Google Sheets is hosted on the cloud, which means that your data is stored on Google's servers. While Google is a reputable company that takes security seriously, storing sensitive data in Google Sheets can still pose a risk. If the sheet is not properly secured with appropriate access controls, unauthorized users may be able to access and manipulate the data.

Data loss: Google Sheets is an online tool, which means that it relies on an internet connection to work. If your internet connection is lost or the Google Sheets server experiences downtime, you may not be able to access your data. Additionally, accidental deletion or data corruption can also result in the loss of data.

Limited functionality: While Google Sheets can be used as a simple database, it may not have all the functionality required for more complex applications. For example, it may be difficult to implement advanced querying, data validation, or relationships between tables.

Scalability: Google Sheets may not be suitable for large-scale applications that require high levels of data processing or storage. As the size of the data grows, the performance of the sheet may suffer, and it may become difficult to manage.

Legal and compliance issues: Depending on the type of data you are storing in Google Sheets, you may be subject to legal and compliance requirements. For example, if you are storing personal information, you may need to comply with data protection regulations such as GDPR or CCPA.


## Background
We faced a lot of challenging situation when we create accessible db between tech and non-tech team. As a workaround, this minimum value script create Google sheet workbook and sheet from pandas data frame, and non-tech team can access this as a db. Edit data_controller.py for data collection logic, and pass it to googlesheet_db.py.

## Set up
create config.yml

- API_SCOPE:
  - 'https://www.googleapis.com/auth/drive'
  - 'https://www.googleapis.com/auth/spreadsheets'
- PATH_TO_JSON: '/path/to/googlesheet_key.json'
- WORKBOOK_NAME: 'xxxx'
- SHEET_NAME: 'xxxx'
- EMAIL: 'xxxxx@xx.com'

## Use-case
example: Create data collection script and setup cron file to collect and update data regularly for the team doesn't have enough engineer support. They just access to google sheet and copy and paste for their usage. Adding weekly stats report, visualisation etc. will be useful?
