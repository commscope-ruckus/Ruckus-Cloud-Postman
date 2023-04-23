# RUCKUS Cloud JWT API
Use this collection to assist in the development of apps using RUCKUS Cloud.
You need to enter your credentials in the body of the /token call. 
Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
response. That needs to be considered when writing API calls using python or any other language. 
Please refer to Ruckus Cloud python examples in the repository Ruckus-Cloud-Python-Scripts for details.

Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud Postman collection (uses API-KEY - Deprecated)
Use this collection to assist in the development of apps using Ruckus Cloud. You need to input your
tenantId, username, password and AP serial number at the tab "Variables". The other variables will be 
assigned automatically by the scripts in this collection.

Note: Ruckus Cloud write-APIs can be asynchronous. A response of 202 indicates an asynchronous 
response. That needs to be considered when writing API calls using python or any other language. 
Please refer to Ruckus Cloud python examples in the repository Ruckus-Cloud-Python-Scripts for details.

Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud with MSP-EC calls (uses API-KEY - Deprecated)
This collection shows how to manage the customer objects in a MSP account.
MSP accounts have different security contexts for the MSP and the customers managed by the MSP. After retrieving the API token using the MSP credentials, you will only be able to do things at the MSP level.
There is an additional call to switch to a customer tenant, in order to be able to manage the customer objects:
 
{{baseUrl}}/api/login/tenant/token/{{customerId}}
 
After that, you can access or change the customer objects.


