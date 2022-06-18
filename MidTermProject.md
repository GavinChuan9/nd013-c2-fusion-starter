# Mid-Term Project: 3D Object Detection

## Step 1. Compute Lidar Point-Cloud from Range Image

### EX1: Visualize range image channels 
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX1/img/midterm/S1_EX1.png?raw=true)

### EX2: Visualize point-cloud
#### 1. Find 10 examples of vehicles with varying degrees of visibility in the point-cloud
* Front of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/1.png?raw=true)
* Side of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/2.png?raw=true)
* Back of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/3.png?raw=true)
* The vehicle features (roof, outer mirror) are lost at medium range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/4_new.png?raw=true)
* The vehicle features are almost lost at long range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/5_new.png?raw=true)
* Vehicle enter blind spot area a little bit, lost some vehicle features<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/6.png?raw=true)
* Vehicle enter blind spot area, lost most of the vehicle features<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/7.png?raw=true)
* The vehicle features blocked by in front of the car<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/8.png?raw=true)
* some vehicle features are blocked by leaves<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/9_new.png?raw=true)
* Some vehicle features are blocked by shrub<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/10_new.png?raw=true)
#### 2. Try to identify vehicle features that appear stable in most of the inspected examples and describe them
#### Vehicle features that appear stable in most of the inspected examples:
* The vehicles running at the same direction:<br/>
    * Rear bumper<br/>
    * Luggage door<br/>
    * Doors, outer mirrors and wheels are hard to perceive at long range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/2_1.png?raw=true)
* The vehicle driving opposite direction<br/>
    * Front bumper<br/>
    * Doors are hard to perceive at long range<br/>
    * Windshield (light is difficult to reflect, intensity value almost equal to zero[black color])<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/2_2.png?raw=true)

## Step 2. Create Birds-Eye View from Lidar PCL

### EX1: Convert sensor coordinates to bev-map coordinates
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S2_EX1/img/midterm/S2_EX1.png?raw=true)

### EX2: Compute intensity layer of bev-map
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S2_EX2/img/midterm/S2_EX2.png?raw=true)

### EX3: Compute height layer of bev-map
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S2_EX3/img/midterm/S2_EX3.png?raw=true)

## Step 3. Model-based Object Detection in BEV Image

### EX1: Add a second model from a GitHub repo
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S3_EX1/img/midterm/S3_EX1.png?raw=true)

### EX2: Extract 3D bounding boxes from model response
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S3_EX2/img/midterm/S3_EX2.png?raw=true)

## Step 4. Performance Evaluation for Object Detection

### EX1: Compute intersection-over-union (IOU) between labels and detections
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S4_EX1/img/midterm/S4_EX1.png?raw=true)

### EX2: Compute false-negatives and false-positives
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S4_EX2/img/midterm/S4_EX2.png?raw=true)

### EX3: Compute precision and recall
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S4_EX3/img/midterm/S4_EX3.png?raw=true)
