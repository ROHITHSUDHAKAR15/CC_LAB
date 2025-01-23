# CC_Monolith

## Overview
CC_Monolith is a modular application consisting of various components like authentication, cart management, product handling, and checkout. It includes scripts for database operations and performance testing.

## Directory Structure
```
CC_Monolith/
|-- auth/                # Authentication-related files
|-- cart/                # Cart management files
|-- checkout/            # Checkout process logic
|-- insert_product.py    # Script to insert products into the database
|-- locust/              # Load testing setup using Locust
|-- main.py              # Main entry point of the application
|-- products/            # Product management files
|-- requirements.txt     # Python dependencies
|-- templates/           # HTML templates for the application
```

## Prerequisites

- Python 3.8 or later
- A virtual environment (recommended)
- SQLite or other supported database systems
- Locust (for performance testing)
- Verv (if applicable for API validation and testing)

## Installation

1. Clone the repository or extract the zip file.
   ```bash
   git clone <repository_url>
   cd CC_Monolith
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the database:
   ```bash
   python insert_product.py
   ```

## How to Execute

1. Start the application:
   ```bash
   python main.py
   ```

2. Access the application in your browser at:
   ```
   http://127.0.0.1:5000
   ```

3. To run load tests using Locust:
   ```bash
   locust -f locust/<locust_file.py>
   ```
   Open Locust's web interface at `http://127.0.0.1:8089`.

4. If Verv is required for API validation, configure it according to your project and execute the relevant scripts.

## Tools Required

- Python (3.8 or later)
- Flask (for the web application framework)
- SQLite (or an alternative database system)
- Locust (for load testing)
- Verv (for API validation and testing)
- Any web browser (for accessing the application)

## Notes

- Ensure all dependencies are installed before running the application.
- Modify the configuration files as needed for your specific environment.
- Test Locust scripts to evaluate application performance under different load conditions.
- Utilize Verv for API testing if applicable to your workflow.



