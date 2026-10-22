# 🧠 Spectral Analysis and Filtering of Neural Data

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![Data Science](https://img.shields.io/badge/Data_Processing-Signal_Analysis-success?style=for-the-badge)

> Dive into the fascinating world of neural signal processing! 🧬 
> This repository showcases a comprehensive analysis of neural data and spike trains, demonstrating core data science concepts like the Sampling Theorem, Noise Reduction, and advanced Spike Train Analysis.

**👩‍💻 Author:** Dana Sela

---

## 📊 Datasets

We explore the hidden patterns within two primary datasets:

* 🔬 **`Neural_data.csv`**: Continuous neural signals capturing Calcium imaging fluorescence changes (ΔF/F (%)). 
* ⚡ **`spike_trains.csv`**: Binary spike train records tracking the firing activity of multiple neurons (Neurons A through E) across various experimental trials.

---

## ✨ Project Highlights

The project is structured into three exciting analytical phases:

### 📉 Part 1: The Sampling Theorem 
*(Nyquist Frequency, Aliasing, and Quantization)*
* **Signal Exploration:** Peering into specific windows of the neural signal, contrasting the quiet noise period (0-9s) with the active stimulus period (12-30s).
* **The Aliasing Effect:** Manually downsampling a 50 Hz stimulus signal to 25 Hz, 10 Hz, and 3.33 Hz to vividly illustrate what happens when we ignore the Nyquist rate!

### 🧹 Part 2: Noise Reduction Strategies
* **SNR Evaluation:** Calculating the true Signal-to-Noise Ratio ($SNR_{rms}$) to quantify data quality.
* **Moving Averages:** Cleaning up the signal! We apply moving averages (windows of 2, 3, 5, and 20 points) and compare the real-world SNR gains against theoretical models.
* **Kernel Smoothing:** Experimenting with specialized techniques like double-rectangular and 5-point triangular kernels for optimal signal smoothing.

### 🧠 Part 3: Spike Train & Correlation Analysis
* **Firing Dynamics:** Computing the mean firing rate (Hz) to understand baseline neuron activity.
* **Fano Factor:** Measuring the wild variability of spike counts within 1-second windows.
* **ISI Distributions:** Visualizing Inter-Spike Interval (ISI) histograms to uncover the rhythmic timing between spikes.
* **Visualizing Activity:** 
  * **Raster Plots:** Beautifully mapping out spike occurrences across multiple trials.
  * **PSTH Plots:** Creating Peri-Stimulus Time Histograms to track average firing rates over time.
* **Autocorrelation:** Finding hidden repeating patterns within the neural activity.

---

## 🛠️ Tech Stack

This project is built using the ultimate Python data science toolkit:

* 🐍 **Python 3** - The core engine.
* 🐼 **Pandas** - For seamless data wrangling and manipulation.
* 🔢 **NumPy** - Powering complex numerical computations.
* 🔬 **SciPy** - Handling the heavy lifting of advanced signal processing.
* 📈 **Matplotlib** - Crafting beautiful, publication-ready visualizations.

---

## 🚀 Getting Started

Want to run this analysis on your own machine? Follow these simple steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. **Install dependencies:**
   Make sure you have all the required libraries ready to go:
   ```bash
   pip install pandas numpy scipy matplotlib
   ```
3. **Set up your data:**
   Verify that `Neural_data.csv` and `spike_trains.csv` are in the correct directory as referenced in the notebook.
4. **Run the magic:**
   Fire up Jupyter Notebook and run the cells to reproduce the plots and analysis!
   ```bash
   jupyter notebook
   ```

---
*If you find this project interesting, feel free to ⭐ star the repository!*