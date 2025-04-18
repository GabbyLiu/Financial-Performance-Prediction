# Financial Performance Prediction & Portfolio Optimization Platform

A modern web application that combines advanced financial models with machine learning to provide portfolio optimization and stock prediction capabilities.

## 🌟 Features

- **Portfolio Optimization**
  - Black-Litterman Model implementation
  - Markowitz Model optimization
  - Hierarchical Risk Parity
  - Customizable risk parameters

- **Stock Analysis & Prediction**
  - Statistical models (ARIMA, GARCH)
  - Machine Learning models (Random Forest, XGBoost)
  - Neural Network predictions
  - Technical indicator analysis

- **Interactive Dashboard**
  - Real-time portfolio metrics
  - Asset allocation visualization
  - Risk-return analysis
  - Historical performance tracking

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Node.js 14+
- npm or yarn
- PostgreSQL (for production)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/financial-performance-prediction.git
   cd financial-performance-prediction
   ```

2. **Backend Setup**
   ```bash
   cd backend
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   ```

### Configuration

1. **Backend Configuration**
   Create a `.env` file in the backend directory:
   ```
   DATABASE_URL=postgresql://user:password@localhost:5432/finance_db
   SECRET_KEY=your_secret_key
   API_KEY=your_api_key
   ```

2. **Frontend Configuration**
   Create a `.env` file in the frontend directory:
   ```
   REACT_APP_API_URL=http://localhost:8000
   ```

### Running the Application

1. **Start the Backend**
   ```bash
   cd backend
   uvicorn main:app --reload
   ```

2. **Start the Frontend**
   ```bash
   cd frontend
   npm start
   ```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:8000
- API Documentation: http://localhost:8000/docs

## 📊 Project Structure

```
financial-performance-prediction/
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── models/
│   │   └── services/
│   ├── requirements.txt
│   └── main.py
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── utils/
│   └── package.json
└── README.md
```

## 🔧 API Endpoints

### Portfolio Management
- `POST /portfolio/optimize` - Optimize portfolio weights
- `GET /portfolio/analysis/{symbol}` - Get stock analysis
- `GET /portfolio/history` - Get portfolio performance history

### Stock Analysis
- `GET /stocks/predict/{symbol}` - Get stock price predictions
- `GET /stocks/indicators/{symbol}` - Get technical indicators
- `GET /stocks/historical/{symbol}` - Get historical data

## 🧪 Testing

### Backend Tests
```bash
cd backend
pytest
```

### Frontend Tests
```bash
cd frontend
npm test
```

## 📈 Models and Algorithms

### Portfolio Optimization
- Black-Litterman Model
- Markowitz Modern Portfolio Theory
- Hierarchical Risk Parity

### Stock Prediction
- ARIMA (Autoregressive Integrated Moving Average)
- GARCH (Generalized Autoregressive Conditional Heteroskedasticity)
- Random Forest
- XGBoost
- Neural Networks with Monte Carlo Dropout

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [PyPortfolioOpt](https://github.com/robertmartin8/PyPortfolioOpt) for portfolio optimization tools
- [yfinance](https://github.com/ranaroussi/yfinance) for financial data
- [Material-UI](https://mui.com/) for frontend components
- [FastAPI](https://fastapi.tiangolo.com/) for backend framework

## 📧 Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter) - email@example.com

Project Link: [https://github.com/yourusername/financial-performance-prediction](https://github.com/yourusername/financial-performance-prediction)
