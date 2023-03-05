# googlesheet_db


## Usecase
We faced a lot of challenging situation when we share the file output between tech and non-tech team. As a workaround, this minimum value script create Google sheet workbook and sheet from pandas data frame.
Edit data_controller.py for data collection logic, and pass it to googlesheet_db.py.

## Set up
create config.yml

API_SCOPE:
  - 'https://www.googleapis.com/auth/drive'
  - 'https://www.googleapis.com/auth/spreadsheets'
PATH_TO_JSON: '/path/to/googlesheet_key.json'
WORKBOOK_NAME: 'xxxx'
SHEET_NAME: 'xxxx'
EMAIL: 'xxxxx@xx.com'
