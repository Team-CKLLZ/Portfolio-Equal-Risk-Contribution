# Portfolio Equal Risk Contribution Project

We are setting up a portoflio Equal Risk Contribution on a universe of 5 ETFs: Momentum, Quality, Low_vol, Dividend and Value.

The first part is recorded in the portoflioBacktesting notebook, where we carry out a rolling window walk forward backtest to demonstrate the soundness of our approach.

The second part (the ETF_weights_to_stock_weight notebook) presents our final results after taking into account the various ESG criteria. We also show how we can move from ETF weights to the weight of the stocks contained in the ETFs.

To make our project modular, we have implemented functions to generate tasks such as stock return calculation, metric calculation from return and many others in the GeneralFunction script.

## Repository Structure

```plaintext
.
├── Smart beta
│   ├── Backtester.ipynb
│   ├── ETF_weights_to_stock_weight.ipynb
│   ├── GeneralFunction.py
│   ├── image.jpg
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
