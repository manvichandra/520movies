
We are basically analysing the  data associated with various movies including their Gross revenue,number of tickets sold,various distributors,rank,ratings and production countries.We are extracting data from a website called http://www.the-numbers.com/ which has a data of over 20,000 movies and nearly 100,000 people are now tracked and we continue our commitment to making this data available to the widest possible audience.
We are processing data on Hadoop cluster using HIVEQL to display movie ratings, gross revenue etc.
The data is represented in the form of graphs which would display the most popular movie on the basis various criteria.

## **System Requirements**
Number of worker nodes-2

Specification of each node

Number of Cores-8

RAM-14GB

Discs-16

## **Getting Started with Hive**
## Step 1
**_Create an Azure Storage account_**

1. Sign in to Azure Portal

2. Click NEW in the lower-left corner and then enter the values as shown in the figure below:- 
 
 [Fig 1:creation of storage account](http://github.com/manvichandra/520movies/tree/master/images/storage.jpg)
    

##Step 2
**_Provision a Hadoop Cluster_**

1. Click NEW -->Data + Analytics--> HDInsight and create a cluster as shown in the following image:-

 [Fig 2:Provision of Hadoop Cluster](http://github.com/manvichandra/520movies/tree/master/images/cluster.jpg)

     
                        
##Step 3

**_Login into Microsoft Azure HDInsight QUERY CONSOLE_**

1. Once the HDInsight Cluster is provisioned in the Azure portal, click on the cluster name where you want to run the query.

2. Enter the Hadoop user account and password. The default user name is admin; the password is what you entered while provisioning the cluster. The dashboard looks like  in the figure below:-

 [Fig 3:HDInsight Query Console](http://github.com/manvichandra/520movies/tree/master/images/console.jpg)

## Step 4 
**_Upload data to Azure Blob storage_**

1. Upload data to Blob storage using Cloudberry Box for Azure Blob Storage as shown below:-

 [Fig 4:Upload data to Azure Blob](http://github.com/manvichandra/520movies/tree/master/images/BLobStorage.jpg)


2. Navigate to Microsoft Azure HDInsight QUERY CONSOLE and click on 
   File Browser-->Storage Account-->HDInsight cluster recently created.
   
3. The folder named "movies" is uploaded .

##Step 5
_**Hive Queries**_

1. On the Hive Editor tab, for Query Name, enter Query520_1. The query name is the job title. 

2. In the query pane, enter the Hive query as shown in the image:

 [ Fig 5:Hive Query Editor](http://github.com/manvichandra/520movies/tree/master/images/queryeditor.jpg)


3. Click Submit. It takes a few moments to get the results back.

4. When the Status field changes to Completed, select View Details for the job. On the details page, the Job Output would be displayed.

[_Note:_ Queries.txt contains the list of queries executed in this application.All the queries can be executed in the similar manner as described above]

## Step 4
**_Exporting data to Excel_**

Once the job has successfully completed, you can use the Microsoft Hive ODBC Driver to import data from Hive into Excel. Once you have installed the driver, use the following steps to connect to the table:-

1. Open Excel and create a blank workbook.
2. From the Data tab, select From Other Sources, and then select From Microsoft Query.
3. When prompted to Choose Data Source, select the Sample Microsoft Hive DSN.
4. In the Microsoft Hive ODBC Driver Connection dialog, enter the following values, and then click OK.

Host - The host name of your HDInsight cluster.

For example, mycluster.azurehdinsight.net

User Name - The administrator name for your HDInsight cluster

Password - The administrator password.

5.In the Query Wizard, select the  table, and then select the > button.

6.Click Next to continue through the wizard, until you reach a dialog with a Finish button. Click Finish.

7.When the Import Data dialog appears, click OK to accept the defaults. After the query completes, the data will be displayed in Excel as shown in the figure below:-


 [Fig 6:Load data to excel](http://github.com/manvichandra/520movies/tree/master/images/excel.jpg)
## **Getting started with Apache Spark**
 
## **Step 1**

1. Login to your Ibm Bluemix Account and look for IBM Analytics for Apache Spark .

2. Create a new notebook.

3.Upload the raw data file to Bluemix Object Storage.

4.Define the first RDD by loading the raw data.

5.Parse the raw data into columns.

6.Transform the dataset according to the Queries.
_**In order to see the output for the Movie Dataset follow the step below:-**_

## **Step 2**

1. Create a new notebook. Click New, and then select Python .

   [Fig 7: Ipython notebook creation](https://github.com/manvichandra/520movies/blob/master/images/notebookcreation.JPG)

2. Import the "Spark.ipynb" attached in the code folder and press the Run button to execute.

    [Fig 7:Imported file](https://github.com/manvichandra/520movies/blob/master/images/Imported.JPG)
   
##**Special Thanks**
- (https://developer.github.com/  "GitHub for  API and style")

- Microsoft Azure

## **Licence**

Developed By:  
- Kumari Parul Bisen
- Manvi Chandra
- Krutik Shah
