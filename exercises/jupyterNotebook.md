# Use Jupyter on Compute Instance to Clone GitHub Repo and run Notebooks

Click the Jupyter link under Applications.  Note: You should have created this earlier, but you my need to Start the Compute instance if you Stopped it

![jrunning](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/jrunning.png)

Your Jupyter environment should look like this:

![jupyter](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/jupyter.png)


Navigate to your user folder and click on New>Terminal

![openterminal](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/openterminal.png)

search for and cd to your User Directory and cut the paste the following to the terminal to clone the GitHub Repo

```
git clone https://github.com/DataSnowman/MLworkshop.git
```

![terminal](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/terminal.png)

The GitHub Repository folders and files should now be visable and usable in Jupyter

![mlwsclone](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/mlwsclone.png)

Open up the notebooks folder

![notebooks](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/notebooks.png)

Open the `PandasOneHotEncoding.ipynb` notebook

![pandasOHE](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/pandasOHE.png)

Run each cell individualy by clicking on the Run this cell icon
![runthiscell](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/runthiscell.png)

You can also run each cell by selecting the cell and entering either `Shift+Enter` which runs the highlighted cell and then moves to the next, or `Control+Enter` which runs the cell as stays on the cell.

![runcell](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/runcell.png)

Description of cells:

Cell1 - Code cell that imports Pandas and loads CSV data into a dataframe

Cell2 - Markdown cell that describes the attributes of the student-mat.csv file

Cell3 - Code cell that describes the numeric features in the dataframe

Cell4 - Code cell that imports numpy and matplotlib and creates some plots of the categorical features in the dataframe

Cell5 - Code cell uses Pandas getdummies to One Hot Encoding of all Nominal Columns

Cell6 - Code cell uses Pandas getdummies and drop_first=True which is important to use, as it helps in reducing the extra column created during dummy variable creation. Hence it reduces the correlations created among dummy variables

Cell7 and Cell8  - Code cell that shows the data types of the colums in each of the dummy columns

Cell9 - Code cell that write the two dataframes out to an output folder

Cell10 and Cell11- Code cell that imports the azureml.core SDK and AML Workspace

Cell12 - Code cell that prints the Compute Resources available in the AML Workspace

Cell13 - Code cell that determinesb the datastores in your AML workspace

Cell14 and Cell15 - Code cell that upload data to a datastore

Cell16 and Cell17 - Code cell that create a tabular datasets in AML

Cell18 and Cell19 - Code cell that registers the tabular datasets in AML

Cell20 = Code cell that prints the registered datasets in AML

Note: The `PandasOneHotEncodingDetail.ipynb` notebook does similar work but show all the detail and merges one dummycolumn at a time.  This maybe a process similar to what you would do for data preparation in Data Integration (ETL/ELT) tools.

Note: Their is alsob koalas.get_dummies in databricks https://koalas.readthedocs.io/en/latest/reference/api/databricks.koalas.get_dummies.html that can be used in Spark Notebooks to do this at scale for large datasets

To continue on your Azure ML journey clone the following GitHub Repo into Jupyter on your Compute instance

```
git clone https://github.com/MicrosoftLearning/mslearn-dp100.git
```

