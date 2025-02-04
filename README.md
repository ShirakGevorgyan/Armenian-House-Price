# House Price Prediction in Yerevan

## Project Overview
This project involves web scraping, data collection, and machine learning to predict house prices in Yerevan based on various parameters. Using Selenium, data was gathered from two real estate websites listing properties for sale in Yerevan. The extracted data was then used to train a machine learning model capable of predicting house prices based on different features.

## Data Collection
### Web Scraping with Selenium
Selenium was used to automate the process of extracting house listings, including key property details such as:
- **Region (Տարածաշրջան)**
- **Building Type (Շինության տիպ)**
- **Number of Rooms (Սենյակներ)**
- **Area (Մակերես in sq. meters)**
- **Floor (Հարկ)**
- **Renovation Status (Վերանորոգում)**
- **Price**

The scraped data was stored in CSV format (`Haus_Price.csv`) for further processing and analysis.

## Machine Learning Model
### Model Selection
The project employs a **RandomForestRegressor**, a powerful ensemble learning method, to predict house prices based on the extracted parameters.

### Hyperparameter Tuning
To optimize the model's performance, **GridSearchCV** was used for hyperparameter tuning. This helped find the best combination of parameters for accurate predictions.

## Technologies Used
- **Python** (for data processing and modeling)
- **Selenium** (for web scraping)
- **pandas, numpy** (for data manipulation)
- **scikit-learn** (for machine learning)
- **RandomForestRegressor** (for price prediction)
- **GridSearchCV** (for hyperparameter tuning)

## Files & Directories
- `Pars_1.ipynb` & `Pars_2.ipynb` - Jupyter notebooks containing the web scraping scripts.
- `Haus_Price.csv` - Collected house price data.
- `Haus_price.ipynb` - Data preprocessing and model training.
- `chromedriver` - Selenium WebDriver for web scraping.
- `README.md` - This documentation file.

## Usage
1. Ensure you have Python and required libraries installed:
   ```sh
   pip install selenium pandas numpy scikit-learn
   ```
2. Run the web scraping script to collect updated house prices.
3. Train the machine learning model using `Haus_price.ipynb`.
4. Use the trained model to predict house prices in Yerevan based on new property details.

## Conclusion
This project demonstrates how web scraping and machine learning can be combined to create a predictive model for real estate pricing. The model can be further improved by incorporating additional data sources and using more advanced ML techniques.

---


