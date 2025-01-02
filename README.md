# dstbn-prob: A Tool for Distribution Probability

[![PyPI version](https://badge.fury.io/py/dstbn-prob.svg)](https://pypi.org/project/dstbn-prob/)  [![Python version](https://img.shields.io/badge/python-3.6%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)


The Distribution Probability `dstbn-prob` is a Python package designed for calculating, analyzing, and visualizing probability distributions. With support for both **Gaussian** and **Binomial** distributions, the package offers intuitive methods for computing statistical properties, probability functions, and creating visualizations. It is an ideal tool for data analysis, statistics, and probability studies.

---

## ✨ Features
  
- **General Distribution:**
  - Read data from a file and calculate basic statistical properties.
  
- **Gaussian Distribution:**
  - Compute mean and standard deviation.
  - Evaluate the probability density function (PDF).
  - Visualize data with histograms and PDF plots.
  - Combine two Gaussian distributions.

- **Binomial Distribution:**
  - Compute mean and standard deviation.
  - Visualize data with bar charts.
  - Evaluate probabilities for specific outcomes.
  - Plot the probability distribution (bar chart).
  - Combine two Binomial distributions with the same probability.

---

## 📦 Installation

To install the package, use pip:

```bash
pip install dstbn-prob
```
Ensure you have the `matplotlib` library installed for visualization. If not, install it:

```bash
pip install matplotlib
```

---

## 🚀 Usage

Below is a quick guide to get started with **`dstbn-prob`**.


### Importing Classes
You can directly import classes from the package as follows:

```python
from dstbn_prob import Gaussian, Binomial, Distribution
```

### 1. General Distribution

```python
from dstbn_prob import Distribution

# Create a general distribution and load data
dist = Distribution()
dist.read_data_file('data.txt')  # Ensure data.txt contains one number per line

print(dist.data)  # Access the loaded data
```

### 2. Gaussian Distribution

```python
from dstbn_prob import Gaussian

# Create a Gaussian distribution
gaussian = Gaussian(mu=10, sigma=5)

# Calculate mean and standard deviation
gaussian.calculate_mean()
gaussian.calculate_stdev()

# Plot histogram and PDF
gaussian.plot_histogram()
gaussian.plot_histogram_pdf()
```

### 3. Binomial Distribution

```python
from dstbn_prob import Binomial

# Create a Binomial distribution
binomial = Binomial(prob=0.4, size=50)

# Calculate mean and standard deviation
binomial.calculate_mean()
binomial.calculate_stdev()

# Plot bar chart and probability distribution
binomial.plot_bar()
binomial.plot_bar_pdf()
```

### Combining Distributions

- **Gaussian Distribution**:

```python
from dstbn_prob import Gaussian

gaussian1 = Gaussian(mu=10, sigma=5)
gaussian2 = Gaussian(mu=20, sigma=7)

result = gaussian1 + gaussian2
print(result)  # mean: 30, standard deviation: ~8.602
```

- **Binomial Distribution**:

```python
from dstbn_prob import Binomial

binomial1 = Binomial(prob=0.5, size=30)
binomial2 = Binomial(prob=0.5, size=20)

result = binomial1 + binomial2
print(result)  # mean: 25.0, standard deviation: ~3.535
```

---

## 🛠️ Development and Contribution

### Local Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/NidaIslam/Distribution_probablility_package.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Distribution_probablility_package
   ```



**Contributing**

Contributions are welcome! Please follow these steps:

- Fork the repository.
- Create a new branch for your feature or bug fix.
- Submit a pull request with a clear description of your changes.

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](dstbn_prob/license.txt) file for details.


## 🌟 Acknowledgments

- [Matplotlib](https://matplotlib.org/) for visualization support.
- Python standard libraries for mathematical operations.



## 📫 Contact

For any inquiries or feedback, please open an issue on the [GitHub repository](https://github.com/NidaIslam/Distribution_probablility_package) or reach out via [LinkedIn](https://www.linkedin.com/in/nidaislam10)

