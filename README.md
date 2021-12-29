# MLworkshop

## Citation: The data used in this exercise is derived from [Student Performance Data Set](http://archive.ics.uci.edu/ml/datasets/Student+Performance)

## Deploy an Azure Machine Learning Workspace

1. Deploy an Azure Machine Learning Workspace using the ML Accelerator ARM template [here](https://github.com/DataSnowman/analytics-accelerator#deploy-an-azure-machine-learning-workspace)

Click the Deploy to Azure button

![deployamlws](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deployamlws.png)

* Select the resource group assigned to you by your Azure Admin.  (Optionally you can create a new resource group if you have access to do so or are an owner of the subscription)

* Select a Region (i.e. West US 2)

* Enter your initials for the Deployment TLA (this makes sure that the storage account created in the deployment is unique.  Note if you have the same intials as someone else in the workshop the second deployment will fail.  Have the second user modify their TLA to allow for a successful deployment)

* Click Review + create

![customdeploy](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/customdeploy.png)

Once Validation is passed click Create.  (Note: If you get an error you may need to register additional resource providers - refer to error for guidance)

![create](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/create.png)

The resources should start to deploy

![progress](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/progress.png)

When the deployment is completed click on `Go to resource group`

![gtrg](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/gtrg.png)

Here are the 4 resources that should be deployed:

![4res](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/4res.png)

Click on the Machine learning workspace (in this case mine is called mlws-q5mmlzaejquga) and then click on Lauch studio

![mlws](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/mlws.png)

![launch](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/launch.png)

Here is what Studio should look like:

![amls](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/amls.png)


