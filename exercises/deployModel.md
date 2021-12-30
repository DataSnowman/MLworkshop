# Deploy an AutoML model to an AML Endpoint

One the AutoML run completes you can review the models and then select one to deploy to an AML Endpoint on an Azure Container Instance docker container, or Azure Kubernetes Server (AKS) cluster.

If you still have the run open you can just click on Models

![complete](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/complete.png)

You can see all of the Models and their normalized root mean square error

![models](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/models.png)

If you can find the run you can alway find it in the Author group under Automated ML Recent runs

![recentRuns](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/recentRuns.png)

Or under the Assets group under Experiments

![experiments](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/experiments.png)

To deploy a model select the Algorithm you would like to deploy like `MaxAbsScaler, RandomForest` 

![maxabs](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/maxabs.png)

Click Deploy>Deploy to webservice

![deploy](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deploy.png)

Name the endpoint `studentgrade`. Select Computer type: `Azure Container Instance` and `Enable authentication`.  Click Deploy

![deployAmodel](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deployAmodel.png)

Select Endpoints in the Assets Group

![endpoint](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/endpoint.png)

Click on the Endpoint name to see the Deployment state

![deploymentState](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/deploymentState.png)

It will eventually change from Unhealthy to Transitioning to Healthy

![healthy](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/healthy.png)

You can test the endpoint

![test](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/test.png)

Also details on how to consume the endpoint

![consume](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/consume.png)

You can now use the API endpoint in something like an application or Power BI

Go to the [Consume the Models AML Endpoint in Power BI](https://github.com/DataSnowman/MLworkshop/blob/main/exercises/consumeModelpbi.md) exercise for the next steps for consuming the AML Endpoint in Power BI Desktop








