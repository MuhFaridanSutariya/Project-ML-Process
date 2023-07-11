## How to run

### 1. Clone this repository
To get started, clone this repository onto your local machine. Follow the instructions below:

1. Open a terminal or Command Prompt.
2. Change to the directory where you want to clone the repository.
3. Enter the following command to clone the repository:
   ```bash
   git clone https://github.com/MuhFaridanSutariya/jakarta-pollution-classification.git
   ```
4. Once the cloning process is complete, navigate into the cloned directory using the `cd` command:
   ```bash
   cd jakarta-pollution-classification
   ```

### 2. System Requirements
Make sure your system meets the following requirements before proceeding:
- Python 3.10+ is installed on your computer.
- Pip (Python package installer) is installed.

### 3. Create a Virtual Environment
A virtual environment will allow you to separate this project from the global Python installation. Follow these steps to create a virtual environment:

**On Windows:**
Open Command Prompt and enter the following command:
```bash
python -m venv virtualenv_name
```
Replace `virtualenv_name` with the desired name for your virtual environment.

**On macOS and Linux:**
Open the terminal and enter the following command:
```bash
python3 -m venv virtualenv_name
```
Replace `virtualenv_name` with the desired name for your virtual environment.

### 4. Activate the Virtual Environment
After creating the virtual environment, you need to activate it before installing the requirements. Use the following steps:

**On Windows:**
In Command Prompt, enter the following command:
```bash
virtualenv_name\Scripts\activate.bat
```
Replace `virtualenv_name` with the name you provided in the previous step.

**On macOS and Linux:**
In the terminal, enter the following command:
```bash
source virtualenv_name/bin/activate.bat
```
Replace `virtualenv_name` with the name you provided in the previous step.

### 5. Install Requirements
Once the virtual environment is activated, you can install the project requirements from the `requirements.txt` file. Follow these steps:

**On Windows, macOS, and Linux:**
In the activated virtual environment, navigate to the directory where the `requirements.txt` file is located. Then, enter the following command:
```bash
pip install -r requirements.txt
```
This command will install all the required packages specified in the `requirements.txt` file

### 6. Run FAST API:

``uvicorn <replace-with-namafile>:app --reload``

This API provides a prediction endpoint for estimating pollution levels based on input features. It utilizes a trained machine learning model to make predictions.

The API server will start running locally at `http://localhost:8000`

### 7. API Endpoint:

`POST /predict`
Make a POST request to this endpoint to get pollution predictions.

<b>Request Body</b>
The request body should be a JSON object with the following fields:


