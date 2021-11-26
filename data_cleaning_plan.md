raw_data/s1757177/Respeck_s1757177_Climbing stairs_06-10-2021_16-34-18.csv
- accel_y: inverse?

raw_data/s1841064/Respeck_s1841064_Climbing stairs_29-09-2021_13-51-13.csv
- accel_x: inverse?
- accel_y: inverse?



---
s1893835: only 12 respeck datasets

---
Task:
1) open visualize_aggregated_data.ipynb
2) open ./individual_pics
3) for aggregated data for each label in visualize_aggregated_data.ipynb, look at pictures in ./individual_pics, compare and idenfity the .csv files with questionable data
4) follow to 2 examples above, note down:
   1) the csv file names, 
   2) and the questionable attribute,
   3) how might it be fixed , if possible, or should we exclude it from the dataset
---
Climbing stairs
1) s1541031, accel_x and accel_y are reversed
2) s1721256, accel_y is reversed with x and z
3) s1757177, accel_y is reversed with x and z
4) s1813106, file name and file content is Climbing stairs, but "activity_type" is falling on knees
5) s1841064, accel_x and accel_y are reversed
---
Descending stairs
1) s1541031, accel_x is reversed
2) s1702583, file name is Descening stair, but content and "activity_type" is Desk work
3) s1721256, accel_y is reversed with x and z
4) s1823274, accel_x averaged at 1, normally should be averaged at 0
5) s1841064, accel_x averaged at -1, normally should be averaged at 0
---
Desk work
1) s1541031, accel_x and accel_y are reversed
2) s1702583, file name and file content is Deskwork, but "activity_type" is Walking at normal speed
3) s1841064, accel_x is reversed with accel_y and accel_z
4) s1823274, accel_x averaged at 1, normally 0-0.4 accel_y averaged at 0 to -0.4, normally -1
5) s2192970, accel_z averaged at -0.6, normally 0
---
Falling on knees
1) s1813106, accel_z is reversed with x and y, data content seems not similar regular falling on knees
2) s1823274, accel_x is reversed with y and z
ALL FALLINGS USE CLEAN DATA PROVIDED BY PROFESSOR, because the frequency of falling that students collects variates
---
Lying down left
1) s1702583, file name and data content is Lying down left, but "activity_type" is Lying down on stomach
2) s1721256, accel_z is reversed
3) s1727780, accel_x averaged 0.6 normally -1, accel_z averaged 0.8 normally -0.5
4) s1757177, accel_x averaged 0.6, normally -1
5) s1817455, accel_x averaged 0.6, normally -1, accel_z averaged 1 normally -0.5
6) s1894401, accel_x and accel_z are inversed to 0
7) s221162, accel_x and accel_z are inversed to 0
8) s1893835, too noizy data, gyro raised to 40, normally in range (4-,-4)
---
Lying down on back
1) s1541031, accel_x and accel_y are reversed
2) s1721256, accel_z is inversed to 0
3) s1727780, accel_z is inversed to 0
4) s1817455, accel_z is inversed to 0
5) s1894401, accel_z is inversed to 0
6) s2211162, accel_z is inversed to 0
---
Lying down on stomach
1) s1721256, accel_z is inversed to 0
2) s1727780, accel_z is inversed to 0
3) s1817455, accel_z is inversed to 0
4) s1894401, accel_z is inversed to 0
5) s2211162, accel_z is inversed to 0
---
Lying down right
1) s1721256, accel_x is inversed to 0
2) s1727780, accel_x is inversed to 0
3) s1817455, accel_x is inversed to 0
4) s1894401, accel_x is inversed to 0
5) s2211162, accel_x is inversed to 0
6) s1757177, accel_x is inversed to 0
7) s1823274,accel_y averaged at 0.65, normally 0
---
Movement
WE CAN DEFINE ANY MOVEMENT TO BE A MOVEMENT
---
Running
1) s1541301,accel_y is inverse to 0
2) s1702583, file name is Running, data content is also running, “activity_type” is Movement
3) s1721256,accel_y is inverse to 0 
4) s1870697,accel_y is inverse to 0
---
Sitting bent backward
1) s1702583, file name and content is sitting bent backward, “activity_type” is Movement
2) s1727780, accel_z is < 0, should be >0
3) s1817455,accel_z is inverse to 0
4) s1894401, accel_z is inverse to 0
5) s2171931, accel_z is inverse to 0
6) s2211162, accel_z is inverse to 0
---
Sitting bent forward
1) s1702583, file name and content is sitting bent forward, “activity_type” is Movement
2) s1541031, accel_y is 0, should be approx -1
3) s1721256, accel_y is 0, should be approx -1, accel_z is > 0, should be < 0
4) s1727780, accel_z is > 0, should be < 0
5) s1757177, accel_y is 0.4, should be approx -1
6) s1817455, accel_z is 1 , should be < 0
7) s1870697, accel_z is 1, should be approx -1
8) s2211162, accel_z is > 0 , should be < 0
---
Standing
1) s1541301, accel_y and x is reversed
2) s1702583, file name and content is Standing, “activity_type” is Movement
3) s1721256, accel_y and x is reversed
4) s1823274, accel_x is at 1, should be around 0, accel_y is at -0.2, should be -1
5) s2171931, accel_x is 1, shoube be 0, accel_y is 0.4, should be -1
---
Sitting
1) s1541301, accel_y and x is reversed
2) s1702583, file name and content is sitting, “activity_type” is Movement
3) s1721256, accel_y and x is reversed
4) s1823274, accel_x is at 1, should be around 0, accel_y is at -0.4, should be -1
5) s2171931, accel_x is 1, shoube be 0, accel_y is 0.2, should be -1
---
Walking at normal speed
1) s1702583, file name and content is sitting, “activity_type” is Movement
2) s1823474, accel_y and x is reversed
3) s1841064,accel_y and x is reversed
4) s1870697, accel_y and x,z is reversed
5) 