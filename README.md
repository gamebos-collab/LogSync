# LogSync Project

## Project Structure

```
LogSync/
├── src/               # Source files for the application
│   ├── main.py       # Main application entry point
│   ├── utils/        # Utility functions
│   └── models/       # Database models
├── tests/            # Test files
├── .env              # Environment configuration
├── requirements.txt   # Python dependencies
└── README.md         # Project documentation
```

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/gamebos-collab/LogSync.git
   cd LogSync
   ```
   
2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the database**
   - Ensure you have the appropriate database installed (e.g., PostgreSQL, MySQL).
   - Configure the connection details in the `.env` file as follows:
     ```
     DB_HOST=localhost
     DB_PORT=5432
     DB_NAME=logsync_db
     DB_USER=your_username
     DB_PASSWORD=your_password
     ```

5. **Run the application**
   ```bash
   python src/main.py
   ```

## Database Configuration

Ensure that the database you are using has the following configuration:
- Host: `localhost`
- Port: `5432` (PostgreSQL) or appropriate port for your DBMS
- Database Name: `logsync_db`
- Username: your database username
- Password: your database password

After setting up the database, you may need to run migrations or initialize the database schema based on the models defined in `src/models/`.

---

For more information, refer to the documentation provided in each module and the source files.