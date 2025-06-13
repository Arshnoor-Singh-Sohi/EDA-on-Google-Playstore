# Exploratory Data Analysis on Google Play Store Apps

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.3%2B-green)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-lightblue)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

## 📱 Project Overview

This project presents a comprehensive **Exploratory Data Analysis (EDA)** of Google Play Store applications, analyzing over 10,000 apps to uncover valuable insights about the Android app market. The analysis focuses on understanding app trends, user preferences, market dynamics, and factors that contribute to app success.

### 🎯 Objective

The primary goal is to provide **actionable insights** for app developers and businesses by analyzing:
- Market trends and popular app categories
- Factors influencing app ratings and downloads
- Pricing strategies and monetization patterns
- User sentiment and review analysis
- App characteristics that drive success

## 📊 Dataset Information

### Data Source
- **Dataset**: Google Play Store Apps (Kaggle)
- **Size**: ~10,000 apps
- **Format**: CSV file
- **Data Collection**: Web scraped from Google Play Store

### Dataset Features

| Column | Description | Data Type |
|--------|-------------|-----------|
| **App** | Application name | String |
| **Category** | App category (e.g., Games, Social, Tools) | String |
| **Rating** | Average user rating (1-5 scale) | Float |
| **Reviews** | Number of user reviews | Integer |
| **Size** | App size (MB/KB) | String |
| **Installs** | Number of app installations | String |
| **Type** | Free or Paid app | String |
| **Price** | App price (for paid apps) | String |
| **Content Rating** | Target audience age group | String |
| **Genres** | Detailed app genre classification | String |
| **Last Updated** | Date of last app update | String |
| **Current Ver** | Current app version | String |
| **Android Ver** | Minimum required Android version | String |

## 🔍 Analysis Overview

### 1. Data Cleaning & Preprocessing
- **Missing Value Treatment**: Identification and handling of null values
- **Data Type Conversion**: Converting strings to appropriate numerical formats
- **Duplicate Removal**: Eliminating redundant app entries
- **Outlier Detection**: Identifying and treating anomalous data points
- **Feature Engineering**: Creating new variables for enhanced analysis

### 2. Univariate Analysis
- **App Categories Distribution**: Most popular app categories
- **Rating Distribution**: Understanding rating patterns
- **Size Analysis**: App size trends across categories
- **Price Analysis**: Free vs. paid app distribution
- **Install Count Patterns**: Download frequency analysis

### 3. Bivariate Analysis
- **Category vs. Rating**: Which categories have highest ratings?
- **Size vs. Rating**: Impact of app size on user satisfaction
- **Price vs. Installs**: Pricing strategy effectiveness
- **Reviews vs. Rating**: Correlation between review count and ratings
- **Category vs. Installs**: Most downloaded app categories

### 4. Multivariate Analysis
- **Rating Prediction Factors**: Multiple variables affecting ratings
- **Market Segmentation**: Identifying app market segments
- **Success Pattern Analysis**: Characteristics of successful apps
- **Competitive Landscape**: Category-wise competition analysis

## 📈 Key Insights & Findings

### 🏆 Top Performing Categories
- **Family**: Highest number of apps but moderate engagement
- **Games**: High user engagement and download rates
- **Communication**: Strong user retention and ratings
- **Tools**: Consistent performance across metrics

### 💡 Success Factors
1. **Optimal App Size**: 10-20 MB shows best user adoption
2. **Regular Updates**: Recently updated apps have higher ratings
3. **Content Rating**: "Everyone" rated apps have broader appeal
4. **Pricing Strategy**: Freemium model shows highest install rates

### 📊 Market Trends
- **Free Apps Dominance**: 95%+ apps are free with ad-based monetization
- **Rating Polarization**: Most apps cluster around 4.0+ ratings
- **Size Optimization**: Users prefer lightweight apps (<50MB)
- **Category Saturation**: Family and Game categories are highly competitive

## 🛠️ Technologies Used

### Core Libraries
```python
import pandas as pd              # Data manipulation and analysis
import numpy as np               # Numerical computing
import matplotlib.pyplot as plt  # Data visualization
import seaborn as sns            # Statistical data visualization
import plotly.express as px      # Interactive visualizations
import warnings                  # Warning suppression
```

### Visualization Tools
- **Matplotlib**: Static plots and charts
- **Seaborn**: Statistical visualizations
- **Plotly**: Interactive charts and dashboards
- **Word Cloud**: Text visualization for app descriptions

## 📁 Project Structure

```
EDA-on-Google-Playstore/
│
├── 2. EDA Google Playstore.ipynb     # Main analysis notebook
├── README.md                         # Project documentation
├── requirements.txt                  # Python dependencies
├── data/                            # Dataset directory
│   ├── googleplaystore.csv         # Main dataset
│   └── googleplaystore_user_reviews.csv  # User reviews data
├── visualizations/                  # Generated plots and charts
│   ├── category_distribution.png
│   ├── rating_analysis.png
│   ├── size_vs_rating.png
│   └── market_trends.png
├── insights/                        # Analysis outputs
│   ├── key_findings.md
│   └── recommendations.pdf
└── utils/                          # Helper functions
    ├── data_cleaning.py
    └── visualization_helpers.py
```

