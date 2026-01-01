# Ironman-703-Performance-Predictor
This is a physiological inference model designed to predict race performance based on cumulative training history and biological efficiency.

The Science Behind the Model: 
This Model (Which I was interested in building thanks to Andrew Ng's Machine Learning Principles Course) interprets training data through: 
- Cumulative Volume: Analyzes the total "aerobic bank" built over a multi week training block.
- Physiological Efficiency: Weights training ROI based on: Watts/kg, Swim Heart Rate efficiency, and Run Economy.
- Logarithmic Adaptation: Uses `np.log1p` to account for Diminishing Returns, ensuring realistic performance gains.
- Course Physics: Factors in specific terrain multipliers for the Victoria 70.3 bike hills and trail run.

Target Benchmark:
- Goal Finish time: 4:58:00
- My current primary metrics: Bike FTP (255W), Run LTP (3:51/km), Swim CSS (2:15/100m).
Each of these signify the pace that I have tested that I can hold for an hour in each of these sports.

How to use it: 
1. Open the `.ipynb` file in this repository.
2. Click the **Open in Colab** button at the top (see link below).
3. Input your personal averages and biometrics to generate your own prediction.
