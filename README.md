## 🚚 Dynamic Pricing & Compensation Optimization for Crowd-Shipping Platforms  
**Integrating matching, routing, and pricing into one powerful optimization model**

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Gurobi](https://img.shields.io/badge/Gurobi-MILP-EA1C24?style=flat-square)](https://www.gurobi.com/)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rim-the-optimizer/Pricing/blob/main/pricing.ipynb)

---

### 🧠 Project Summary

This project adapts a powerful **Mixed Integer Linear Program (MILP)** originally developed by *Tho V. Le, Satish V. Ukkusuri, Jiawei Xue, and Tom Van Woensel*, which integrates:

- ✅ **Driver-to-order matching**  
- 🚛 **Route construction**  
- 💰 **Compensation calculation**  
- 💸 **Dynamic customer pricing**

into one **profit-maximizing optimization model** for crowd-shipping platforms.

---

### 📌 Key Features

| ✔ Feature | 💬 Description | 🛠 Customization |
|----------|----------------|----------|
| 🔗 Based on [this research paper](https://www.sciencedirect.com/science/article/pii/S1366554520308516) | The [original MILP model](https://www.github.com/rim-the-optimizer/Pricing/blob/main/pricingmodel_0.ipynb) was created for joint pricing and routing decisions | There is a full description of the functionality of the original MILP model |
| 🧑‍💻 Fully implemented in Python | Adapted to work smoothly in Python using Gurobi | check the [adapted version](https://www.github.com/rim-the-optimizer/Pricing/blob/main/pricingmodel.ipynb) |
| 📊 Highly configurable | Input data, cost structures, and constraints can be adjusted | see in [data description](https://github.com/rimchmielowitz/Pricing/blob/main/data_Berlin/data_description.md) how the [data](https://github.com/rimchmielowitz/Pricing/blob/main/data_Berlin/TWD.csv) is structured |
| 🧪 Ready-to-run notebook | Works in [Google Colab](https://colab.research.google.com/github/rim-the-optimizer/Pricing/blob/main/pricing.ipynb) without local setup |
| 🎯 Focus on profit maximization | Balancing driver payouts with competitive customer pricing |

---

### 📂 Project Structure

| File | Purpose |
|------|---------|
| [`pricingmodel_0.ipynb`](https://github.com/rim-the-optimizer/Pricing/blob/main/pricingmodel_0.ipynb) | Original model implementation |
| [`pricingmodel.ipynb`](https://github.com/rim-the-optimizer/Pricing/blob/main/pricingmodel.ipynb) | My refactored Python version, compatible with Gurobi |
| [`pricing.ipynb`](https://colab.research.google.com/github/rim-the-optimizer/Pricing/blob/main/pricing.ipynb) | Interactive example with documentation and output |

---

### 🚀 Run It Now

Curious to try it out? Open the full demo notebook in Google Colab and experiment with your own parameters:

👉 **[Launch the Notebook in Colab](https://colab.research.google.com/github/rim-the-optimizer/Pricing/blob/main/pricing.ipynb)**

---

### 📸 Screenshots & Output Overview

Here's what you'll see when you run the model:

#### ✔️ Optimized assignments & pricing
![optimized_output](https://github.com/rim-the-optimizer/Pricing/assets/your-image-folder/output_table_example.png)

#### 📈 Gurobi optimization log
![gurobi_log](https://github.com/rim-the-optimizer/Pricing/assets/your-image-folder/gurobi_log.png)

> *(Make sure to replace the image URLs with the actual paths in your repo or a GitHub-hosted folder.)*

---

### 🧮 Model Overview

The MILP model combines multiple decision layers:

#### 1️⃣ **Matching**  
Assign each available delivery task to the most suitable driver, considering feasibility, availability, and cost.

#### 2️⃣ **Routing**  
Construct delivery routes by optimizing task sequences per driver — minimizing time, distance, or cost.

#### 3️⃣ **Compensation**  
Calculate fair driver payments based on delivery effort, distance, time windows, and route difficulty.

#### 4️⃣ **Pricing**  
Set customer prices dynamically — ensuring competitiveness and profitability while covering compensation and platform margin.

#### 🎯 Objective  
Maximize the total platform profit:  
\[
\text{Profit} = \text{Customer Revenue} - \text{Driver Compensation} - \text{Operational Costs}
\]

> The result: a mathematically balanced system where every delivery is **profitable**, **efficient**, and **fair**.

---

### 🛠 Technologies Used

- Python 🐍  
- Gurobi Optimizer 🔧  
- Jupyter Notebooks 📓  
- Linear & Integer Optimization 📈  
- Logistics & Pricing Algorithms 🚚  

---

### 💡 Potential Use Cases

- Last-mile delivery platforms  
- Crowdsourced logistics optimization  
- Smart pricing algorithms for marketplaces  
- Simulation of cost/revenue trade-offs  
