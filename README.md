# CO2-Levels-Analysis-and-Forecasting
The dataset contains CO2 ppm from March 1958 to September 2018. PPM (Parts Per Million)  is a measure of the concentration of a substance in a solution or gas. It indicates the number of parts of a particular substance per one million parts of the total solution or gas. It's a way to express small quantities of substances in a larger mixture.

In air quality ppm is the number of molecules of CO2 per million air molecules. Because indoor air quality has generated more and more awareness, individuals continue to use CO2 detectors to monitor their airflow. 

The fresh air we inhale will typically have about 400ppm of background CO2 with the life-sustaining oxygen of the atmosphere. By measuring your indoor air quality and CO2 ppm levels you can further mitigate airborne illnesses, and lack of productivity, and create a healthier lifestyle.

# 1- CO2 ppm Levels from 1958 to 2018:
![CO2 Levels from 1958 to 2018](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/483e59c2-a9f4-4499-86b0-e4db71236e0a)

# 2- Monthly Average CO2 ppm Levels:
![Monthly Average CO2 Levels](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/328dd040-f20c-4113-b89c-06732cba1c75)

# 3- The Data Decomposition Values (Trend & Seasonality):
![CO2 Levels Decomposition](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/58eb7bac-c2b2-44e5-a5f8-3c4f91b0eef8)

# 4- Finding the Lowest AIC & BIC:
I looped from 1 to 10 to find the best combination of P and Q that achieves the lowest AIC. Where:
P is the order of the autoregressive model.
Q is the order of the moving-average model.
Taking the difference once was enough to make the time series stationary. A p of 8 and a q of 9 was an excellent fit for our data. Here is the SARIMAX results:
![SARIMAX Results](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/9da8709d-d265-47a8-a0fc-2fcff6dda9c7)
  


# 5- Model Results:
The model was trained on the data from 1958 to 2014, and the rest was used for testing. Here are the model results on the test set.
![Model Prediction of CO2 Levels on the Test Set](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/b503186f-88c3-430d-97f7-a9c44369be6e)
We can see it is doing great.

# 6- Forecasting to 2030:
Here are model results on forecasting from 2015 to 2030 and beyond.
![Model Prediction of CO2 Levels from 2015 and above](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/03ca133d-5a6d-47a1-8c70-23fcd04febac)

A closer look at the predictions.
![Model Prediction of CO2 Levels from 2015 and above 2](https://github.com/HazemMohammed100/CO2-Levels-Analysis-and-Forecasting/assets/89959626/633cdb7c-1660-4363-a98f-51e3fb81d516)
