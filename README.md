# ⚡ Electricity Demand Forecasting with LSTM & SARSA

This project explores hybrid approaches for forecasting electricity demand using:
- Deep Learning (LSTM) to capture sequential patterns in time-series data  
- Reinforcement Learning (SARSA) to optimize decision-making policies based on forecasts  

---

## 📌 Overview / Motivation
Accurate electricity demand forecasting is crucial for:
- Ensuring grid stability  
- Reducing costs from over/under-supply  
- Enabling better renewable energy integration  

While LSTM provides reliable short-term forecasts, SARSA introduces an adaptive reinforcement learning agent that learns how to optimize energy management strategies from demand predictions. Together, they provide both prediction and decision optimization.

---

## 🛠️ Tech Stack / Dependencies
- Python 3.8+
- Libraries:
  - `pandas`, `numpy` → Data preprocessing
  - `matplotlib`, `seaborn` → Visualization
  - `scikit-learn` → Scaling, splitting data
  - `keras` / `tensorflow` → Deep Learning (LSTM)
  - Custom implementation of SARSA algorithm  

You can install dependencies via:
pip install -r requirements.txt

## Dataset
The dataset used (continuous dataset.csv) contains:
  - T2M_toc → Temperature (Tocumen city)
  - QV2M_toc → Humidity
  - TQL_toc → Total liquid water
  - W2M_toc → Wind speed
  - T2M_san → Temperature (Santiago city)
  - nat_demand → Target variable: National electricity demand


## Project Structure
- DL.ipynb                 # Jupyter Notebook (LSTM + SARSA implementation)
- continuous dataset.csv    # Dataset (not included in repo)
- requirements.txt          # Python dependencies
- README.md                 # Project documentation

## How to Run
1. Clone the repository
  - git clone https://github.com/Khushipatel27/Electricity-Demand-Forecasting-with-LSTM-SARSA.git
  - cd electricity-demand-lstm-sarsa

2. Install dependencies
  - pip install -r requirements.txt

3. Run the notebook
  - jupyter notebook DL.ipynb

Follow the notebook to:
  1.Preprocess the dataset
  2.Train and evaluate the LSTM model
  3.Train and test the SARSA agent

## Results
- Forecasts future electricity demand from historical weather & demand data
- Visualization of actual vs. predicted demand

<img width="2800" height="1487" alt="image" src="https://github.com/user-attachments/assets/f8d4b769-f000-4733-927e-980137c398e9" />


<img width="2794" height="1398" alt="image" src="https://github.com/user-attachments/assets/151cb3c2-6479-47d9-8a2b-116c661000a4" />


<img width="2798" height="1194" alt="image" src="https://github.com/user-attachments/assets/1d03a248-7dcc-43c9-ad7d-cbb30e43a123" />

## Future Work
  - Hyperparameter tuning (LSTM layers, SARSA learning rate, epsilon decay)
  - Compare with other RL algorithms (Q-learning, DQN)
  - Include seasonal and holiday effects
  - Deploy as a Flask/Django API or interactive dashboard

## Contributing
Contributions are welcome!
If you'd like to improve this project:
  1. Fork the repo
  2. Create your feature branch (git checkout -b feature-name)
  3. Commit your changes (git commit -m 'Add feature')
  4. Push to the branch (git push origin feature-name)
  5. Open a Pull Request


  




