# Writeup: Visualize point-cloud (ID_S1_EX2)

### 1. Find 10 examples of vehicles with varying degrees of visibility in the point-cloud
1. Front of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/1.png?raw=true)
2. Side of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/2.png?raw=true)
3. Back of the car at short range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/3.png?raw=true)
4. The vehicle features (roof, outer mirror) are lost at medium range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/4_new.png?raw=true)
5. The vehicle features are almost lost at long range<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/5_new.png?raw=true)
6. Vehicle enter blind spot area a little bit, lost some vehicle features<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/6.png?raw=true)
7. Vehicle enter blind spot area, lost most of the vehicle features<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/7.png?raw=true)
8. The vehicle features blocked by in front of the car<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/8.png?raw=true)
9. some vehicle features are blocked by leaves<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/9_new.png?raw=true)
10. Some vehicle features are blocked by shrub<br/>
![alt text](https://github.com/GavinChuan9/nd013-c2-fusion-starter/blob/ID_S1_EX2/img/midterm/10_new.png?raw=true)

### 2. Try to identify vehicle features that appear stable in most of the inspected examples and describe them

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
