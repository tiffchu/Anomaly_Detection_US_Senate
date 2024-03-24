# Anomaly Detection of US Senate Investments
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Datasets</a></li>
      </ul>
    </li>
    <li><a href="#approach">Approach</a></li>
    <li><a href="#eda">EDA</a></li>
    <li><a href="#Modelling">Modelling</a></li>
    <li><a href="#next-steps">Next Steps</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project  📈

This capstone analyzes time series data of stock transactions from US congress members, and aims to identify anomalies that may point to insider trading.

#### Problem Statement 🤯
* Members of Congress wield significant influence over companies they invest in, raising concerns about potential conflicts of interest and unfair advantages in financial markets
* The STOCK Act mandates public reporting of asset transactions by Congress members, providing an opportunity to detect and prevent insider trading
* This project addresses the challenge of identifying abnormal stock purchases that may warrant further investigation.
others

<!-- GETTING STARTED -->
## Getting Started
Download the jupyter file in this repository, or open it in google colab. 

### Dataset 
The dataset consists of combined data from Senate stock transactions and stock news events. It covers the period from 2020 to 2023 and contains approximately 30,000 rows and 12 relevant columns. Data quality concerns include missing values in news events and potential overlaps in news event timelines with transaction dates.

These are the datasets I'll be using 
- [Congress trades dataset](https://senatestockwatcher.com/api)
- S&P Data from Yfinance

<!-- ROADMAP -->
## Roadmap 

- [x] EDA
- [x] Update Readme
- [x] Scaling
- [x] One hot encoding
- [x] Find a stock market metric
- [x] Choose algorithms to classify data
    - [ ] Clustering
    - [ ] Isolation forest
    - [ ] Encoders
    - [ ] LSTM

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- APPROACH -->
## Approach

The project takes a data-driven approach by combining numerical and textual data from Senate stock transactions and financial news. Unsupervised machine learning algorithms, including hierarchical clustering, isolation forest, and LSTM autoencoders, are utilized for anomaly detection. Feature engineering techniques such as sentiment analysis and market indices inclusion are employed to enhance model performance.

<!-- EDA -->
## EDA

1. **Data Processing**: Merge and preprocess datasets, handle missing values, and ensure data consistency.
2. **Feature Engineering**: Extract relevant features, including temporal, numerical, and textual features. Then incorporate market indices.
3. **Sort Data**: Based on transaction dates, and make sure the merged dataset has matching dates.

<!-- Modelling -->
5. **Time Series Plots**: Baseline visualizations of the data based on dates
6. **Scaling data**: So that certain columns dont dominate others. - Use robust scaling.
7. **One hot encoding**: Turning categorical columns (type, party, industry, sector, owner) into numerical
8. **Baseline Modelling**: Getting the models started for Autoencoding, hierarchical clustering, isolation forest

<!-- NEXT STEPS -->
## Next Steps
 
- **Deriving Model Performance and Explore Patterns and Trends**: Visualize the data surrounding the anomalies to identify any patterns or trends that might explain them
- **Research Online**: Use domain knowledge to interpret the anomalies. confirm through manually searching anomalies. 
- **Iterative Changes**: Fine-tune model hyperparameters, experiment with different values. 
- **Documentation and Reporting**: Document project steps, summarize findings, and communicate results to stakeholders.


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<!-- CONTACT -->
## Contact

Tiffany Chu - tiffanymchu@gmail.com

Project Link: [https://github.com/tiffchu/Anomaly_Detection_US_Senate](https://github.com/tiffchu/Anomaly_Detection_US_Senate/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
- me and brainstation 👩‍❤️‍👩
