# PeopleCraftAPI
Google Contacts Exporter using People API
This project helps you extract your Google Contacts using the Google People API and export them to Excel (.xlsx) and Google Sheets — all from a simple Python notebook using Google Colab.

🚀 What This Project Does
This notebook allows you to:

Authenticate securely with your Google account via OAuth2

Fetch contacts including names, phone numbers, and email addresses using the Google People API

Save the contact data to an Excel file (.xlsx)

Upload the same data to your Google Sheets (optional)

It’s perfect for anyone wanting a quick way to back up their contacts or analyze them for personal or business use.

📂 Files Included
peoplecraft.ipynb — the main Colab notebook

requirements.txt — list of Python dependencies

sample_client_secret.json — a dummy client secret file name you should replace with your actual one

🛠️ Requirements
A Google account

Access to Google Cloud Console to create credentials

Python libraries:

pandas

google-auth

google-auth-oauthlib

google-api-python-client

openpyxl

🔐 How to Set Up
Go to the Google Cloud Console: https://console.cloud.google.com

Create a new project (or select an existing one)

Go to APIs & Services > Library and enable the "Google People API"

Go to APIs & Services > Credentials and create a new "OAuth client ID" for Desktop App

Download the JSON file and rename it to client_secret.json

Upload this file to your Google Colab environment

📌 Important: Add your Google account as a "Test user" under OAuth Consent Screen settings to avoid authorization issues.

▶️ How to Run This Notebook
Open the notebook in Google Colab

Upload your client_secret.json when prompted

Authenticate using the link provided and paste the authorization code

Run the cells to:

Extract contacts

Save to Excel

Upload to Google Sheets (optional)

📈 Sample Output
Excel file saved as contacts_export.xlsx

Google Sheet created and populated with your contact data

(You can add screenshots here later if you'd like)

🔒 Privacy Notice
Your credentials are handled securely through Google’s OAuth2 flow.

No data is stored or sent anywhere outside your own account.

Be sure to exclude your real client_secret.json if you're pushing this project to a public GitHub repository.

Use this in .gitignore:

pgsql
Copy
Edit
client_secret.json
📘 Example Use Cases
Backing up personal or professional Google Contacts

Performing data analysis on your contact data

Integrating with CRM tools or other automation pipelines

💡 Bonus Features (Included)
Upload data directly to Google Sheets

Clean, readable output via Pandas

Modular design for easy reuse

📝 To-Do (Optional Enhancements)
Add UI using Streamlit or Gradio

Enable scheduled exports using Google Cloud Functions

Visualize contacts distribution by domain or location

📎 License
This project is licensed under the MIT License — feel free to use, modify, or build on top of it.
