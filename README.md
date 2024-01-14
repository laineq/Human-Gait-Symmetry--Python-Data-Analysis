# Human Gait Symmetry Analysis 

**Data Collection:**

The data collected is stored under CMPT353_Project/data. There is a total of 101 files where each file contains information such as time, x-acceleration, y-acceleration, z-acceleration and total_acceleration of the activity performed which can be known via the file name, 
For example :
1. hand__R.csv represents the dataset for the right hand 
2. hand__L.csv represents the dataset for the left hand 
3. sensor__L_regular.csv represents the dataset for normal left foot 
4. sensor__R_regular.csv represents the dataset for normal right foot 
5. sensor__L_injury.csv represents the dataset for the injured left foot 
6. sensor__R_injury.csv represents the dataset for the injured right foot 

**Libraries Required**

```pip install spark``` 

```python -m pip install -U matplotlib```

```pip install pandas pandas```

```pip install numpy```

```python -m pip install scipy```

**Problem Statement:**

1.Does the two legs’ movement symmetric during walking? Or in another word, does the left leg move at a different scale compared to the right leg? 
2.If someone got injured, does our method successfully determine the asymmetric of the movement of the legs?
3.Does the hand and leg from the same side move at different scales during walking? 


**Code Instruction :**

To run the code in data_analysis.py, pySpark is required and data should be stored in the same folder as data_analysis.py

```spark-submit data_analysis.py data output```

**Output :**

1. normal_data.png - Line graph which shows the data of left vs right foot versus time 
2. injury_data.png - Line graph which shows the data of left injured foot and right injured foot versus time
3. hand_data.png - Line graph which shows the data of left hand and normal hand versus time
4. csv file which contains the p-value of each of the problem statements stated above
