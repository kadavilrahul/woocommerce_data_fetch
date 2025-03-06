# WP Activity Log Data Fetcher

This script fetches data from the `wp_activity_log` table in a WordPress database.

## Prerequisites

-   Python 3.6+
-   `pip` (Python package installer)
-   MySQL Connector/Python
-   python-dotenv

## Installation

1.  **Install Python 3:**

    -   On Debian/Ubuntu: `sudo apt update && sudo apt install python3 python3-pip`
    
2.  **Create a virtual environment (recommended):**

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1.  **Create a `.env` file** in the same directory as the script.

2.  **Add the following environment variables** to the `.env` file:

    ```
    IP=your_database_ip
    DOMAIN=your_domain
    DATABASE_NAME=your_database_name
    DATABASE_USER=your_database_user
    DATABASE_PASSWORD=your_database_password
    DOMAIN_WHOLESALE=your_wholesale_domain
    ```

    Replace the placeholders with your actual database credentials.

## Usage

1.  **Run the script:**

    ```bash
    python3 wp_activity_log.py
    ```

## Troubleshooting

-   **"ModuleNotFoundError: No module named 'mysql.connector'"**: Make sure you have installed the `mysql-connector-python` package using `pip install mysql-connector-python`.
-   **"ModuleNotFoundError: No module named 'dotenv'"**: Make sure you have installed the `python-dotenv` package using `pip install python-dotenv`.
-   **"Access denied for user..."**: Double-check your database credentials in the `.env` file.
