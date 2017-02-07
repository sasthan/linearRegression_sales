# reporting_linearRegression_Sales : scikit-learn + pandas

Understanding Linear Regression with scikit-learn and using Sales for the same. 

Reference : 
https://github.com/justmarkham/DAT4/blob/master/notebooks/08_linear_regression.ipynb

## Requirements

Need python installed on computer. 
I used IDLE IDE to run python scripts

### Use interactively with IDLE

```python
>>> import pandas as pd
>>> import matplotlib.pyplot as plt

# read data into dataframe
>>> data = pd.read_csv("Advertising.csv", index_col=0)
>>> data.head()
      TV  Radio  Newspaper  Sales
1  230.1   37.8       69.2   22.1
2   44.5   39.3       45.1   10.4
3   17.2   45.9       69.3    9.3
4  151.5   41.3       58.5   18.5
5  180.8   10.8       58.4   12.9

#print the shape of dataframe
>>> data.shape
(200, 4)

# visualize the relationship between the features and the response using scatterplots
>>> fig, axs = plt.subplots(1,3, sharey=True)
>>> data.plot(kind='scatter',x='TV',y='Sales',ax=axs[0],figsize=(16,8))
<matplotlib.axes._subplots.AxesSubplot object at 0x065CD3D0>
>>> data.plot(kind='scatter', x='Radio', y='Sales', ax=axs[1])
<matplotlib.axes._subplots.AxesSubplot object at 0x06617C10>
>>> data.plot(kind='scatter', x='Newspaper', y='Sales', ax=axs[2])
<matplotlib.axes._subplots.AxesSubplot object at 0x067E5FF0>

>>>import pylab
>>> pylab.show()

```


