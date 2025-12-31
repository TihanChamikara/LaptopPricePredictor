# Laptop Price Predictor

A machine learning-powered web application that predicts laptop prices based on their specifications. This Flask-based application uses a trained scikit-learn model to provide instant price estimates in LKR (Sri Lankan Rupees).

## 📋 Description

The Laptop Price Predictor is an intelligent web application that helps users estimate laptop prices based on various hardware specifications and features. By inputting details such as RAM, weight, brand, processor type, graphics card, and display features, users receive an estimated price prediction powered by a machine learning model.

## ✨ Features

- **Intelligent Price Prediction**: Uses a pre-trained machine learning model to estimate laptop prices
- **User-Friendly Interface**: Clean, modern web interface with Font Awesome icons
- **Comprehensive Specifications**: Supports multiple input parameters including:
  - RAM capacity (GB)
  - Weight (Kg)
  - Brand/Company (Acer, Apple, Asus, Dell, HP, Lenovo, MSI, Toshiba, and more)
  - Laptop Type (2-in-1 Convertible, Gaming, Netbook, Notebook, Ultrabook, Workstation)
  - Operating System (Windows, Mac, Linux, Other)
  - CPU (Intel Core i3/i5/i7, AMD, Other)
  - GPU (Intel, AMD, Nvidia)
  - Touchscreen capability
  - IPS Display
- **Instant Results**: Real-time price prediction displayed in LKR
- **Responsive Design**: Custom-styled interface with modern aesthetics

## 🛠️ Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Step 1: Clone the Repository

```bash
git clone https://github.com/[YourUsername]/[Insert Your Repo Name Here].git
cd [Insert Your Repo Name Here]
```

### Step 2: Create a Virtual Environment

```bash
python -m venv env
```

### Step 3: Activate the Virtual Environment

**On Windows:**
```bash
env\Scripts\activate
```

**On macOS/Linux:**
```bash
source env/bin/activate
```

### Step 4: Install Required Dependencies

```bash
pip install flask numpy scikit-learn
```

Alternatively, if a `requirements.txt` file is provided:
```bash
pip install -r requirements.txt
```

## 🚀 How to Run the Project

1. **Navigate to the web application directory:**
   ```bash
   cd "web application"
   ```

2. **Run the Flask application:**
   ```bash
   python app.py
   ```

3. **Access the application:**
   - Open your web browser
   - Navigate to `http://127.0.0.1:5000/` or `http://localhost:5000/`

4. **Use the predictor:**
   - Fill in the laptop specifications in the form
   - Click "Predict Price" to get the estimated price
   - The predicted price will be displayed in LKR

## 📁 Project Structure

```
LaptopPricePredictor/
├── env/                          # Virtual environment
├── web application/
│   ├── app.py                    # Main Flask application
│   ├── model/
│   │   └── predictor.pickle      # Pre-trained ML model
│   ├── static/
│   │   └── style.css             # Custom CSS styles
│   └── templates/
│       └── index.html            # Main HTML template
└── README.md                     # Project documentation
```

## 🤖 How It Works

1. The user inputs laptop specifications through the web form
2. The Flask backend receives the form data via POST request
3. Input features are processed and encoded into the format expected by the model
4. The pre-trained machine learning model (`predictor.pickle`) makes a prediction
5. The predicted price is calculated and converted to LKR
6. Results are displayed on the web interface

## 🔧 Technologies Used

- **Backend**: Flask (Python web framework)
- **Machine Learning**: scikit-learn, NumPy
- **Frontend**: HTML5, CSS3
- **Icons**: Font Awesome 6.4.0
- **Model Storage**: Pickle

## 📝 Notes

- The model predicts prices in LKR (Sri Lankan Rupees)
- The prediction is based on the trained model's understanding of laptop specifications and their correlations with price
- Ensure all required fields are filled before submitting the form

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

Your Name - [Your GitHub Profile]

## 🙏 Acknowledgments

- Dataset used for training the machine learning model
- Flask documentation and community
- scikit-learn library contributors
