# 🏏 IPL Moneyball Analytics – Crickonomics
A Data-Driven Approach to Building a Competitive IPL Team

This project applies analytics and machine learning to the Indian Premier League (IPL) with the goal of constructing a competitive, low-budget franchise using only objective performance metrics — inspired by the Moneyball philosophy.

Instead of relying on reputation or star power, we evaluated players using statistical modeling, predicted auction prices, and tested team performance through large-scale simulations.

### 📌 Important Note on Code Availability

Due to college academic policies and project restrictions, the source code and notebooks used for modeling cannot be uploaded publicly on GitHub.
However, this repository contains:

All datasets used in the project

The final project report

The poster presented at NMIMS University Day Symposium

The project presentation slides

This README explains the complete methodology so the workflow and findings remain fully transparent and reproducible in concept.

## 🎯 Project Objective

Build an IPL team primarily from unsold / undervalued players

Keep the total budget lower than existing franchises

Use analytics instead of intuition for selection

Validate competitiveness using simulation

## 📂 Repository Contents
1. Data

Player statistics for 300+ IPL players

Unsold player pool with batting, bowling & fielding metrics

Sold players dataset with base price & final auction price

Final rated player lists after PCA weighting

Playing XI data of all IPL teams

2. Documents

Project Report (PDF): Detailed methodology, models, and results

Presentation (PDF): Summary slides explaining workflow

Poster (PDF): Presented at the NMIMS 23rd University Day Symposium

## 🧠 Methodology Overview
#### 1️⃣ Player Rating System

Three approaches were compared:

Recursive Feature Elimination (RFE)

PCA on raw statistics

PCA on engineered T20 features (selected method)

Engineered features included:

Hard-Hitter Index

Finisher Ability

Boundary Frequency

Strike Bowler Efficiency

Pressure Builder Metric

Consistency Scores

PCA on engineered features provided the most realistic evaluation of T20 performance.

#### 2️⃣ Auction Price Prediction

Models tested:

Random Forest Regressor

XGBoost

K-Nearest Neighbours (Best – R² ≈ 0.53)

This helped estimate the expected cost of each target player and identify high value-for-money picks.

#### 3️⃣ Team Formation

Initial squad from unsold players: ₹54 Cr

IPL rule requires minimum ₹90 Cr spend

To simulate a real scenario, we:

Replaced Rajasthan Royals (worst performing team in previous season – 9th place, 4/14 wins)

Used new-franchise pre-signing rule

Pre-signed players:

Yashasvi Jaiswal – ₹20 Cr

Jofra Archer – ₹12 Cr

Riyan Parag – ₹12 Cr

➡ Final Squad Cost: ₹94.64 Cr
➡ Lower than all existing IPL teams

#### 4️⃣ Performance Validation

Simulated 1,000,000 IPL seasons

Match outcomes based on logistic regression of team ratings

Results:

Playoff Qualification: 39.57%

Final Appearance: ~21%

Championship Probability: 10.44%

The team built mainly from unsold players performed on par with several real franchises.

### 📈 Key Learnings

Data analytics can uncover hidden talent ignored in auctions

Performance-based selection can rival reputation-based buying

Budget-efficient teams can still be highly competitive

Simulation helps validate decisions before real investment

### 🧩 Limitations

Auction dynamics (brand value, bidding wars) not fully modeled

Fielding metrics limited by public data

Player form treated as static in simulations

Dataset size restricted to available seasons

### 🚀 Future Scope

Context-aware ratings (venue, opposition, match phase)

Dynamic form modeling

Advanced price prediction using deep learning

Player synergy & matchup analysis

## 👥 Team

Keegan Nunes – NSOMASA, Mumbai

Shrey Agarwal

Shashvath Arun

Shitiz Gupta

Project presented at SVKM NMIMS – 23rd University Day Poster Symposium, representing NSOMASA Mumbai Campus.

## 📬 Contact

I’d love to discuss this project, sports analytics, or data science opportunities.

Connect with me on LinkedIn: [your link]

⭐ If you find the methodology interesting, feel free to star this repository!
