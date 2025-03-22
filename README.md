📝 Flask Job Application Form

🌐 Overview

This is a Flask-based web application that allows users to fill out a job application form. Submitted data is stored in a local SQLite database, and users receive a confirmation email upon successful submission.

📌 Features

Collects user input: first name, last name, email, availability date, and current occupation

Stores form submissions in a local SQLite database

Sends confirmation email to the applicant using Flask-Mail

Displays success message using Flask flash messaging

Responsive UI with Bootstrap 5

🛠 Technologies Used

Python 3

Flask

Flask-Mail

Flask-SQLAlchemy

SQLite

Bootstrap 5 (via CDN)

dotenv for environment variables

🚀 Installation & Setup

1. Clone the Repository

git clone [CLICK](https://github.com/PolytechnicCoder/flask_form_app/tree/master)

2. Create a Virtual Environment

python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

3. Install Dependencies

pip install -r requirements.txt

4. Set Environment Variables

Create a .env file in the root directory with the following content:

KEY=your_secret_key
USERNAME_EMAIL=your_email@gmail.com
PASSWORD_EMAIL=your_app_password

⚠️ For Gmail, make sure you use an App Password if 2FA is enabled.

5. Run the Application

python app.py

App will be available at http://localhost:5001/

📂 Project Structure

├── app.py                # Main Flask application
├── data.db               # SQLite database file (auto-generated)
├── templates/
│   └── index.html        # Job application form UI
├── .env                  # Environment variables (not tracked by Git)
├── requirements.txt      # Python dependencies

📧 Email Functionality

Emails are sent using the Gmail SMTP server via Flask-Mail.

Email contains a confirmation message and summary of submitted data.

🛡️ Security Notes

Never upload .env or real credentials to version control

Use .gitignore to exclude data.db, .env, and __pycache__ files

🖼️ Screenshot Placeholder

![flask_app](https://github.com/user-attachments/assets/c522178f-23d1-48ab-b9af-62c8d4e1c02d)


📝 Flask Job Form App – Built with Flask, SQLite & Email Integration
