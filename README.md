🏡 Housing Market EDA — Hyderabad Real Estate Data
This project presents an exploratory data analysis (EDA) of residential property listings in Hyderabad, India.
The data was scraped from CommonFloor and includes attributes like price, area, agent, BHK type, house type, direction, and locality.

📁 Files Included
.
├── Dataset.csv                 # 📊 Main dataset with 23,970 property records
├── Script.ipynb           # 📒 Jupyter notebook performing EDA
└── README.md                   # 📄 Project overview and documentation
📊 Dataset Overview
The dataset contains 23,970 property listings with the following features:

Column	Description
Area_sq.ft	Total area in square feet
Price	Property price in lakhs
Price_per_sq.ft	Price per square foot
Locality	Area or neighborhood in Hyderabad
Booking_start	Days since posted
Agent_Name	Name of the property listing agent
Direction	Facing direction (e.g., east, west)
parking	Availability of parking (Yes/No/Unknown)
Type_BHK	Number of bedrooms (e.g., 2BHK, Plot)
Type_Of_House	Apartment or Plot
📈 EDA Highlights
The notebook performs:

Univariate Analysis

Distribution of Price, Area, Price per Sq.Ft
Count of BHK types, facing directions, and house types
Bivariate Analysis

Correlation between area and price
Price trends across localities and BHK types
Agent-level summary: average price, number of listings
Derived Insights

Which localities are most expensive?
Are plots cheaper than apartments per sq.ft?
Most active agents and their pricing behavior
📌 Sample Insights
# Highest priced localities
df.groupby("Locality")["Price"].mean().sort_values(ascending=False).head()

# Parking impact on price per sq.ft
df.groupby("parking")["Price_per_sq.ft"].mean()
🛠️ Requirements
Python 3.x
Jupyter Notebook
Libraries:
pandas
numpy
matplotlib
seaborn
Install with:

pip install pandas numpy matplotlib seaborn
🚀 How to Run
Clone the repo or download the files
Launch Jupyter Notebook
Open Script.ipynb
Run all cells to explore insights and visualizations
👤 Author
Sameena Banu
GitHub: @Samee-na28

📄 License
This project is for academic and learning purposes. Attribution appreciated.