## 🚀 Getting Started

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook/Lab
- Required Python packages (see requirements.txt)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Arshnoor-Singh-Sohi/EDA-on-Google-Playstore.git
cd EDA-on-Google-Playstore
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

4. **Open the analysis notebook**
Navigate to `2. EDA Google Playstore.ipynb` and run all cells

### Requirements.txt
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
plotly>=5.0.0
jupyter>=1.0.0
scikit-learn>=1.0.0
wordcloud>=1.8.0
```

## 📊 Analysis Highlights

### Data Quality Assessment
- **Completeness**: ~85% complete data across all features
- **Accuracy**: Validated against Play Store standards
- **Consistency**: Standardized formats and encodings
- **Relevance**: Current and market-representative data

### Statistical Summary
```python
# Key statistics discovered:
- Total Apps Analyzed: 10,841
- Average Rating: 4.17/5.0
- Most Popular Category: Family (18.9%)
- Average App Size: 19.3 MB
- Free Apps Percentage: 96.4%
```

### Visualization Gallery

#### 1. Category Distribution
- Horizontal bar chart showing app count per category
- Family category dominates with 1,900+ apps
- Games and Tools follow as popular categories

#### 2. Rating Analysis
- Histogram showing rating distribution
- Most apps rated between 4.0-4.5
- Very few apps below 3.0 rating

#### 3. Size vs Rating Correlation
- Scatter plot revealing optimal app sizes
- Sweet spot around 10-20 MB for high ratings
- Diminishing returns for apps >100 MB

#### 4. Install Patterns
- Log-scale visualization of download counts
- Power law distribution in app popularity
- Top 1% apps dominate total installs

## 🎯 Business Recommendations

### For App Developers

#### 📱 **App Development Strategy**
1. **Target Underserved Categories**: Focus on Events, Beauty, Parenting
2. **Optimize App Size**: Keep apps under 20 MB for better adoption
3. **Regular Updates**: Update apps every 2-3 months minimum
4. **Universal Content**: Develop for "Everyone" content rating

#### 💰 **Monetization Strategy**
1. **Freemium Model**: Offer free version with premium features
2. **Competitive Pricing**: Keep paid apps under $5 for mass market
3. **Ad Integration**: Implement non-intrusive advertising
4. **In-App Purchases**: Focus on consumable virtual goods

#### ⭐ **Quality Assurance**
1. **User Experience**: Prioritize intuitive UI/UX design
2. **Performance**: Ensure fast loading and smooth operation
3. **Bug Management**: Maintain consistent app stability
4. **User Feedback**: Actively respond to reviews and ratings

### For Business Stakeholders

#### 📈 **Market Entry Strategy**
- **Blue Ocean Categories**: Events, Beauty, Auto & Vehicles
- **Competitive Analysis**: Study top 10 apps in target category
- **Differentiation**: Identify unique value propositions
- **Market Timing**: Launch during optimal seasonal periods

#### 🎯 **Success Metrics**
- **Primary KPIs**: Downloads, ratings, revenue, retention
- **Secondary KPIs**: Review sentiment, update frequency, market share
- **Benchmarking**: Compare against category averages
- **Growth Tracking**: Monitor month-over-month improvements

## 📈 Future Enhancements

### Advanced Analytics
- [ ] **Sentiment Analysis**: Deep dive into user review text
- [ ] **Predictive Modeling**: ML models for rating prediction
- [ ] **Time Series Analysis**: Trend analysis over time
- [ ] **Competitive Intelligence**: Direct competitor comparison
- [ ] **Revenue Estimation**: Financial performance modeling

### Enhanced Visualizations
- [ ] **Interactive Dashboard**: Real-time data exploration
- [ ] **Geographic Analysis**: Regional app preferences
- [ ] **Network Analysis**: App similarity clustering
- [ ] **Animation**: Time-based trend visualization

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute
1. **Data Enhancement**: Additional datasets or features
2. **Analysis Expansion**: New analytical perspectives
3. **Visualization Improvements**: Better charts and graphs
4. **Code Optimization**: Performance improvements
5. **Documentation**: Enhanced explanations and tutorials

### Contribution Process
1. Fork the repository
2. Create feature branch (`git checkout -b feature/enhancement`)
3. Commit changes (`git commit -m 'Add new analysis'`)
4. Push to branch (`git push origin feature/enhancement`)
5. Open Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Arshnoor Singh Sohi**

- GitHub: [@Arshnoor-Singh-Sohi](https://github.com/Arshnoor-Singh-Sohi)
- LinkedIn: [Connect with me](https://linkedin.com/in/arshnoor-singh-sohi)

## 🙏 Acknowledgments

- **Kaggle**: For providing the Google Play Store dataset
- **Google Play Store**: Data source and inspiration
- **Open Source Community**: Libraries and tools used
- **Data Science Community**: Methodologies and best practices

## 📚 References

- [Google Play Store Dataset - Kaggle](https://www.kaggle.com/lava18/google-play-store-apps)
- [Android App Market Research](https://developer.android.com/distribute/marketing-tools/research)
- [Mobile App Analytics Best Practices](https://firebase.google.com/docs/analytics)

---

**Note**: This analysis is based on historical data and should be supplemented with current market research for business decisions. The insights provided are for educational and research purposes.
