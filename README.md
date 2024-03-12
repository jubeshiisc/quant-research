# quant-research
A quant research

General Assumptions:

For the Z-Score Trading System:
Stationarity: The model assumes that the spread between Bank Nifty IV and Nifty IV is stationary over the period considered. Stationarity means that the statistical properties of the spread (mean, variance) do not change over time.

Mean Reversion: The strategy is based on the assumption that the spread exhibits mean-reverting behavior. This means if the spread deviates significantly from its historical average (as indicated by the z-score), it is expected to revert back to the mean over time.

Overfitting Control: The model assumes that measures such as splitting data into training and testing sets, along with the inherent randomness in Random Forest, help mitigate overfitting.

Summary of Results and Findings

The base model utilized the z-score of the IV spread between Bank Nifty and Nifty to generate trading signals. Trades were executed when the z-score exceeded predetermined thresholds, indicating a significant deviation from the mean.

The advanced model incorporated additional features, such as lagged values of the spread and historical z-scores, to predict trading signals using a Random Forest classifier.

Findings:

Both models confirmed the initial hypothesis that the IVs of Bank Nifty and Nifty are influenced by similar factors, allowing for profitable pairs trading opportunities.
The advanced model provided a more robust framework for capturing dispersion between the indices, although it required careful tuning and validation to avoid overfitting.
The analysis highlighted the importance of considering transaction costs and market impact, as these factors significantly affect the net profitability of the strategy.
