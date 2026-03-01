# Hybrid-Load-Balancer-using-Soft-Computing-Techniques
# 🚀 Proactive Intelligent Load Balancer: ANN-Fuzzy-GA Hybrid

An advanced soft-computing project that replaces traditional "blind" load balancing with an intelligent, predictive, and adaptive system. This prototype demonstrates a **32.9% efficiency improvement** over standard Round Robin algorithms during extreme traffic surges.



## 📌 The Problem
Standard load balancers (Round Robin, Least Connections) are fundamentally **static and reactive**. They treat all servers equally regardless of speed (Heterogeneity) and only respond to traffic spikes *after* they occur. This leads to server saturation, high latency, and system crashes during "Flash Crowd" events.

## 💡 The Solution: A Hybrid Soft-Computing Brain
This system utilizes a three-tier intelligent architecture:
1. **Artificial Neural Network (ANN):** Acts as the "Forecaster" by analyzing historical logs to predict upcoming traffic trends.
2. **Fuzzy Logic Controller (FLC):** Acts as the "Decision Maker." It evaluates predicted trends and real-time server health to route tasks with human-like nuance.
3. **Genetic Algorithm (GA):** Acts as the "Optimizer" to evolve the fuzzy rules for maximum efficiency.

## 📊 Experimental Results

### Normal Traffic vs. Stress Test
We benchmarked the Hybrid AI against traditional methods using both standard and "Stress" datasets (500% traffic spikes).

| Method | Total Processing Time (Stress) | Performance Gain |
| :--- | :--- | :--- |
| **Round Robin** | 16,133.40s | Baseline |
| **Weighted RR** | 13,872.80s | +14.0% |
| **Hybrid AI (Ours)** | **10,825.30s** | **+32.9%** |



### Key Finding: 
During peak stress, the AI prioritized the high-speed node (**Server 1**), handling **16,845 tasks** successfully, while traditional methods bottlenecked on slower nodes.



## 🛠️ Project Structure
* `main.py`: The core simulation runner (AI-driven).
* `generate_stress.py`: Generates the "Flash Crowd" traffic dataset.
* `baselines.py`: Logic for RR, WRR, and Least Connection comparisons.
* `visualize_all.py`: Generates comparative performance graphs.
* `summary_stats.py`: Calculates and prints efficiency metrics.
* `src/`: Contains the ANN and Fuzzy Logic logic modules.

## 🚀 Getting Started

1. **Clone the repo & setup environment:**
   ```bash
   python -m venv lb_env
   source lb_env/bin/activate  # Or lb_env\Scripts\activate on Windows
   pip install -r requirements.txt
Generate Traffic Data:

Bash
python generate_stress.py
Run the Simulation:

Bash
python main.py
Compare Results:

Bash
python summary_stats.py
python visualize_all.py
🏆 Conclusion
By shifting from reactive distribution to proactive anticipation, this model maximizes hardware utilization and significantly reduces processing time, proving that Soft Computing is a superior approach for modern, high-load cloud architectures.
