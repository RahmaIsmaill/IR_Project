# IR_Project

An Information Retrieval system with a web-based interface for searching, indexing, and retrieving information efficiently.

## Overview

This project implements a comprehensive Information Retrieval system combining Python backend logic with an HTML-based frontend. It provides tools for indexing documents, performing searches, and ranking results based on relevance.

## Tech Stack

- **Backend**: Python 
- **Frontend**: HTML

## Project Structure

```bash
IR_Project/
├── backend/                     # Python backend
│   ├── main.py                  # Main application file
│   ├── requirements.txt         # Python dependencies
│   └── __pycache__/             # Compiled Python files
│
├── frontend/                    # Frontend files
│   └── index.html               # Main frontend page
│
├── data/                    # Dataset files (indexed documents)
│   ├── *.json
│   ├── *.csv
│   ├── *.txt
│   ├── *.pdf
│   ├── *.xlsx
│
├── README.md                    # Project documentation
└── docker-compose.yml           # Docker configuration
```

 Features

 Indexing  
Supports multiple file formats: JSON, CSV, TXT, PDF, Excel (.xlsx).  
Each file is parsed into searchable documents.  
Rebuild or reindex data anytime.

 Search Engine Features  
Supports advanced search capabilities:
- Boolean search: AND, OR, NOT  
- Phrase search: "exact phrase"  
- Wildcard search: term*  
- Fuzzy search: retrival~  
- Multi-field search (name, description, content)  
- Highlighted search results  
- Pagination (5 results per page)

 Filters  
Users can filter results by:
- Category  
- File type  
- Price range  
- Date range (modification date)

 Did You Mean?  
Automatic suggestion when no results are found.  
Uses Elasticsearch term suggestions.

 Statistics Dashboard  
The system provides analytics including:
- Total indexed documents  
- Breakdown by file type  
- Breakdown by category  
- Top 10 most frequent terms  

 Data Processing Strategy  
Each file type is converted into searchable documents as follows:
- JSON → each object is treated as a document  
- CSV → each row is treated as a document  
- TXT → each file is treated as one document  
- PDF → extracted text per file  
- XLSX → each row in each sheet is indexed as a document  

 Search Syntax Guide  

- AND → phone AND samsung  
- OR → apple OR samsung  
- NOT → NOT refurbished  
- Phrase → "wireless headphones"  
- Wildcard → iph*  
- Fuzzy → retrival~
## Getting Started

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/RahmaIsmaill/IR_Project.git
   cd IR_Project
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python app.py
   ```

4. Open your browser and navigate to `http://localhost:5000`

## Usage

1. **Index Documents**: Upload or index your document collection
2. **Search**: Enter queries in the search interface
3. **View Results**: Browse ranked results with relevance 
