# Portfolio Equal Risk Contribution Project  

This project focuses on implementing a **Portfolio Equal Risk Contribution** strategy across a universe of five ETFs: **Momentum**, **Quality**, **Low Volatility**, **Dividend**, and **Value**.  

## Project Structure  

1. **Portfolio Backtesting**:  
   The `PortfolioBacktesting` notebook contains a rolling window, walk-forward backtest to validate the robustness of our approach.  

2. **ETF to Stock Weights**:  
   The `ETF_weights_to_stock_weight` notebook presents the final results after incorporating ESG criteria. It also demonstrates the transition from ETF weights to the corresponding stock-level weights.  

3. **Modular Design**:  
   The project is modular, leveraging reusable functions implemented in the `GeneralFunction` script. These functions include tasks such as stock return calculations, metric derivation from returns, and more.  

## Data Sources  

The data for this project was gathered from the following sources:  
- **Yahoo Finance**: Stock prices  
- **AlphaVantage API**: Financial statements  

The data processing pipeline is available in the following repository:  
[https://github.com/McKingN/Majestic-Equity-Data.git](https://github.com/McKingN/Majestic-Equity-Data.git)  

## Algorithms  

Our algorithms can be reviewed in:  
- `./Smart beta/Backtester.ipynb`  
- `./Smart beta/ETF_weights_to_stock_weight.ipynb`  

## Results  

The final results are compiled in PDF format and can be found in the `Results` directory.  


## Repository Structure

```plaintext
.
├── Smart beta
│   ├── Backtester.ipynb
│   ├── ETF_weights_to_stock_weight.ipynb
│   ├── GeneralFunction.py
│   ├── image.jpg
├── Results
│   ├── Backtester.pdf
│   ├── ETF_weights_to_stock_weight.pdf
├── requirements.txt
├── test.py
└── Readme.md
```

### `Smart beta`

Core scripts and notebooks for backtesting:

- **Backtester.ipynb**: Main notebook for backtesting smart beta strategies.
- **ETF_weights_to_stock_weight.ipynb**: Notebook for converting ETF weights to individual stock weights.
- **GeneralFunction.py**: Contains utility functions used across the project.
- **image.jpg**: Placeholder or illustrative image for strategy visualization.

### Project Files

- **`requirements.txt`**: Lists the Python dependencies required for the project. Use a virtual environment (e.g., `venv`) to install dependencies:
  ```bash
  python -m venv venv
  source venv/bin/activate # On Windows: venv\Scripts\activate
  pip install -r requirements.txt
  ```


### Version Control

The project uses Git for version control. The `.git` directory contains configuration and history information for the repository.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Team-CKLLZ/Portfolio-Equal-Risk-Contribution.git
   cd Portfolio-Equal-Risk-Contribution
   ```

2. Set up the virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Run the backtesting scripts:
   - Open `Backtester.ipynb` in your preferred Jupyter environment or convert it to a Python script if needed:
     ```bash
     jupyter notebook Backtester.ipynb
     ```



## Notes

- The `.DS_Store` file and `.git` directory are ignored from the project and should not be manually modified.
- Ensure data integrity when modifying files in the `data` directory, as these are crucial for accurate backtesting results.

## License

This project is licensed under the MIT License. See `LICENSE` for more details.

## Contributing

Contributions are welcome! Please follow the guidelines in `CONTRIBUTING.md` (if available).
