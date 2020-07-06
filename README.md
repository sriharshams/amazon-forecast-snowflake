# Amazon Forecast with Snowflake

- End to end example of Amazon Forecast using Snowflake.
- Note that it follows [amazon-forecast-samples](https://github.com/aws-samples/amazon-forecast-samples/tree/master/notebooks/advanced/Incorporating_Related_Time_Series_dataset_to_your_Predictor)
  - Uses simulated Snowflake as initial data store to for the source data
  - After data transformation as needed by Amazon Forecast, data is updated back to Snowflake data store
  - Unload data from Snowflake to S3 and import dataset to Amazon Forecast, build predictor and forecast
  - Export Forecast Query and load it to Snowflake data store.



### Install

I recommend install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.

Once you have Anacoda installed, create a new conda env. 
In below command replace myenv with your preferred env name

```bash
conda create -n myenv python=3.6
```

once you create myenv, activate it

```bash
conda activate myenv 
```



This use case requires **Python 3.6** and the following Python libraries installed:

- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html)
- [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector.html)



### Code

Code is provided in the `Incorporating_Related_Time_Series_dataset_to_your_Predictor.ipynb` notebook file. Some utility code is present in util folder.

### Snowflale Connection Details

Env file is present in `env/dev/credentials` file, this file shold contain snowflake connection and aws credentials as a dictionary.

### Run

In a terminal or command window, navigate to the directory `advanced/Incorporating_Related_Time_Series_dataset_to_your_Predictor/` and run one of the following commands:


```bash
jupyter notebook Incorporating_Related_Time_Series_dataset_to_your_Predictor.ipynb
```

This will open the iPython Notebook software and use case file in your browser.

