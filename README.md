# Recommender System for User Connections

This repository contains a Python-based recommender system that predicts user connections based on preference data stored in a CSV file. The system uses collaborative filtering with matrix factorization to analyze user impressions (likes or preferences) and recommend potential connections. It accounts for reciprocal dislikes to ensure accurate recommendations, making it suitable for applications like social networking, matchmaking, or team formation.

## Features
- **Data Processing**: Loads user preference data from a CSV file (`data.csv`) containing email addresses and up to 30 impressions per user.
- **Adjacency Matrix**: Constructs a binary adjacency matrix where `1` indicates a mutual like, `-1` indicates an unreciprocated like (dislike), and `0` indicates no interaction.
- **Matrix Factorization**: Applies Singular Value Decomposition (SVD) to predict latent connections between users.
- **Connection Analysis**: Identifies the top 10 most connected users based on predicted connections.
- **Scalability**: Handles variable-sized datasets with missing values (NaN) in the impressions columns.

## Prerequisites
To run the recommender system, ensure you have the following installed:
- Python 3.8 or higher
- Required Python libraries:
  - `pandas`
  - `numpy`

You can install the dependencies using:
pip install pandas numpy

#Installation
1. Clone the repository: 'git clone https://github.com/Kanishkjain0510/Recommender-system.git'
