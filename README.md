# webscrap
# Web Scraping Loan Service Providers using BeautifulSoup

This project is a web scraping script that extracts details of loan service providers from the Indian Yellow Pages website using Python, the requests library, and BeautifulSoup for parsing HTML. The extracted data is then stored in an Excel file using the pandas library.

*Input :-*

The script prompts the user to enter the name of a city.
It dynamically constructs the URL to scrape loan service provider data from the Indian Yellow Pages website for the specified city.
*Output :-*

If the request is successful(HTTP Status Code= 200), the script extracts the following details for each listed loan service provider:
Title (Company Name), Link (Company Profile URL), Address, Rating.

The extracted data is saved in an Excel file named loan_service_providers_.xlsx

If the request fails, an error message with the HTTP status code is displayed.(e.g. 403)

*Target Website :-* https://www.indianyellowpages.com/

How to Run the Script

Install the required Python libraries:

pip install requests beautifulsoup4 pandas

Run the script:

python script.py

Enter the desired city name when prompted.

The extracted data will be saved in an Excel file in the same directory as the script.
Enter the city name: Mumbai
Data saved to loan_service_providers_Mumbai.xlsx



bash 
```
/multi_agent_system
|
├── 📂 agents/                # Directory for all specialized agents
│   ├── __init__.py         # Makes the folder a Python package
│   ├── arxiv_agent.py      # Logic for the ArXiv search agent
│   ├── pdf_rag_agent.py    # Logic for the PDF RAG agent
│   └── web_search_agent.py   # Logic for the web search agent
|
├── 📂 domain_pdfs/           # Contains sample PDFs for testing
│   └── ...
|
├── 📂 logs/                  # Stores logs from the system
│   └── controller_log.jsonl # Logs every decision made by the Controller
|
├── 📂 uploads/               # Temporary storage for user-uploaded PDFs
│   └── ...
|
├── 📂 vector_store/          # Caches the FAISS vector embeddings for PDFs
│   └── ...
|
├── 📜 .env                   # Stores secret environment variables (API keys)
├── 📜 .gitignore             # Specifies files for Git to ignore (e.g., myenv/, __pycache__/)
├── 📜 README.md              # Project documentation
├── 📜 app.py                 # The Streamlit frontend application
├── 📜 controller.py           # The Controller Agent logic (the "brain")
├── 📜 main.py                # The FastAPI backend server
├── 📜 requirements.txt        # Lists all Python package dependencies
└── 📜 utils.py               # Helper functions, like the answer synthesizer

```
