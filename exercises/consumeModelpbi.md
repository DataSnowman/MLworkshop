# Consume the Models AML Endpoint in Power BI

One the selected model is deployed to an AML endpoint and in a Healthy Deployment state you can now access the endpoint in Power BI

Open up Power BI Desktop

![pbidesktop](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/pbidesktop.png)

Click on Get data and select Web to import data from a webpage

![web](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/web.png)

Choose Basic and copy and paste this URL into the From Web dialog:

```
https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/data/pbidata/student-mat-ohe-k1.csv
```
Click OK

![fromweb](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/frombweb.png)

Select Anonymous and click Connect

![anonymous](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/anonymous.png)

Take the default and click Transform Data button

![transformdata](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/transformdata.png)

This opens the Power Query editor

![pqeditor](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/pqeditor.png)

Click on Azure Machine Learning in the AI insights ribbon group

![aiinsights](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/aiinsights.png)

Select the `studentgrade` endpoint (or the name of your model if it is different). Click OK

![amlmodels](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/amlmodels.png)

Click on the Continue button to set the data privacy

![dataprivacy](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/dataprivacy.png)

Select `Public` as the Privacy level. Click Save

![privacylevel](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/privacylevel.png)

Scroll over to the far right

![predgrade](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/predgrade.png)

Click on the Close & Apply button in the top left corner

![closeapply](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/closeapply.png)

This brings the data including the prediction into the Power BI Desktop report Data

![reportdata](https://raw.githubusercontent.com/DataSnowman/MLworkshop/main/images/reportdata.png)

Thanks for completing this exercise and the proceding exercises


