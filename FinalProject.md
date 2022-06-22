# Final Project: Sensor Fusion and Object Tracking

### 1. Write a short recap of the four tracking steps and what you implemented there (filter, track management, association, camera fusion). Which results did you achieve? Which part of the project was most difficult for you to complete, and why?
* Step 1. Tracking<br/>
I implemented predict and update step, and EKF is applied to a simple single-target scenario with lidar only.<br/>
The result of execution is as follows. The mean RMSE is 0.32 (smaller than 0.35).<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S1/img/final/S1_RMSE.png?raw=true)
* Step 2. Track Management<br/>
Set track state to ***Initialized / Tentative / Confirmed*** at the right time, and try to keep track score between 0 and 1.<br/>
Delete track if the score is too low or P is too big.<br/>
The result of execution is as follows. There is one single track without track losses in between.<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S2/img/final/S2_RMSE.png?raw=true)
* Step 3. Data Association
Which track has to be updated by which measurement? In there, we apply the Mahalanobis distance to solve that.<br/>
The result of execution is as follows.<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S3/img/final/S3_RMSE.png?raw=true)
* Step 4. Sensor Fusion
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S4/img/final/S4_RMSE.png?raw=true)

### 2. Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)? 

### 3. Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?


### 4. Can you think of ways to improve your tracking results in the future?

