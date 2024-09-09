# LangChain Chat with SQL DB

This Streamlit app allows users to interact with SQL databases using natural language queries. The app uses LangChain and ChatGroq to enable chat-based interactions with either a local SQLite database or a MySQL database.

## Features

- **Interactive Chat Interface**: Users can chat with the application to query the database.
- **Database Options**: Choose between a local SQLite database and a remote MySQL database.
- **GRoq API Integration**: Uses GRoq API with ChatGroq for natural language processing.

## Setup

### Prerequisites

- Python 3.8 or higher
- Streamlit
- LangChain
- SQLAlchemy
- sqlite3
- mysql-connector-python
- langchain_groq

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/your-repo.git
    cd your-repo
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Ensure you have your SQLite database file (`student.db`) in the correct location, or configure the MySQL database settings as needed.

### Configuration

1. Open `app.py` and set up your GRoq API key and database connection details in the sidebar.

2. For MySQL:
   - Provide the MySQL host, user, password, and database name in the sidebar.

3. For SQLite:
   - The app will automatically use `student.db` located in the same directory as `app.py`.

### Running the App

To start the Streamlit app, run:

```bash
streamlit run app.py
