# 🌱 AgriAssist — Smart Agriculture Assistant

AgriAssist is a smart agriculture assistance web application that combines Machine Learning, agricultural market price data, and an AI-powered chatbot to help farmers explore data-driven farming decisions.

## 🚀 Features

- **Crop Recommendation:** Recommends suitable crops based on agricultural input conditions.
- **Crop Price Prediction:** Estimates crop prices using machine learning models and market price data.
- **AI Agriculture Chatbot:** Provides answers to agriculture-related questions through an interactive chatbot.
- **Government Market Price Integration:** Fetches agricultural market price information using the Government of India's Data.gov.in API.
- **MySQL Database:** Stores and manages application data.
- **Prediction History:** Allows users to view previous predictions.
- **Multilingual Interface:** Supports English, Hindi, and Marathi.
- **Web Dashboard:** User-friendly interface developed using HTML, CSS, and JavaScript.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Backend:** Flask, Flask-CORS
- **Frontend:** HTML5, CSS3, JavaScript
- **Machine Learning:** Scikit-learn
- **Database:** MySQL
- **APIs:** REST APIs, Data.gov.in Agricultural Market Price API
- **AI Integration:** Google Gemini API
- **Version Control:** Git and GitHub
- **Deployment & DevOps:** Docker, Jenkins, Kubernetes, and AWS

## 📁 Project Structure

```text
AgriAssist/
│
├── backend/
│   ├── app.py
│   ├── ml_models.py
│   ├── market_prices_api.py
│   ├── requirements.txt
│   └── README.md
│
├── database/
│   ├── database.sql
│   └── README.md
│
├── datasets/
│   ├── Crop_recommendation.csv
│   ├── crop_production_data.csv
│   ├── soil_analysis_data.csv
│   ├── water_usage_data.csv
│   └── README.md
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   └── README.md
│
├── tests/
│   ├── test_data_gov_api_fixed.py
│   └── README.md
│
├── .gitignore
└── README.md
```

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/vedant-mahajan111/AgriAssist.git
cd AgriAssist
```

### 2. Install Backend Dependencies

```bash
pip install -r backend/requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file in the appropriate backend directory and configure the required environment variables, such as:

- Gemini API key
- MySQL database name
- MySQL username
- MySQL password
- Database host

**Security:** Never upload `.env` files, API keys, passwords, or other sensitive credentials to GitHub.

### 4. Configure the MySQL Database

Make sure MySQL Server is installed and running.

Execute the SQL script:

```bash
mysql -u root -p < database/database.sql
```

Ensure that the database configuration in the backend matches your MySQL settings.

### 5. Start the Backend

Navigate to the backend directory:

```bash
cd backend
```

Run the Flask application:

```bash
python app.py
```

The backend will start on the configured local address and port.

### 6. Start the Frontend

- Open the `frontend` folder in Visual Studio Code.
- Launch `index.html` using the Live Server extension.
- Ensure that the frontend API URL matches the running Flask backend address.

## 🌾 Government Agricultural Market Data

AgriAssist integrates with the Government of India's Data.gov.in API to retrieve agricultural market price records.

Depending on API availability, the data may include:

- Commodity name
- State and district
- Market or mandi
- Arrival date
- Minimum price
- Maximum price
- Modal price

The availability and accuracy of market records depend on the external API.

## ☁️ DevOps and Deployment

The project also incorporates DevOps practices to automate application deployment.

**Technologies used:**

- **AWS EC2:** Hosts the application environment.
- **Docker:** Packages the application into containers.
- **Docker Hub:** Stores Docker images.
- **Jenkins:** Automates the CI/CD pipeline.
- **Kubernetes:** Manages application deployment and containers.

The CI/CD pipeline automates the process of checking out source code, building Docker images, pushing images to Docker Hub, and deploying updated application versions to Kubernetes.

## 🎯 Project Purpose

AgriAssist is an educational project that demonstrates the integration of machine learning, web development, database management, public agricultural data, and DevOps technologies to develop a smart agriculture assistance platform.

## 👨‍💻 Author

**Vedant Mahajan**

GitHub: [@vedant-mahajan111](https://github.com/vedant-mahajan111)

**Project Repository:** [AgriAssist](https://github.com/vedant-mahajan111/AgriAssist)
---

If you find this project interesting, feel free to explore the repository and its individual components.
