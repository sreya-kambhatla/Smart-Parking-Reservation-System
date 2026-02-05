# 🚗 PARK — Smart Parking Web Application

A full-stack web application built with Flask that helps users search, reserve, and manage parking spaces through a clean web interface with integrated payments and user management.

This project was developed as part of a Software Engineering project and demonstrates practical implementation of backend services, database models, UI templates, and payment workflows.

---

## 📌 Features

* User registration and account management
* Parking location search and processing
* Reservation and route handling
* Payment processing with Stripe integration
* Booking success and cancellation flows
* Database initialization and models
* Responsive UI with HTML, CSS, and JavaScript
* Test case documentation included

---

## 🏗️ Tech Stack

**Backend**

* Python
* Flask
* Flask-WTF
* SQLAlchemy (database models)
* Stripe API (payments)

**Frontend**

* HTML templates (Jinja2)
* CSS stylesheets
* JavaScript scripts

**Other**

* SQLite / relational DB (via Flask ORM)
* Webhooks for payment confirmation
* Form validation

---

## 📂 Project Structure

```
SE-Project-main/
│
├── PARK/
│   ├── static/
│   │   ├── css/
│   │   ├── images/
│   │   └── scripts/
│   │
│   ├── templates/
│   │   └── HTML templates
│   │
│   ├── Initialize Database.py
│   ├── create user model.py
│   ├── creat form.py
│   ├── payment.py
│   ├── location-processor.py
│   ├── webhook.py
│   ├── success route.py
│   ├── cancel route.py
│   └── flask app update files
│
├── Test Cases V1.md
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install flask flask-wtf sqlalchemy stripe
```

Add any additional packages used in your environment as needed.

---

## 🔐 Environment Configuration

Update your Stripe keys and secret values before running:

```python
stripe.api_key = "YOUR_SECRET_KEY"
```

Never commit real secret keys to version control. Use environment variables in production.

---

## 🗄️ Initialize the Database

Run the database initialization script:

```bash
python "Initialize Database.py"
```

This creates the required tables and schema.

---

## ▶️ Run the Application

```bash
python app.py
```

Then open your browser:

```
http://127.0.0.1:5000
```

---

## 💳 Payment Flow

The project integrates Stripe Checkout:

* Create checkout session endpoint
* Redirect to Stripe hosted payment page
* Webhook handler confirms payment
* Success and cancel routes handle outcomes

For local webhook testing:

```bash
stripe listen --forward-to localhost:5000/webhook
```

---

## 🧪 Testing

Functional test scenarios are documented in:

```
Test Cases V1.md
```

Includes:

* User registration tests
* Booking flow tests
* Payment success/cancel cases
* Route handling checks

---

## 🎯 Learning Goals Demonstrated

* Full-stack Flask development
* Modular route design
* Form handling and validation
* ORM data modeling
* Third-party API integration
* Payment workflow design
* Template-driven UI structure

---

## 📜 License

This project is for academic and educational use. Add a formal license if distributing publicly.

---

## 👥 Contributors

Add your team members here.

* Name — Role
* Name — Role

---
## 👤

Sreya Kambhatla<br>
Data Analyst | Business Analyst<br>
SQL • Python • Power BI • Analytics Engineering
