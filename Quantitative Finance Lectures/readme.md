# Quantitative Finance Lectures

Here you will find a set of notebooks to help get started with implementing some basic quantitative strategies described in the academic literature of factors and commonly employed in practice. You can see these notebooks as a follow up on our Python Lectures covering fundamentals of the Python programming language.

## Trackers

Financial time series are the "atoms" of quantitative finance. Hence, it is important that these financial time series realistically reflect the cumulative **total returns** of those asssets and not simply their prices over time. Total return is the actual rate of return of a position, portfolios or strategy over a given evaluation period, typically a business day. Total return of an asset has to include interest gained or paid when holding the position, capital gains coming from price or exchange rate variations in the period as well as dividends, coupons, borrow costs, and other distributions or payments realized over the period of time the asset was held. For example, check out our Jupyter Notebook on how to create a financial time series for trading [currencies](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/creating_fx_time_series_fh.ipynb), [futures](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/rolling_futures_time_series.ipynb), and [interest rates swaps](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/swap_historical_returns.ipynb)!

## Signals

We use financial time series to generate trading signals. There are many of them, using simple as well as complex modeling techniques. Check out our notebook on [Classic Momentum Signals](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/time_series_momentum.ipynb) as well as on [Carry Signals](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/carry.ipynb)

## Pricing

Sometimes constructing these financial time series can be very difficult as the valuation of the underlying instruments can be a very challenging thing to do based on pulically available data. Check out our notebook that shows how to price and calculate the returns of a plain-vanilla interest rate swap [here](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/interest_rate_swaps.ipynb)

## Machine learning

While our focus is on basic quantitative strategies described in the academic literature of factors and commonly employed in practice, we do give some examples of more sophisticated models. For example, check out or example here for using AWS SageMaker for training, validating, and testing a regression tree model to predict future returns of financial time series based on momentum signals [here](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/momentum_with_regression_trees.ipynb)! Also, check out the notebook where we use [PCA to construct portfolios](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/PCA_based_portfolios.ipynb) and [clustering algos](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/fx_pca_case.ipynb) to decide which currencies to trade against each other.

## BQuant and Bloomberg Query Language
Bloomberg is developing a new function in the Terminal, called BQuant, BQNT, under the Bloomberg Anywhere license. Basically, if you type BQNT<GO> on a Bloomberg Terminal, provided you have the license, a JupyterLab type of environment will pop up allowing you to run Jupyter notebooks inside a Bloomberg Terminal. One of the reason that this is such a great idea is that now we can use Jupyter notebook with Bloomberg data pulled into the notebook using a data retrieval interface called Bloomberg Query Language, or BQL.
    
BQL works a lot like SQL. You submit a query request to Bloomberg’s server and get the data directly from server, which also enables basic calculations so as to further reduce the size of data being pulled out. Also, BQNT comes with pre-installed bqplot and some wrappers of libraries like ipwidgets, which makes visualization easy and interactive. Check out our example that use BQNT, BQL, and [K-Means Clustering for stock picking](https://github.com/Finance-Hub/FinanceHubMaterials/blob/master/Quantitative%20Finance%20Lectures/kmeans_clusters_factors.ipynb)
