# Exploring the Potential of Hoeffding Trees with Change Point Detection Employment for Multistep Natural Gas Consumption Forecasting in Continual Learning Scenarios

Forecasting natural gas consumption, considering seasonality and trends, is crucial in planning its supply and consumption and optimizing the cost of obtaining it, mainly by industrial entities. However, in times of threats to its supply, it is also a critical element that guarantees the supply of this raw material to meet individual consumers' needs, ensuring society's energy security.

This paper aims to propose and evaluate two novel approaches, Pure and Mixed, for multistep forecasting of natural gas consumption based on change point detection and model aggregation. We design a general methodology for multistep multivariate time series forecasting with continual learning capabilities using data stream processing. The performance of the defined change point divided model collection approaches is compared with two baseline approaches. We use three metrics and three settings of the PELT algorithm to measure the forecasting error and the effect of the number of change points. Our experiments show that the defined Pure approach outperforms all other approaches by each selected metric and for all tested parameter settings. We also demonstrate that fewer change points result in a lower error and that the Pure approach is more robust and suitable for continual learning tasks. We present the potential of our methodology for forecasting natural gas consumption in a dynamic and complex environment and suggest future work.

## Jupyter notebooks
* Reuired packages are in the *requirements.txt*, experiments were conducted in Jupyter notebooks in the repository.

* PELT setting for *Low, Medium and High* are controlled by variables **LOW, MED, HIGH** for the PELT penalization factor in the notebooks, just change the multiplicator in the penalization variables, e.g. for *LOW* it is *pen = cp_params[model][47]*LOW*.

These notebooks contains source codes for the experiments:
* *NGC_HT_Day2Day_Online.ipynb*: SMCA
* *NGC_HT_Day2Day_BySeason_2021*: QDMDC
* *NGC_HT_Day2Day_ByCP_2021.ipynb*: PCPDMC
* *NGC_HT_Day2Day_ByCP_ERR_Switch_2021.ipynb*: MCPDMC-SW
* *NGC_HT_Day2Day_ByCP_ERR_WAVG_2021.ipynb*: MCPDMC-WA