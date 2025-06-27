# HospitalManagement
A hospital management app built with Django

# Full-Stack Hospital Management System (HMS)

This project is an advanced, full-stack Hospital Management System (HMS) architected with a powerful Django backend and a dynamic, responsive ReactJS frontend. It's designed to streamline hospital operations, from patient and doctor management to secure, cutting-edge payment processing.

The architecture emphasizes a decoupled design, where a robust Django REST API serves data to a sophisticated React Single-Page Application (SPA), ensuring scalability and a seamless user experience.

## Core Architectural Philosophy

This system is built on the principle of a clean separation of concerns:

* **Django REST Backend**: The backend is more than just a web application; it's a powerful API-first service built with the Django REST Framework. It handles all business logic, database interactions, user authentication, and serves as the single source of truth.
* **ReactJS Frontend**: The user interface is a modern SPA built with React. It communicates with the Django backend via RESTful API endpoints, providing a fast, interactive, and intuitive experience for patients and administrators without needing page reloads.

## Key Features & Technical Highlights

This project demonstrates expertise in a range of advanced development concepts:

* **Secure API Design**: The backend exposes a comprehensive suite of RESTful endpoints for managing patients, doctors, appointments, and insurance details.
* **Blockchain-Integrated Payments**: Moving beyond traditional payment gateways, the system features a payment module that records transactions on a blockchain. This provides an immutable, transparent, and highly secure ledger for all financial activities.
* **Two-Factor Authentication (2FA)**: User security is paramount. The patient signup and login flow is fortified with 2FA, requiring an authenticator app (like Google Authenticator) to protect sensitive patient data.
* **Asynchronous Task Processing**: Patient account approval and other long-running processes are handled by Celery with a Redis broker, preventing API blocking and ensuring a responsive system.
* **Component-Based UI**: The React frontend is built with reusable components, managing state efficiently to handle everything from user registration and data visualization to real-time appointment updates.

## Technology Stack

The technology choices reflect a modern, scalable, and secure application architecture.

| Category      | Technology                                         |
| :------------ | :------------------------------------------------- |
| **Backend** | Python, Django, Django REST Framework              |
| **Frontend** | ReactJS, HTML5, CSS3, Bootstrap                    |
| **Database** | PostgreSQL                                         |
| **Caching** | Redis                                              |
| **Async Tasks**| Celery & Redis                                     |
| **Security** | JWT Authentication, 2FA, CORS                      |
| **Blockchain**| Integration with an Ethereum-based smart contract for payments |

## Getting Started

To get the project up and running locally, you'll need to set up the backend and frontend separately.

### Backend Setup (Django)

```bash
# 1. Clone the repository
git clone [https://github.com/your-username/hms-project.git](https://github.com/your-username/hms-project.git)
cd hms-project

# 2. Set up and activate a virtual environment
python -m venv venv
source venv/bin/activate

# 3. Install backend dependencies
pip install -r requirements.txt

# 4. Run database migrations
python manage.py migrate

# 5. Start the Django development server
python manage.py runserver
# The API will be available at [http://127.0.0.1:8000](http://127.0.0.1:8000)
```

### Frontend Setup (React)

```bash
# 1. Navigate to the frontend directory
cd frontend

# 2. Install frontend dependencies
npm install

# 3. Start the React development server
npm start
# The application will be available at http://localhost:3000


## Dev Environment
Build an python 3.10 virtual environment using `conda`, `mamba`, or `venv`. Then run `pip install -r requirements.txt`.
