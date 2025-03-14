# Project Template for Developing Autotests Python+Pytest+Allure
This repository contains a project structure template for developing automated tests in Python. It includes a basic organization for API and UI testing, as well as necessary files for environment setup, such as requirements.txt and .gitignore.

## Project Structure
Here's how the project is organized:

```Bash
project/
├── python/
│   ├── api/ # Directory for API tests
│   │   ├── automation/
│   │   │   ├── src/ # Source code for API tests
│   │   │   ├── tests/ # API tests
│   │   │   ├── config/ # Configurations for API tests
│   │   │   ├── conftest.py # Fixtures for pytest
│   │   │   ├── pytest.ini # Configuration for pytest
│   │   │   └── tools/ # Helper tools
│   │   └── .gitignore # Ignored files and directories
│   ├── ui/ # Directory for UI tests
│   │   ├── automation/
│   │   │   ├── src/ # Source code for UI tests
│   │   │   │   └── base_page/ # Base classes for working with UI
│   │   │   ├── tests/ # UI tests
│   │   │   ├── config/ # Configurations for UI tests
│   │   │   ├── conftest.py # Fixtures for pytest
│   │   │   ├── pytest.ini # Configuration for pytest
│   │   │   └── tools/ # Helper tools
│   │   └── .gitignore # Ignored files and directories
│   ├── README.md # Project description
│   └── requirements.txt # Project dependencies
├── LICENSE # Project license
└── README.md # Main README file
```
## How to Use the Project
Choosing a Directory
Depending on the type of tests you're developing, choose the appropriate directory and copy its contents into your project:

- **API Tests** : Use the python/api directory.
- **UI Tests** : Use the python/ui directory.
### Virtual Environment
It is recommended to use a virtual environment (`venv`) to isolate project dependencies. To create and activate the virtual environment, run the following commands:

```bash
# Create a virtual environment
python -m venv .venv
bash
```
```bash
# Activate the virtual environment
# For Windows:
.venv\Scripts\activate
```
```bash
# For macOS/Linux:
source .venv/bin/activate
```
The virtual environment is created in the root directory of the project.

### Installing Dependencies
Before starting, install the required dependencies by running the command:

```bash
pip install -r requirements.txt
```
### Example Project Structure
If you chose the ui directory and copied it into your project named my-autotest-project, the structure will look like this:

```
my-autotest-project/
├── .venv/ 
├── automation/
│   ├── src/ 
│   │   └── base_page/ 
│   ├── tests/ 
│   ├── tools/ 
│   ├── config/ 
│   ├── pytest.ini 
│   └── conftest.py 
├── README.md 
├── requirements.txt 
└── .gitignore
```
### Notes:
- The `.venv` directory is created when activating the virtual environment and should not be committed to the repository (ensure it is added to .gitignore).
- You can adapt the structure to your needs by adding or removing directories and files.