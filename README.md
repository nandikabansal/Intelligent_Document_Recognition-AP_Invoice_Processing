# Intelligent_Document_Recognition-AP_Invoice_Processing
A Python-based automation tool that extracts invoice details from PDFs, saves them to an Excel file, and archives processed files in Google Drive.

📌 Features
 -Reads invoice pdf files from a designated directory in google drive</br>
 -Parses invoice details with Gemini AI</br>
 -Extracts text from invoices using PyMuPDF</br>
 -Saves extracted data to Excel appending to the existing records</br>
 -Moves processed invoices to a designated archive folder in Google Drive</br>

🛠 Setup & Installation
-Setup google cloud workspace. Create project and enable OAuth APIs for connection with gmail and google drive for personal accounts. Refer to https://support.google.com/googleapi/answer/6158849?hl=en for details</br>
-Setup account on make.com to automate the process of saving invoice attatchments automatically to Google drive. (optional)</br>
-Clone the repository and navigate to it. </br>
-Download the OAuth Client JSON file and save it as client_secrets.json in the same directory as final.py
-Run the following to install dependencies. 
```sh
pip install -r requirements.txt
```
-Add your unique gemini API key in the final.py code under main.
-Provide your INVOICE_FOLDER_ID which is the id of the google drive folder where invoices are stored. 
-Provide your ARCHIVE_FOLDER_ID which is the id of the google drive folder where invoices should be saved after processing is complete. 
