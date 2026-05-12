# IR_Project

An Information Retrieval system with a web-based interface for searching, indexing, and retrieving information efficiently.

## Overview

This project implements a comprehensive Information Retrieval system combining Python backend logic with an HTML-based frontend. It provides tools for indexing documents, performing searches, and ranking results based on relevance.

## Tech Stack

- **Backend**: Python 
- **Frontend**: HTML

## Features

- Document indexing and storage
- Full-text search capabilities
- Relevance ranking and scoring
- Web-based user interface
- Fast query processing

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
