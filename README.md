Exception Logger
The Exception Logger is a Python package designed to simplify logging of exceptions in any application. It seamlessly integrates with your existing codebase to log errors and exceptions to a MySQL database, providing a centralized and structured approach to error tracking.

Features
Easy Integration: Integrate with your application without modifying the backend code.
Centralized Logging: Store all exceptions in a MySQL database for easy access and analysis.
Customizable: Configure the logger to suit your application's needs.
Simple Setup: Quick and straightforward setup process.
Installation
To install the package, use pip:

bash
Copy code
pip install exception-logger
Usage
Here's a basic example of how to use the Exception Logger in your application:

python
Copy code
from exception_logger import ExceptionLogger

# Initialize the logger with your MySQL credentials
logger = ExceptionLogger(
    db_host='localhost',
    db_user='root',
    db_password='Aayush187@',
    db_name='flask_logging_db'
)

# Use the logger to log exceptions
try:
    # Your code here
    pass
except Exception as e:
    logger.log_exception(e)
Configuration
The logger can be configured using the following parameters:

db_host: The hostname of your MySQL database.
db_user: The username to connect to your MySQL database.
db_password: The password to connect to your MySQL database.
db_name: The name of your MySQL database.
Contributing
We welcome contributions! If you would like to contribute, please fork the repository and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Issues
If you encounter any issues or have any questions, please open an issue on GitHub.

Feel free to customize this description to better suit your needs and provide more specific information about your project.
