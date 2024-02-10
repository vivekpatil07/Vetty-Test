# Vetty Internship Assignment 

A Flask application that renders text files into HTML pages.

# Prerequisites

To run this project, the user should install Python 3, and optionally venv for a virtual running environment.

# Steps to Run

1. Download the project from GitHub and extract the zip folder:
   
You can do this manually by downloading the zip file from GitHub and extracting it to your desired location on your local machine.

3. Optionally, open the project in a virtual environment with venv:
   
Navigate to the project directory in your terminal and create a virtual environment:

     -- python3 -m venv venv

     Activate the virtual environment:
   
     On Windows:
     -- venv\Scripts\activate
   
     On macOS and Linux:
     -- source venv/bin/activate

5. Install requirements.txt using pip:
   
Make sure you're in the project directory and your virtual environment is activated. Then, install the requirements using pip:
-- pip install -r requirements.txt
   
7. Run app.py with Python 3:

Once the requirements are installed, you can run the Flask application using Python 3:
-- python app.py

# Files in project

app.py - Contains the Python code for running the flask application.

file1.txt - Sample text file for input to app.py.

file2.txt - Sample text file for input to app.py.

file3.txt - Sample text file for input to app.py.

file4.txt - Sample text file for input to app.py.

requirements.txt - Contains package and version requirements to run this project. Install with pip.

# Get Queries
With these modifications, the application now accepts three query parameters: file, begin, and end. If any of these parameters are not provided in the request, the default values will be used (file1.txt for file, None for begin, and None for end). The application will then read the specified file and return the content between the specified line numbers or the entire file if line numbers are not provided.

Example request: localhost:5001/?file=file2.txt&begin=4&end=6
