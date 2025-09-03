# SSCM-CAI-Framework

## Cultural Integration for Sustainable Supply Chain Management in Emerging Markets

This repository contains data and code for the paper "Cultural Integration for Sustainable Supply Chain Management in Emerging Markets: Framework Development and Empirical Validation Using Public Data" published in Sustainability Journal.

### 📊 Repository Overview

This repository provides all necessary materials to replicate our Cultural Affinity Index (CAI) calculations and empirical analyses examining the relationship between cultural factors and sustainable supply chain management performance in Southeast Asia.

### 👥 Authors

- **Tsai Hsin Jiang** - Department of Industrial Engineering and Management, National Yang Ming Chiao Tung University
  - Email: three.c@nycu.edu.tw
  - ORCID: [0000-0000-0000-0000]
  
- **Yung Chia Chang** - Department of Industrial Engineering and Management, National Yang Ming Chiao Tung University
  - Email: jasmine.chang@g2.nctu.edu.tw

### 📁 Repository Structure

```
SSCM-CAI-Framework/
├── data/                  # Processed datasets
│   ├── cai_scores_2019_2023.csv
│   ├── country_pairs_analysis.csv
│   └── performance_indicators.csv
├── scripts/               # Analysis scripts
│   ├── 01_data_extraction.py
│   ├── 02_cai_calculation.py
│   ├── 03_statistical_analysis.R
│   ├── 04_optimization_model.py
│   └── 05_visualization.py
├── results/               # Generated outputs
│   ├── figures/
│   └── tables/
└── documentation/         # Additional documentation
```

### 🔧 Requirements

#### Python (3.8+)
```bash
pandas==1.5.3
numpy==1.24.3
scipy==1.10.1
matplotlib==3.7.1
seaborn==0.12.2
scikit-learn==1.2.2
```

#### R (4.0+)
```r
tidyverse
lme4
car
stargazer
```

### 💻 Installation & Usage

1. **Clone the repository**
```bash
git clone https://github.com/[your-username]/SSCM-CAI-Framework.git
cd SSCM-CAI-Framework
```

2. **Install Python dependencies**
```bash
pip install -r requirements.txt
```

3. **Run the analysis pipeline**
```bash
# Calculate CAI scores
python scripts/02_cai_calculation.py

# Generate visualizations
python scripts/05_visualization.py

# Run statistical analysis (in R)
Rscript scripts/03_statistical_analysis.R
```

### 📊 Data Sources

Our analysis uses publicly available data from:

- **UN COMTRADE**: https://comtrade.un.org
  - Bilateral trade volumes and partner networks
- **World Bank Open Data**: https://data.worldbank.org
  - GDP, population, and development indicators
- **World Governance Indicators**: https://info.worldbank.org/governance/wgi/
  - Institutional quality measures
- **Hofstede Insights**: https://www.hofstede-insights.com
  - National cultural dimensions
- **ILO Statistics**: https://ilostat.ilo.org
  - Labor and employment indicators
- **Environmental Performance Index**: https://epi.yale.edu
  - Environmental sustainability metrics

### 📈 Key Results

- **850 supplier-manufacturer dyads** analyzed across 5 Southeast Asian countries
- High cultural affinity (CAI > 0.7) associated with:
  - 18.0% improvement in economic performance
  - 12.0% enhancement in environmental compliance
  - 32.0% increase in social sustainability
- Interaction effects between language compatibility and regional trust (γ = 0.15, p < 0.01)
- Stronger CAI effects in weaker institutional environments (correlation = -0.92)

### 🔬 Methodology

The Cultural Affinity Index (CAI) comprises four components:

1. **Language Compatibility (LC)**: 25% weight
2. **Regional Trust (RT)**: 30% weight
3. **Trade Networks (TN)**: 25% weight
4. **Historical Trade (HT)**: 20% weight

Including interaction effects:
```
CAI = w₁LC + w₂RT + w₃TN + w₄HT + γ(LC × RT)
```

### 📝 Citation

If you use this data or code in your research, please cite:

```bibtex
@article{jiang2025cultural,
  title={Cultural Integration for Sustainable Supply Chain Management in Emerging Markets: Framework Development and Empirical Validation Using Public Data},
  author={Jiang, Tsai Hsin and Chang, Yung Chia},
  journal={Sustainability},
  volume={17},
  number={X},
  pages={XXX},
  year={2025},
  publisher={MDPI}
}
```

### 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### 🤝 Contributing

We welcome contributions! Please feel free to:
- Report bugs or issues
- Suggest enhancements
- Submit pull requests
- Share your extensions of the framework

### 📧 Contact

For questions or collaborations, please contact:
- **Corresponding Author**: Tsai Hsin Jiang (three.c@nycu.edu.tw)

### 🙏 Acknowledgments

We thank the United Nations, World Bank, and other organizations for maintaining comprehensive public databases that made this research possible.

### ⚠️ Disclaimer

The findings and opinions expressed in this repository are those of the authors and do not necessarily reflect the views of the affiliated institutions or data providers.

---

