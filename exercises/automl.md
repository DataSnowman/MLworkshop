# Use AutoML and Compute Cluster to build Student Final Grade prediction model

Click on Datasets under the Assets group in AML.  You should see the following Datasets.  Note: You should have created this earlier bu following the [Use Jupyter on Compute Instance to Clone GitHub Repo and run Notebooks](https://github.com/DataSnowman/MLworkshop/blob/main/exercises/jupyterNotebook.md) exercise.  If have not done this please  compete this exercise, or fix any errors encountered during running the notebook.

![datasets](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/datasets.png)

Click on the `student ohe k1 dataset` dataset and click Explore.  Under Preview you can see the columns and rows of this tabular dataset

![explore](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/explore.png)

Click on Profile.  You can scroll down and see profiles of each of the columns

![profile](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/profile.png)

Now lets use AutoML to create some regression models using this dataset.  Click on Automated ML under the Author group in AML.
Click on `+New Automated ML run`

![automl](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/automl.png)

Click on the `student ohe k1 dataset` Dataset name

![selectDataset](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/selectDataset.png)

You will see Data preview and Data Statistics similar to what we looked at when viewing the Dataset earlier.  Click Close to return to the AutoML wizard

![dataStats](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/dataStats.png)

Click Next

![next](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/next.png)

Fill out the details to Configure run 

Select Create new with New experiment name of `StudentGrade`, Target Column `G3` (which is the students final grade in the dataset).  Select compute type `Compute cluster` and select the Compute cluster we created earlier.  Click Next

![configRun](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/configRun.png)

Select `Regression` for the Select task and settings. Click Next

![regress](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/regress.png)

Go with the defaults for Validate and Test. Click Finish

![optional](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/optional.png)

This should start the AutoML run

![run](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/run.png)

The run will take about ?minutes.  Depending the type of Compute you chose for the Compute cluster and the size of the cluster.





