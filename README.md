# Cricket Analytics

A data-driven approach to select the optimal cricket team based on player performance metrics and team composition constraints.

## Overview

This project aims to analyze cricket player performance data and select the best possible team of 11 players while adhering to specific constraints. It involves data cleaning, statistical analysis, and optimization techniques to ensure a balanced and high-performing team selection.

## Features

- Data cleaning and preparation
- Player performance analysis (batting, bowling, wicketkeeping, all-rounder)
- Team composition optimization
- Consistency and recency calculations
- Automated data pipeline for scalability

## Tech Stack

![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

## Installation

1. Clone the repository: git clone https://github.com/chetanyamahana/Cricket-Analytics

## Data Cleaning and Preparation

- Removal of duplicates
- Handling of missing values
- Correction of data types
- Logical imputations based on related data

## Player Selection Strategy

### Batsmen
- Total Points: Based on Strike Rate, Batting Average, Centuries, and Half-centuries
- Consistency Score: Standard Deviation of Strike Rate
- Recency Score: Exponentially Weighted Average (EWA) of Strike Rate

### Bowlers
- Total Points: Based on Bowling Strike Rate, Economy Rate, Bowling Average, and Four-wicket hauls
- Consistency Score: Standard Deviation of Economy Rate
- Recency Score: EWA of Economy Rate

### All-Rounders
- Combined score of batting and bowling points

### Wicketkeepers
- Batting points and designation as wicketkeeper in at least 2 matches

## Optimization Technique

- Normalization of scores
- Weighted combination of Total Points, Consistency, and Recency scores
- Team composition constraints adherence

## Scalability

- Automated data pipeline
- Dynamic weight adjustment using machine learning
- Continuous improvement through feedback loops
