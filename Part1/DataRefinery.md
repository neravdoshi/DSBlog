# Tutorial 

This lab will use the [COVID data set](https://www.kaggle.com/fireballbyedimyrnmom/us-counties-covid-19-dataset) to demonstrate data profiling, data visualization, and data preparation capabilities of the Data Refinery tool.  The lab consists of the following steps: 

## Steps

1. [Create Watson Studio service on IBM Cloud](#1-Create-a-Watson-Studio-service-on-IBM-Cloud)
2. [Create a project in Watson Studio and upload the data](#2-create-a-project-in-Watson-Studio-and-upload-the-data)
3. [Use the Data Refinery Tool](#3-use-the-data-refinery-tool)
   a. Profile the data to help determine missing values 
   b. Visualize the data to gain a better understanding  
   c. Prepare the data for modeling 
   d. Run the sequence of data preparation operations on the entire data set. 

### 1. Create Watson Studio service on IBM Cloud

The first step in this tutorial is to set up your IBM Cloud [Watson Studio service](https://cloud.ibm.com/catalog/services/watson-studio). See the video below to help you create your free
IBM Watson Studio service.

* After logging into IBM Cloud, click `Proceed` to show that you have read your data rights.

* Click on `IBM Cloud` in the top left corner to ensure you are on the home page.

* Within your IBM Cloud account, click on the top search bar to search for cloud services and offerings. Type in `Watson Studio` and then click on `Watson Studio` under `Catalog Results`.

* This takes you to the Watson Studio service page. There you can name the service as you wish. For example, one may name it 
`Watson-Studio-trial`. You can also choose which data center to create your instance in. The gif above shows mine as 
being created in Dallas.

* For this guide, you choose the `Lite` service, which is no-charge. This has limited compute; it is enough
to understand the main functionality of the service.

* Once you are satisfied with your service name, and location, and plan, click on create in the bottom-right corner. This creates your Watson Studio instance. 

![watsonStudio](https://media.github.ibm.com/user/79254/files/e493eb80-8626-11ea-87b5-f1c7cf8d50e0)

### 2. Create a project in Watson Studio and upload the data

* To launch your Watson Studio service, go back to the home page by clicking on `IBM Cloud` in the top-left corner. There you see your services, and under there you should see your service name. This might take a minute or two to update. 

* Once you see your service that you just created, click on your service name, and this takes you to your 
Watson Studio instance page, which says `Welcome to Watson Studio. Let's get started!`. Click on the `Get Started` button.

* This takes you to the Watson Studio tooling. There you see a heading that says `Start by creating a project` and a button that says `Create Project`. Click on `Create a Project`. Next click on `Create an Empty project`.

* On the create a new project page, name your project. One may name the project - `insurance-demo`. You also need to associate an IBM Cloud Object store instance, so that you store the data set.

* Under `Select Storage service` click on the `Add` button. This takes you to the IBM Cloud Object Store service page. Leave the service on the `Lite` tier and then click the `Create` button at the bottom of the page. You are prompted to name the service and choose the resource group. Once you select a name, click the resource group `Confirm` button. 

* Once you've confirmed your IBM Cloud Object Store instance, you are taken back to the project page. Click on `refresh` and you should see your newly created Cloud Object Store instance under `Storage`. That's it! Now you can click `Create` at the bottom right of the page to create your first IBM Watson Studio project :) 

![createProj](https://user-images.githubusercontent.com/10428517/81858932-5fab3c00-9519-11ea-9301-3f55d9e2e98d.gif)

* Once you have created your Watson Studio Project, you see a blue `Add to Project` button on the top-right corner of your screen. 

![addProj](../images/addData.png)

* Select `Data`.

* On the right-hand side bar, click on `browse` and then go to where you cloned the repository, and select `TM1 Import.csv`.

![addProj](../images/browse.png)

* Once the upload has finished, you should see `Upload Successful` as shown below. 

![addProj](../images/success.png)
