# 🤖 Sonic: AI Chat Companion for Excel Data

[](https://www.google.com/search?q=https://%3Cyour_streamlit_app_url_here%3E) Sonic is an intelligent AI assistant built with [Streamlit](https://streamlit.io/) and [OpenAI's Assistant API](https://platform.openai.com/docs/assistants), designed to help you interact with and extract insights from your Excel files. Simply upload your spreadsheets, and Sonic will answer your questions, provide relevant information, and even generate various types of graphs based on your data.


-----

## ✨ Features

  - **Intelligent Chat:** Ask natural language questions about your Excel data and get accurate, context-aware answers powered by OpenAI.
  - **Excel Data Extraction:** Seamlessly reads and interprets data from `.xlsx` and `.xls` files using [Pandas](https://pandas.pydata.org/) and [Openpyxl](https://openpyxl.readthedocs.io/en/stable/).
  - **Dynamic Graph Generation:** Create a wide variety of interactive plots (Line, Bar, Scatter, Pie, Area, Histogram, Box, Bubble, Radar, Gantt) from your uploaded data with customizable options using [Plotly](https://plotly.com/).
  - **Theming:** Toggle between light and dark modes for a personalized user experience.
  - **Citation and Referencing:** Responses are accompanied by references to the specific files, sheets, or cells where the information was found.
  - **New Chat Functionality:** Easily clear the current conversation and start fresh.

-----

## 🚀 Getting Started

Follow these steps to get Sonic up and running on your local machine.

### Prerequisites

Before you begin, ensure you have the following installed:

  - **Python 3.8+** ([Download Python](https://www.python.org/downloads/))
  - **Pip** (Python package installer - usually comes with Python)
  - **Git** ([Download Git](https://git-scm.com/downloads))

### Installation

1.  **Clone the repository:**

    Open your terminal or command prompt and run:

    ```bash
    git clone (https://github.com/Kaizer321/Pdf_assistant/tree/main)
    cd Pdf_assistant
    ```

    Replace `<repository_url>` with the URL of this GitHub repository and `<repository_name>` with the name of the cloned directory.

2.  **Create a virtual environment (recommended):**

    Navigate to the project directory in your terminal and run:

    ```bash
    python -m venv venv
    source venv/bin/activate   # On macOS/Linux
    venv\Scripts\activate      # On Windows
    ```

3.  **Install the required packages:**

    Run the following command to install the necessary Python libraries:

    ```bash
    pip install -r requirements.txt
    ```

    If you don't have a `requirements.txt` file yet (if you're setting up a new project based on this README), create one with the following content and then run the `pip install` command:

    ```
    streamlit
    openai
    pandas
    openpyxl
    plotly
    python-docx
    ```

### OpenAI API Key Setup

This application uses the OpenAI Assistant API. You need to provide your OpenAI API key as a Streamlit secret for secure access.

1.  Create a folder named `.streamlit` in the root directory of your project.

2.  Inside the `.streamlit` folder, create a file named `secrets.toml`.

3.  Add your OpenAI API key to `secrets.toml` like this:

    ```toml
    OPENAI_API_KEY = "your_openai_api_key_here"
    ```

    Replace `"your_openai_api_key_here"` with your actual OpenAI API key from your [OpenAI Platform](https://platform.openai.com/).

### Running the Application

Once you have set up the API key and installed the dependencies, run the Streamlit application from your terminal within the project directory:

```bash
streamlit run main.py
```

This command will start the Streamlit server and automatically open the application in your default web browser.

-----

## 💡 How to Use

1.  **Upload Excel Files:** On the main page, you will find a section labeled "📊 Upload your Excel files". Click on the "Browse files" button and select one or more `.xlsx` or `.xls` files that you want to analyze. Sonic will process these files and initialize the AI assistant. You will see a success message upon completion.
2.  **Ask Questions:** Once your files are uploaded and the assistant is ready, a chat input box will appear at the bottom of the screen labeled "💬 Ask your question:". Type your question related to the data in the uploaded Excel files and press Enter or click the send button. Sonic will process your query and provide an answer.
3.  **Create Graphs:** In the sidebar on the left, you will find a button labeled **"Create Graph"**. Click this button to reveal options for generating charts. You can select the columns for the X and Y axes, choose from various chart types (Line, Bar, Scatter, Pie, etc.), and customize other plot parameters. The generated interactive graph will be displayed on the screen.
4.  **New Chat:** To start a new conversation and clear the previous chat history, click the **"New Chat"** button located in the sidebar.
5.  **Toggle Theme:** You can switch between light and dark visual themes by clicking the **"🌓 Dark"** (if in light mode) or **"🌞 Light"** (if in dark mode) button in the sidebar.

-----

## 📁 Project Structure

```
sonic-excel-ai/
├── .streamlit/
│   └── secrets.toml      # Stores your OpenAI API key
├── functions.py          # Contains the core logic and functions
├── main.py               # The main Streamlit application file
├── requirements.txt      # Lists the project dependencies
└── README.md             # This README file
```

-----

## 🛠️ Key Components and Technologies

  - **Streamlit:** An open-source Python library for creating beautiful, custom web apps for machine learning and data science.
  - **OpenAI Assistant API:** Leveraged for natural language understanding, information retrieval, and intelligent responses based on the uploaded Excel data.
  - **Pandas:** A powerful data analysis and manipulation library for Python, used here for reading and processing Excel data.
  - **Openpyxl:** A Python library to read and write Excel 2010+ `.xlsx` files.
  - **python-docx:** Used to convert Excel data into a `.docx` format temporarily for better processing by the OpenAI Assistant API.
  - **Plotly Express & Plotly Graph Objects:** Used for creating interactive and customizable data visualizations.
  - **Custom CSS:** Applied within the Streamlit app to enhance the user interface and provide theming options.

-----

##  Developed with ❤️ in SWAT, Khyber Pakhtunkhwa, Pakistan.

We are proud to contribute to the open-source community from Swat.

-----

## 🤝 Contributing

Contributions are welcome\! If you'd like to contribute to the development of Sonic, please follow these steps:

1.  Fork the repository on GitHub.
2.  Create a new branch for your feature or bug fix: `git checkout -b feature-name`
3.  Make your changes and commit them: `git commit -m 'Add new feature or fix bug'`
4.  Push your changes to your fork: `git push origin feature-name`
5.  Submit a pull request through the GitHub website.

-----

## 📄 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE)
