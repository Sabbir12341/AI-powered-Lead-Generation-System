# Instagram AI Agent for Lead Generation

An automated **n8n workflow** that finds targeted Instagram profiles and leads using Google Search. Perfect for marketers, agencies, and businesses looking to generate high-quality Instagram leads at scale.

---

## ✨ Overview

This workflow allows users to submit search keywords and a location through a clean web form. It then automatically:
- Searches Google for Instagram profiles matching the criteria
- Extracts relevant lead data
- Saves everything directly into a Google Spreadsheet

Built with **n8n** — a powerful workflow automation tool.

---

## 🚀 Features

- **Simple Web Form** – User-friendly input interface
- **Smart Google Search** – Uses `site:instagram.com` operator for precise results
- **Automated Data Extraction** – Title, Profile URL, Description, and Position
- **Google Sheets Integration** – Leads saved automatically
- **Scalable & Reusable** – Easy to modify for different platforms

---

## 📋 How It Works

1. User submits the form with **keywords** and **location**
2. Workflow sends request to **Apify Google Search Scraper**
3. Results are split and cleaned using JavaScript
4. Clean leads are appended to Google Sheets

---

## 🛠️ Prerequisites

Before importing this workflow, make sure you have:

- **n8n** (self-hosted or cloud)
- **Apify Account** – Get your API token from [apify.com](https://apify.com)
- **Google Sheets Account** – OAuth2 credentials in n8n
- A Google Sheet with columns: `Title`, `Profile URL`, `Description`, `Position`

---

## 📥 Installation & Setup

1. Download the workflow file: `My workflow 2.json`
2. In n8n, go to **Workflows** → **Import from File**
3. Import the downloaded JSON file
4. Configure credentials:
   - **Apify API Token** in the HTTP Request node
   - **Google Sheets OAuth2** credentials
5. Update the Google Sheet Document ID if needed
6. Activate the workflow

---

## 📝 Usage

1. Open the workflow and click **"Execute Workflow"** or use the **Form Trigger** URL
2. Fill the form:
   - **What are you looking for?** → e.g., `fitness coach`, `digital marketing`, `restaurant`
   - **Location** → e.g., `Bangladesh`, `New York`, `worldwide`
3. Submit → Leads will automatically appear in your Google Sheet

---

## 🔧 Technologies Used

- **n8n** – Workflow automation
- **Apify Google Search Scraper**
- **Google Sheets API**
- **JavaScript Code Node**

---

## 📸 Screenshots

*(Add screenshots of your form and Google Sheet here)*

---

## ⚡ Future Improvements

- Add Instagram direct scraping (using Apify Instagram actors)
- Email notification when leads are generated
- Lead enrichment with contact info
- Multi-platform support (TikTok, LinkedIn, Facebook)

---

## 📄 License

This project is open-source and available under the **MIT License**.

---

## 🤝 Contributing

Feel free to fork this repository and submit pull requests. Any improvements or new features are welcome!

---

**Made with ❤️ using n8n**

---

*If you found this workflow useful, please give it a ⭐ on GitHub!*
