# MLworkshop

## Citation: The data used in this exercise is derived from [Student Performance Data Set](http://archive.ics.uci.edu/ml/datasets/Student+Performance)

## Prerequisites

If you are not an Owner, Co-Administrator or Contributor of your Azure Subscription you will need to an Administrator to create an Azure Resource Group for you and provider you with Contributor access at the Resource Group level for the Resource Group.  See [Prerequisites](https://github.com/DataSnowman/MLworkshop/blob/main/prereqs/azureresources.md) for details

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

2. Create a Compute instance

Click on Compute under the Manage section, choose Compute instances, and click on +New

![computeinst](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/computeinst.png)

Go with the recommended CPU Option and click `Create`

![createcomp](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/createcomp.png)

This will start creating the compute instance for your Jupyter Notebook

![creating](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/creating.png)

Click the Jupyter link under Applications

![jrunning](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/jrunning.png)

Your Jupyter environment should look like this:

![jupyter](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/jupyter.png)

3. Create a Compute cluster for use with AutoML

Under Compute click on Compute clusters, then click +New

![cluster](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/cluster.png)

Go with the same Location where your deployed your AML workspace (i.e. West US 2). Choose Dedicated, CPU, Select from recommended options, General purpose and click `Next`

![selectvm](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/selectvm.png)

Give it a Compute name like <initials>cpucluster, Min 0, Max 3 and click `Create`

![clustername](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/clustername.png)

Once the cluster is created you can use it for AutoML as well as Designer Compute (Note that the cluster spins down to zero when it is not being used)

![resizing](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/resizing.png)

4. Use Jupyter in Compute instance

5. Use AutoML with One Hot Encoded dataset

6. Stop the Compute instance and/or to Cleanup resources following completion of the ML Workshop

Once the workshop is over you should at least Stop the Compute instance running Jupyter.  To stop the Compute instance click on the instance Name and select stop.  You can also go back and Start the Compute instance VM when you need it.

![jrunning](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/jrunning.png)

To delete all the resources created for the workshop once you have completed the workshop the resources can be deleted by deleting the Resource Group.  Click on Delete resource group

![deleterg](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deleterg.png)

To confirm this is what you want to do, enter the name of the Resource Group and click Delete

![confirm](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/confirm.png)