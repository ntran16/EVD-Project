# EVD-Project
Using Machine Learning to predict patients outcome after External ventricular drains Trials

Run Create Train-Test. This function will create a train set and a test set for each hour and save them.
First, Locate the Dropbox Folder and point to the path of the dropbox folder. For example, if my dropbox is at 'D:/Dropbox', then my input will be:

```server = 'D:'
```

This will create 20% test and 80% train sample. This function will try to create new hour folder so
the current path should be empty, otherwise error message (go to the path and move all the train/test 
folder into a new folder)

Run Logistic Model (Hold out set): 
Pinpoint to the path of the dropbox folder.

```server = 'D:' 
```

Run the training function and testing function in the ipython notebook. This should:
- Train the model
- Save the model for each hour into a .pkl file (that can be loaded later)
- Load the .pkl model for each hour and fit, then test on different test set
- Save the results to a .csv file

Run RandomForest (Test set).ipynb:
Same as before


