# Azure Admin setup for the attendees of the ML Workshop

1. Each user while need an Azure Resource Group that they have contributor access to.  Named something like: mlworkshop-<alias> (Example: mlworkshop-darsch for darsch@microsoft.com)


Create an Azure Resouce Group for each workshop attendee

![createrg](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/createrg.png)

2. User must have Contributor access to their assigned Resource Group

Add Role Assignment

![addrole](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/addrole.png)

Select Contributor

![contrib](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/contrib.png)

  `+ Select members` to add

![selectmemb](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/selectmemb.png)

The member must show up as a Contributor

![contribaccess](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/contribaccess.png)

3. Make sure that these resource providers are registered

    * `Microsoft.MachineLearning`
    * `Microsoft.MachineLearningServices`
    * `microsoft.insights`

![rpreg1](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/rpreg1.png)

![rpreg2](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/rpreg2.png)

4. Have one of the users test that they can deploy an Azure Machine Learning Workspace using the ML Accelerator ARM template [here](https://github.com/DataSnowman/analytics-accelerator#deploy-an-azure-machine-learning-workspace) using the directions in the ML workshop [ReadMe](https://github.com/DataSnowman/MLworkshop/blob/main/README.md)

![deployamlws](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deployamlws.png)