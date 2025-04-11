# Google Contacts Exporter using People API

This project allows you to extract Google Contacts using the Google People API and export them to both Excel and Google Sheets. It's perfect for personal backups, contact analysis, or CRM integrations — all powered via Python and Google Colab.

---

## 🚀 What This Project Does

- Authenticates securely via Google's OAuth2
- Extracts contacts with names, emails, and phone numbers using the People API
- Saves contacts to an Excel (.xlsx) file
- Optionally uploads the same data to a Google Sheet

---

## 📂 Files Included

- peoplecraft.ipynb — main Colab notebook to run everything
- requirements.txt — dependencies used in the project
- sample_client_secret.json — dummy filename (replace with your own actual credentials)

---

## 🛠️ Requirements

- A Google account
- Access to Google Cloud Console
- Python libraries:
  - pandas
  - google-auth
  - google-auth-oauthlib
  - google-api-python-client
  - openpyxl

---

## 🔐 How to Set Up

1. Visit the [Google Cloud Console](https://console.cloud.google.com)
2. Create a new project or choose an existing one
3. Navigate to: APIs & Services → Library → Enable "Google People API"
4. Go to: APIs & Services → Credentials → Create credentials → OAuth Client ID
   - Application type: Desktop App
   - Download the generated JSON file and rename it to: client_secret.json
5. Upload client_secret.json to your Google Colab environment
6. Add your Gmail ID under OAuth Consent Screen > Test Users in the Google Cloud Console

---

## ▶️ How to Run This Notebook

1. Open peoplecraft.ipynb in Google Colab
2. Upload your client_secret.json when prompted
3. Follow the auth link and paste your authorization code
4. Run the notebook to:
   - Extract and display your Google contacts
   - Save the data to an Excel file
   - Upload the data to a new Google Sheet (optional)

---

## 📈 Output Example

- contacts_export.xlsx (saved locally or downloadable from Colab)
- A new Google Sheet with all your contacts

You can add screenshots below to show what the output looks like:

![Sample Output Screenshot](path_to_your_screenshot.png)

---

## 🔒 Privacy Notice

- Your credentials are handled securely using Google’s OAuth flow
- The notebook does not store or transmit your data externally
- Be sure to exclude your actual client_secret.json from public uploads

.gitignore recommendation:
