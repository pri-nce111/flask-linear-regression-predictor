# flask-linear-regression-predictor
ML-powered Flask web app for Boston house price prediction using Linear Regression. Interactive UI with real-time predictions and model training features.



# 🏠 Boston House Price Predictor

A machine learning web application built with Flask and scikit-learn that predicts house prices using Linear Regression. This project features an interactive web interface with real-time predictions and model retraining capabilities.

## 🎯 Project Overview

This application uses the famous Boston Housing dataset to predict house prices based on 13 different features including crime rate, number of rooms, accessibility to highways, and more. Built as part of the **Python Zero to Hero Bootcamp**.

## ✨ Features

- **🔮 Real-time Price Prediction**: Input house features and get instant price predictions
- **🎯 Model Retraining**: Retrain the Linear Regression model with a single click
- **📱 Responsive Design**: Beautiful, mobile-friendly interface with modern UI/UX
- **📊 Interactive Form**: Easy-to-use form with feature descriptions and default values
- **🔄 Form Management**: Clear form and reset to default values functionality
- **⚡ Fast Processing**: Optimized Flask backend for quick predictions

## 🛠️ Technology Stack

- **Backend**: Python, Flask
- **Machine Learning**: scikit-learn, NumPy
- **Frontend**: HTML5, CSS3, JavaScript
- **Model**: Linear Regression
- **Data**: Boston Housing Dataset

## 📋 Dataset Features

The model uses 13 input features to predict house prices:

| Feature | Description |
|---------|-------------|
| CRIM | Per capita crime rate by town |
| ZN | Proportion of residential land zoned for lots over 25,000 sq.ft. |
| INDUS | Proportion of non-retail business acres per town |
| CHAS | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| NOX | Nitric oxides concentration (parts per 10 million) |
| RM | Average number of rooms per dwelling |
| AGE | Proportion of owner-occupied units built prior to 1940 |
| DIS | Weighted distances to five Boston employment centers |
| RAD | Index of accessibility to radial highways |
| TAX | Full-value property-tax rate per $10,000 |
| PTRATIO | Pupil-teacher ratio by town |
| B | 1000(Bk - 0.63)² where Bk is the proportion of blacks by town |
| LSTAT | % lower status of the population |

## 🚀 Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/boston-house-price-predictor.git
cd boston-house-price-predictor
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Train the Model
```bash
python app.py
```
This will automatically train the Linear Regression model and save it as `model.pkl`.

### Step 4: Run the Application
```bash
python app.py
```

### Step 5: Access the Application
Open your web browser and navigate to:
```
http://localhost:5000
```

## 📁 Project Structure

```
boston-house-price-predictor/
│
├── app.py                 # Main Flask application & model training script
├── requirements.txt       # Python dependencies
├── index.html            # Frontend interface
├── model.pkl             # Trained Linear Regression model (generated)
└── README.md             # Project documentation
```

## 🎮 Usage

1. **Open the Application**: Navigate to `http://localhost:5000` in your browser
2. **Input Features**: Fill in the house features in the form (default values are provided)
3. **Get Prediction**: Click "🔮 Predict Price" to get the estimated house price
4. **Retrain Model**: Click "🎯 Retrain Model" to retrain the model with fresh data
5. **Clear Form**: Click "🔄 Clear Form" to reset all inputs to default values

## 📊 Model Performance

The Linear Regression model achieves the following performance metrics on the test set:

- **R² Score**: ~0.67 (67% accuracy)
- **Mean Absolute Error (MAE)**: ~3.27K
- **Root Mean Squared Error (RMSE)**: ~4.68K

*Note: Results may vary slightly due to random train/test splits*

## 🔧 API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/` | GET | Serve the main interface |
| `/predict` | POST | Predict house price based on input features |
| `/train` | POST | Retrain the Linear Regression model |

## 📝 Important Notes

- The dataset uses median home values in thousands of dollars (1970s prices)
- Modern equivalent prices would be significantly higher due to inflation
- The model is trained on historical data and should be used for educational purposes
- Some features in the original dataset may not reflect current social perspectives

## 🔮 Future Improvements

- [ ] Add more advanced ML algorithms (Random Forest, XGBoost)
- [ ] Implement feature importance visualization
- [ ] Add data visualization charts
- [ ] Create model comparison functionality
- [ ] Add input validation and error handling
- [ ] Implement model performance metrics display
- [ ] Add data preprocessing options
- [ ] Create API documentation with Swagger

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

Prince Prajapati
- GitHub: https://github.com/pri-nce111
- LinkedIn: https://www.linkedin.com/in/prince-prajapati-133020252/

## 🙏 Acknowledgments

- Python Zero to Hero Bootcamp for the project inspiration
- scikit-learn team for the amazing machine learning library
- Boston Housing dataset contributors
- Flask community for the excellent web framework

---

