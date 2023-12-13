
<img src="https://github.com/agujalwar/Analyzing-Insights-for-Environmental-Monitoring-Using-Python-MySQL/assets/125154280/e65bc56d-c5f2-4f28-9db4-1cfcdf6b7c85" width="600" height="400">


## Analyzing-Insights-for-Environmental-Monitoring-Using-Python-MySQL
* Conducted in-depth analysis on a real-world Environmental Monitoring database, scrutinizing diverse data including timestamp, carbon monoxide, humidity,light, liquefied petroleum gas, motion, smoke, and temperature for corresponding devices.
* Utilized Python pandas library for robust data preprocessing, effectively handling duplicate records, null values, and implementing necessary data type changes to ensure data integrity.
* Applied MySQL for extracting valuable insights from the database, including the identification of the highest recorded temperature for each device and calculating the exponential moving average (EMA) of temperature.
* Implemented data-driven analysis techniques to identify devices experiencing sudden changes in humidity, showcasing a keen ability to draw meaningful conclusions from complex datasets.
### Module 1: Data preprocessing
  1.Reading the Data from CSV
  2.Renaming the columns
  3.Checking for Null Values
  4.Removing duplicates
  5.Handling Missing Values
  6.Data Type Conversion
  7.Exporting the cleaned Dataset
  8.Generate the Database table using cleaned Dataset
### Module 2: Data Analysis using MySQL
  1.  The task is to calculate the average temperature recorded for each device in the dataset.
  2.  This task involves identifying the devices with the highest average carbon monoxide levels and retrieving the top 5 devices based on this metric.
  3.  The objective is to Determine the average temperature recorded in the cleaned_environment dataset.
  4.  This task requires identifying the highest recorded temperature for each device and retrieving the corresponding timestamp and temperature values.
  5.  The goal is to Identify devices where the temperature has increased from the minimum recorded temperature to the maximum recorded temperature
  6.  Calculate the exponential moving average (EMA) of the temperature for each device. Retrieve the device ID, timestamp, temperature, and the EMA temperature for the first 10 devices from the 'cleaned_environment' table. The EMA temperature is calculated by partitioning the data based on the device ID, ordering it by the timestamp, and considering all preceding rows up to the current row
  7.  The objective is to identify the timestamps and devices where the carbon monoxide level exceeds the average carbon monoxide level across all devices.
  8.  The objective is to identify the devices that have recorded the highest average temperature among all the devices in the dataset.
  9.  The goal is to calculate the average temperature for each hour of the day, considering data from all devices.
  10. The objective is to identify device(s) in the cleaned environment dataset have recorded only a single distinct temperature value.
  11. The objective is to identify the devices that have recorded the highest humidity levels.
  12. This task requires calculating the average temperature for each device while excluding outliers, which are temperatures beyond 3 standard deviations from the mean.
  13. The goal is to identify devices that have undergone a sudden change in humidity, where the difference is greater than 50%, within a 30-minute time window.
  
  15. This task involves calculating the average temperature for each device separately for weekdays and weekends.
  16. Calculate the cumulative sum of temperature for each device, ordered by timestamp limit to 10.
The objective is to calculate the cumulative sum of temperature for each device, considering the records ordered by timestamp limit to 10
Hint:
To calculate the cumulative temperature for each device in the "cleaned_environment" dataset, you'll need to use the SUM function with the OVER clause. Remember to partition the SUM function by the device_id column to perform the calculation separately for each device. Also, ensure that the temperatures are ordered by the timestamp column. Finally, assign the calculated cumulative temperature to a new column named "cumulative_temperature." Don't forget to limit the results to the first 10 records using the LIMIT clause. This will allow you to observe the device_id, timestamp, temperature, and cumulative_temperature values for each device. 


## Project link
https://hicounselor.com/projects/analyzing-insights-for-environmental-monitoring-using-python-mysql
