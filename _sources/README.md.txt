# SEM3-Project

https://stayfinder4u.vercel.com/



\# StayFinder Documentation



\## project requirements 

Flask

flask-pymongo

flask-jwt-extended

flask-socketio

python-dotenv

cloudinary

authlib

bcrypt

firebase-admin

gunicorn

eventlet

flask-mail

razorpay

pymongo

reportlab



\## Project Overview

StayFinder is India's most trusted platform for finding hostels, PGs, and apartments. Zero brokerage, verified properties, and hassle-free booking.



\## Features

\- Search hostels by location

\- Search hostels by college (within 30km radius)

\- Property listing for owners

\- User authentication (students and owners)

\- Booking system

\- Email notifications



\## Technology Stack

\- \*\*Backend\*\*: Flask (Python)

\- \*\*Database\*\*: MongoDB Atlas

\- \*\*Frontend\*\*: HTML, CSS, JavaScript, Bootstrap

\- \*\*Authentication\*\*: JWT, Firebase (Google OAuth)

\- \*\*File Storage\*\*: Cloudinary

\- \*\*Email\*\*: Flask-Mail



\## Project Structure

```

stayfinder/

├── app.py                 # Main Flask application

├── config/

│   └── settings.py       # Configuration settings

├── utils/

│   └── database.py       # Database utilities

├── templates/            # HTML templates

│   ├── base.html         # Base template

│   ├── index.html        # Home page

│   ├── detail.html       # Property details

│   └── ...              # Other templates

├── static/

│   ├── css/              # Stylesheets

│   ├── js/               # JavaScript files

│   ├── images/           # Images and logos

│   └── uploads/          # User uploads

├── config/

│   └── colleges.json     # Colleges data

├── docs/                 # Documentation

├── requirements.txt      # Python dependencies

├── .env                 # Environment variables

└── vercel.json          # Deployment configuration

```



\## Installation

1\. Clone the repository

2\. Install dependencies: `pip install -r requirements.txt`

3\. Set up environment variables in `.env` file

4\. Run the application: `python app.py`



\## Environment Variables

\- `SECRET\_KEY`: Flask secret key

\- `JWT\_SECRET\_KEY`: JWT secret key

\- `MONGO\_URI`: MongoDB connection string

\- `MAIL\_SERVER`, `MAIL\_PORT`, etc.: Email configuration

\- `CLOUDINARY\_CLOUD\_NAME`, etc.: Cloudinary configuration

\- `GOOGLE\_CLIENT\_ID`, `GOOGLE\_CLIENT\_SECRET`: Google OAuth



\## API Endpoints

\- `GET /api/hostels` - Get all hostels

\- `POST /api/hostels/search` - Search hostels

\- `POST /api/hostels/search/college` - Search hostels by college

\- `GET /api/colleges` - Get all colleges

\- `POST /api/bookings/request` - Submit booking request



\## Deployment

The application is configured for deployment on Vercel using the `vercel.json` configuration file.



