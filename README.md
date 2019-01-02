# QuickStartDatalake

--------------------------------------------------------------------------
# Overview :
--------------------------------------------------------------------------
The aim of Yash Azure Quick start solution is to showcase the capabilities of Server less Data Lake in the Azure Cloud. 
- Yash Data Lake in Azure Cloud showcases features such as
	* Data Ingestion
		* Batch 
		* Streaming 
	* Data Processing
		* Batch 
		* Real Time 
	* Data Governance
		* Meta data management
		* Data Lineage
		* Data Security
	* Ad-Hoc analytics for exploring different data insights and visualization
<br />
The deployment  of Quick start Data lake also includes an optional wizard and a sample dataset that is used  to demonstrate data lake capabilities.

![alt text](https://raw.githubusercontent.com/KuldeepShikhare/AzureQuickStartDatalake/master/scripts/images/Architecture.png)

--------------------------------------------------------------------------
# Pre-Requisites
--------------------------------------------------------------------------
- Application registration in AAD :
	1. Service Principal
	2. App Secret Key
	3. Assign required permissions
	4. Set Reply URL :https://your-function-app-name.azurewebsites.net/.auth/login/aad/callback
		[Note = your-function-app-name : The function name which you would be giving while deploying Yash Data Lake]
- Add following permissions to Application registered in AAD :
	1. Azure Analysis Services
	2. Azure Data Lake
	3. Windows Azure Active Directory
- Check services used in Quick start Data lake are available in that region.Also check whether resources are registered in that region for that subscription.

- User of Quick start Data lake must be owner for existing resource group or admin of  newly created resource group used at the time of deployment of ARM template.

- Add Application in IAM of subscription.
	
- Open Elasticsearch function app to load data to Elasticsearch for first time
	
--------------------------------------------------------------------------
The following section provide steps for running the Quickstart.
# Run and monitor the deployment:
After you deploy the template, to run Quickstart, do the following steps:
1. Go to the Output section of ARM template deployment services.
2. Copy URL from output section.
3. Open this URL in new tab
4. Check app service plan in that resource group.
5. dd Application and user in IAM of ADL store and in data explorer access.
6. Add application and user in IAM of Azure Data Factory.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FKuldeepShikhare%2FAzureQuickStartDatalake%2Fmaster%2FazureDeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
