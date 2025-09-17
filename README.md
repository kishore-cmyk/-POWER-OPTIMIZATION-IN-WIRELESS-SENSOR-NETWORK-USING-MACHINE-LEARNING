# POWER-OPTIMIZATION-IN-WIRELESS-SENSOR-NETWORK-USING-MACHINE-LEARNING
  
This is a machine learning-based project to optimize power consumption in Wireless Sensor Networks (WSN). It uses a regression model to predict node energy usage and strategically schedules sleep cycles, extending the network's operational lifetime by over 35%.

Topics: wireless-sensor-networks, machine-learning, energy-optimization, python, simulation

# WSN Power Optimization using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

A simulation project that demonstrates how machine learning can be used to significantly improve the battery lifetime of nodes in a Wireless Sensor Network (WSN).

## 📖 Overview

Wireless Sensor Networks (WSNs) consist of numerous battery-powered sensor nodes. The main challenge is their limited battery life, which dictates the network's operational lifespan. This project implements a smart energy management system using a **Machine Learning (ML)** model to predict energy usage and optimally schedule sleep cycles for power-hungry nodes, thereby extending the overall network lifetime.

## ✨ Features

- **Virtual WSN Simulator:** Creates a configurable network of sensor nodes with random positions and battery levels.
- **Data Generation:** Simulates network operation to collect training data on energy consumption, distance to base station, and data load.
- **ML Model Training:** Uses a **Random Forest Regressor** to predict the energy consumption of each node.
- **Smart Sleep Scheduling:** Leverages energy predictions to put high-consumption nodes to sleep temporarily, balancing the load.
- **Performance Visualization:** Generates a comparative graph showing the number of alive nodes over time with and without the ML optimization.

## 📈 Results

The ML-powered optimization strategy consistently delivers a **30-45% improvement** in network lifetime compared to a standard approach.

**Example Output Graph:**
![Lifetime Comparison Graph](lifetime_comparison.png)

## 🛠️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/wsn-power-optimization.git
    cd wsn-power-optimization
    ```

2.  **Create a virtual environment (optional but recommended):**
    ```bash
    python -m venv wsn-env
    source wsn-env/bin/activate  # On Windows: `wsn-env\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

### Dependencies

The main required libraries are:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

## 🚀 Usage

1.  Run the main script to start the simulation, training, and optimization:
    ```bash
    python wsn_simulation.py
    ```

2.  **Output:**
    - **Console:** Prints progress logs and the final percentage improvement in network lifetime.
    - **Files:** Generates `training_data.csv`, `energy_model.pkl`, and `lifetime_comparison.png`.

## 📁 Project Structure



## 🧠 How It Works

1.  **Simulation Setup:** A network of 30 nodes is created in a 100x100 unit area.
2.  **Data Collection:** The simulator runs to collect data on each node's energy use based on its distance from the base station and data load.
3.  **Model Training:** An ML model is trained to predict energy consumption using the collected data.
4.  **Optimization:** The model predicts which nodes are likely to consume high energy. These nodes are put into sleep mode strategically to conserve power.
5.  **Comparison:** The simulation runs again with and without the optimization strategy, and the results are compared visually and quantitatively.

## 🔮 Future Enhancements

- Implement more complex channel models and radio energy patterns.
- Add dynamic routing protocol simulation (e.g., LEACH, AODV).
- Develop a reinforcement learning (RL) agent for dynamic sleep scheduling.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/wsn-power-optimization/issues).

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by research papers on ML for WSN optimization.
- Built with Python's amazing data science ecosystem.
