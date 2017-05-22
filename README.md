# EVD-Project
Using Machine Learning to predict patients outcome after External ventricular drains Trials

# Create Train/Test set
This function is to make sure we have one consistent train/test set.

Run Create Train-Test. This function will create a train set and a test set for each hour and save them.
First, Locate the Dropbox Folder and point to the path of the dropbox folder. For example, if my dropbox is at 'D:/Dropbox', then my input will be:

```
server = 'D:'
```

This will create 20% test and 80% train sample. This function will try to create new hour folder so the current directory should be empty, otherwise error message. To fix this, go to the path (should be '~/Dropbox/Rotation 3 Project/TrainTest') and move all the train/test folder (should be named 01, 02, etc.) for each hour into a newly created folder (whatever name you want to use)

# Logistic Model
Run Logistic Model (Hold out set): 
Pinpoint to the path of the dropbox folder.

```
server = 'D:' 
```

Run the training function and testing function in the ipython notebook. This should:
- Train the model
- Save the model for each hour into a .pkl file (that can be loaded later)
- Load the .pkl model for each hour and fit, then test on different test set
- Save the results to a .csv file

NOTE: The model will try to save .pkl files at '~/Dropbox/Rotation 3 Project/Models/Logistic', thus you want to store old .pkl files somewhere (preferbly in a new folder in the same directory with the same name as the TrainTest folder so we don't get confused), otherwise previous .pkl files will be overwritten. 

NOTE2: The results will be output into '~/Dropbox/Rotation 3 Project/Result'. This directory has 3 folders, including RF and Logistic. Make sure to move all old results into one of these 2 folders so we don't overwrite it. 

# RandomForest Model
Run RandomForest (Test set).ipynb:
Same as before Logistic


