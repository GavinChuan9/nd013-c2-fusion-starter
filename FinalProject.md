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
* Step 3. Data Association<br/>
Which track has to be updated by which measurement? In there, we apply ***the Mahalanobis distance*** to solve that.<br/>
The result of execution is as follows.<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S3/img/final/S3_RMSE.png?raw=true)
* Step 4. Sensor Fusion<br/>
In this step, i fuse measurements from lidar and camera. and check the object is in camera field of view.<br/>
The result of execution is as follows.<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/FP_S4/img/final/S4_RMSE.png?raw=true)
* Which part of the project was most difficult for you to complete, and why?<br/>
I think is ***Step 3. Data Association***. When i first finished it, the result of execution is very worse, it even can not track any objects.<br/>
Because i forgot to put the appropriate index in the lists of unassigned tracks & meas, so i spent a little time to solve this issue.<br/>

### 2. Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)? 
The reliability of camera-lidar fusion is higher than lidar-only tracking.<br/>
In theory, camera and lidar can complement each other's weaknesses, and camera-lidar fusion can improve the performance of object tracking.<br/>
The result of execution from ***Step 4. Sensor Fusion***, overall RMSE are reduce, and ghost tracks can not easily change it's state from ***Initialized*** to ***Tentative***.<br/>

### 3. Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?
In real-life scenarios, the environment is more complex (ex. weather, traffic, sensor misalignment, etc.), that maybe affect the stability of fusion result.<br/>

### 4. Can you think of ways to improve your tracking results in the future?
* Association: Apply GNN or JPDA
* Using Object Detection. apply different motion models and covariates after recognize object's class(ex. vehicle, bike, pedestrian, etc.).
