# Telegram Chat Dump Analyzer

A lightweight Google Colab tool to analyze Telegram chat history dumps (JSON). It automatically extracts questions, help requests, or other signals based on keywords and presents them in an interactive table.

Useful for **Community Managers**, **Support Teams**, and **Researchers** looking to filter noise and find user queries in large chat logs.

## 🚀 Features

*   **Offline Parsing:** Works with the standard JSON export from Telegram Desktop.
*   **Keyword Filtering:** Automatically detects messages containing words like "help", "question", "error" (customizable).
*   **Data Cleaning:** Handles Telegram's complex JSON structure (nested text entities).
*   **Interactive UI:** Provides instant filtering by User or Content directly in the notebook.
*   **Export Ready:** Data can be sent to Google Sheets for further analysis.

## 🛠 Prerequisites

1.  **Telegram Desktop:** To export chat history.
    *   Go to *Chat Settings* -> *Export Chat History*.
    *   Choose **JSON** format (Machine-readable).
2.  **Google Colab:** This notebook relies on Colab-specific widgets for file uploads and UI.

## 📥 How to Run

1.  Open the notebook in **Google Colab**.
2.  Run the cells sequentially.
3.  Click the **"Choose Files"** button and upload your `result.json` (Telegram export file).
4.  The script will parse the file and display a table with all found matches.
5.  Use the filter fields to drill down into specific users or topics.

## ⚙️ Configuration

KEYWORDS = [
"bug", "fail", "broken", "vulnerability" # Example for issue tracking
]


## 🔒 Privacy Note
Processing happens entirely within your Colab session. The uploaded JSON file is stored in the temporary runtime and deleted when the session ends. No data is sent to external servers.

## License
MIT



You can modify the `KEYWORDS` list in the "Configuration" cell to target specific topics:

# telegram_dumper
