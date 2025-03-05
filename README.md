
# CropYieldPredictor-Ethiopia

- A Flask and FastAPI-based web application to predict crop yields for Ethiopian farmers using rainfall, pesticide use, and available climate data and machine learning. Empowering small-scale farmers with data-driven insights for better agricultural outcomes.
- AI-powered crop yield prediction platform for Ethiopian farmers, integrating climate data, machine learning, and accessible web tools.
- An open-source platform leveraging Flask, FastAPI, and regression models to enhance agricultural productivity in Ethiopia.
- A weather-based crop yield prediction tool for Ethiopian farmers, fostering sustainable agriculture through technology.

Instead of relying on missing World Bank temperature data, we will:

- Use rainfall data from World Bank / FAOSTAT.
- Include crop yield & pesticide use data from FAOSTAT.
- If necessary, fetch satellite-based temperature data from ERA5 (a global climate reanalysis dataset).

## 📦 Project Structure

```
📦 CropYieldPredictor-Ethiopia
├── 📂 api
│   ├── main.py            # FastAPI app for handling API endpoints
│   ├── models.py          # Machine learning model loading and prediction logic
│   ├── schemas.py         # Request/response schemas for API
│   ├── utils.py           # Helper functions for the API
│   ├── requirements.txt   # Dependencies for the FastAPI service
├── 📂 app
│   ├── 📂 static          # Static files (CSS, JS, images)
│   ├── 📂 templates       # HTML templates for the Flask frontend
│   ├── app.py             # Flask web app main file
│   ├── forms.py           # Flask-WTF forms for user input
│   ├── config.py          # Configuration settings for Flask
│   ├── requirements.txt   # Dependencies for the Flask web app
├── 📂 data
│   ├── weather_data.csv   # Example dataset for weather data
│   ├── crop_data.csv      # Example dataset for crop yields
│   ├── processed_data.csv # Processed dataset for model training
├── 📂 models
│   ├── train_model.ipynb  # Jupyter notebook for training the ML model
│   ├── model.pkl          # Serialized ML model
├── 📂 deployment
│   ├── Dockerfile         # Dockerfile for containerizing the app
│   ├── docker-compose.yml # Docker Compose file for multi-service setup
│   ├── README.md          # Instructions for deployment
├── 📂 docs
│   ├── README.md          # Documentation for the project
│   ├── api_endpoints.md   # Details about FastAPI endpoints
│   ├── user_manual.md     # Instructions for end-users
├── .env                   # Environment variables (excluded in .gitignore)
├── .gitignore             # Git ignore file
├── README.md              # Main repository README
├── LICENSE                # License for the project
```

## Features in the Structure

1. **Modular API and App Directories**: Separate folders for Flask frontend and FastAPI backend for clean architecture.
2. **Data Folder**: Organized data storage for raw and processed datasets.
3. **Models Directory**: Includes training scripts and serialized models.
4. **Deployment Folder**: Contains files for containerization and deployment, ensuring the app is ready for production.
5. **Documentation**: Clear and detailed documentation files to guide developers and users.