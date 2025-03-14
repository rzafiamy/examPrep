# PrepareExam

A Flask-based web application to help users prepare for various certification exams by providing 1,000,000+ QCMs (Multiple Choice Questions). It supports user authentication, scoring, and certification-based exam attempts.

## Tech Stack

- Backend: Flask (Python)
- Frontend: JavaScript (Vanilla JS), Tailwind CSS
- Database: PostgreSQL
- Authentication: Flask-Login
- API: Flask-RESTful
- Deployment: Docker + Gunicorn + Nginx

---

## Features

### User Features

✔️ Sign Up / Login / Logout
✔️ Take timed QCMs for different certifications
✔️ Track scores and history of attempts
✔️ View past incorrect answers
✔️ Responsive UI with Tailwind CSS

### Admin Features

✔️ Secure login for admins
✔️ Add / Update / Delete QCMs
✔️ Manage certifications
✔️ View users' performance & statistics


---

## Installation

1️⃣ Clone the Repository

git clone https://github.com/yourusername/prepareExam.git
cd prepareExam

2️⃣ Create Virtual Environment

python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Setup Environment Variables

Create a .env file in the root directory and add:

FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_secret_key
DATABASE_URL=postgresql://your_db_user:your_db_password@localhost/prepareexam

5️⃣ Initialize Database

flask db init
flask db migrate -m "Initial migration"
flask db upgrade

6️⃣ Run the Application

flask run

Access the app at: http://127.0.0.1:5000


---

## Project Structure

```bash
/prepareExam
│── /app
│   │── models.py        # Database Models
│   │── routes.py        # API Endpoints
│   │── auth.py          # User Authentication
│   │── admin.py         # Admin Panel
│   │── templates/       # Jinja2 HTML Templates
│   │── static/          # Tailwind CSS & JavaScript
│   │── utils.py         # Utility functions
│── config.py            # Configuration settings
│── app.py               # Flask Entry Point
│── requirements.txt     # Python Dependencies
│── Dockerfile           # Containerization
│── README.md            # Project Documentation
```

---

## API Endpoints


---

## Tailwind CSS Setup

If you plan to customize Tailwind CSS:

1. Install Tailwind CSS

npm install -D tailwindcss
npx tailwindcss init


2. Configure tailwind.config.js


3. Use Tailwind classes in templates like:

<button class="bg-blue-500 text-white px-4 py-2 rounded">Start Exam</button>




---

## Deployment

Using Docker

1. Build the Image

docker build -t prepareexam .


2. Run the Container

docker run -p 5000:5000 prepareexam



Using Gunicorn & Nginx

Set up Gunicorn to serve the app

Use Nginx as a reverse proxy

Configure PostgreSQL in production mode



---

## Contributing

✔ Fork the repository
✔ Create a feature branch
✔ Submit a pull request


---

## License

This project is licensed under the MIT License.


---

## Next Steps

[ ] Implement the Admin Dashboard

[ ] Improve QCM scoring system

[ ] Add User progress tracking



---

This README provides a structured guide for development. Let me know if you need modifications! 🚀

