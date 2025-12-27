<h1 align = center>
✈️ Airline Flight Delays ✈️
</h1>
<h3 align = center>
Analysis for 5,000,000+ Commercial Airline Flights in 2015
</h3>
<h5 align = center><i>Data and questions sourced from <a>mavenanalytics.io/data-playground/airline-flight-delays</i></a></h4>

---

## Steps to follow
1. Clone repositroy
```bash
git clone https://github.com/juggled/2015-airplane-mavenanalytics.git
```
2. Install requirements
```bash
pip3 install -r requirements.txt
```
3. Download ALL CSVs from <a>mavenanalytics.io/data-playground/airline-flight-delays</a>
4. Download random_forest-Model.joblib from releases section as this was removed due to file limits
4. Launch Jupyter to open the notebooks
5. There are four notebooks. The first notebook is main.ipynb , which answers the questions from mavenanalytics. The second is tree.ipynb , which is a random forest classifier to guess if it's a delayed flight. The third is catboost.ipynb to guess if it's a delayed flight via catboost. The latter two were run in Google Colab with the T4-GPU and then exported. The fourth is a comparison between the two models via a bar graph.
---
## Explanation of files
### File directory
```bash
📦Airlines+Airports+Cancellation+Codes+&+Flights
 ┣ 📂data
 ┃ ┗ 📂01-raw # All of these files are not uploaded. PLease download directly from mavenanalytics.io/data-playground/airline-flight-delays
 ┃ ┃ ┣ 📜airlines.csv
 ┃ ┃ ┣ 📜airports.csv
 ┃ ┃ ┣ 📜cancellation_codes.csv
 ┃ ┃ ┗ 📜flights.csv
 ┣ 📂model
 ┃ ┣ 📜catboost_model
 ┃ ┗ 📜random_forest_model.joblib # Removed due to size limits, please download from releases
 ┣ 📂src
 ┃ ┣ 📜comparison.ipynb
 ┃ ┣ 📜catboost.ipynb
 ┃ ┣ 📜main.ipynb
 ┃ ┗ 📜tree.ipynb
 ┣ 📜.gitignore
 ┣ 📜ComparisonBetweenCatBoost&RandomForestClassifier.jpg
 ┣ 📜README.md
 ┗ 📜requirements.txt
 ```
 ### Pre-included data
 - data/01-raw
    - All files in here are from mavenanalytics
    - Processing was not needed
- model
    - catboost_model is model made by catboost
    - random_forest_model.joblib is model made by RandomForestClassifier
- src
    - comparison.ipynb
        - Compares the two different models in an interactive bar graph
    - catboost.ipynb
        - File to run Catboost
    - main.ipynb
        - File to answer questions
    - tree.ipynb
        - File to run RandomForestClassifier
- ComparisonBetweenCatBoost&RandomForestClassifier.jpg
    - Comparison between Cat Boost & Random Forest Classifier models
- README.md
    - The current file
- requirements.txt
    - Required libraries to install
- .gitignore
    - Files for GitHub to ignore uploading