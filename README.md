# Lottery Probability Calculator & Visualizer

A Python tool that calculates and visualizes match probabilities in lottery systems (like 6/49), using combinatorial mathematics.

![Probability Distribution](lottery_probabilities.png)

## Features
- 🎲 Calculates exact probabilities for all possible matches (0-6)
- 📊 Generates professional-grade visualizations
- 📈 Computes cumulative probabilities (e.g., "<3 matches")
- 🖥️ Saves visualization as high-resolution PNG
- 🔧 Configurable for any K/N/n lottery system

## Installation
```bash
pip install matplotlib

Usage

    Modify parameters in lottery_probability.ipynb:

python

K = 6   # Known numbers (winning numbers)
N = 49  # Total numbers in pool
n = 6   # Numbers drawn

    Run:

bash

python lottery_probability.ipynb

Sample Output

Probability of matches in 6-number draw from 49 numbers (6 known numbers):

#01 -- 0 matches: 43.59650541%
#02 -- 1 matches: 41.30194507%
#03 -- 2 matches: 13.23780290%
#04 -- 3 matches: 1.76504039%
#05 -- 4 matches: 0.09686197%
#06 -- 5 matches: 0.00184499%
#07 -- 6 matches: 0.00000715%

Probability of <3 matches: 98.13625338%

Mathematical Basis

Uses hypergeometric probability formula:

P(k) = [C(K,k) × C(N-K, n-k)] / C(N,n)

Where:

    C(n,k) = combinations of n items taken k at a time

    K = known numbers

    N = total numbers

    n = numbers drawn

    k = matches

Customization

    Change K, N, n for different lottery formats

    Modify visualization colors/styles in the plt commands

    Adjust decimal precision in the print statements
