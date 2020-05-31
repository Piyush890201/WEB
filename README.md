# Contact Application 
Contact application - simple .Net core Web Api for managing contacts using .Net core Web API and EntityframeworkCore ans SQL server as database


##Database Setup

```bash
Run command using Package Manger console 

Add-Migration -Context ContactWebAPI.Data.ContactDbContext -Name ContactInfo

update-database
```bash
above commands will generate DB at localMSSQLSERVER

Build application 

#Run API using postman tool

https://localhost:443/api/Contact/AddContact -  

for adding conatct need to provide details in body in Json format
Input parameter
{
	"FirstName":"Piyush",
	"LastName":"Bhole",
	"Email":"Piyush.Bhole@gmail.com",
	"ContactNumber":"9890398207"
}


https://localhost:443/api/Contact/GetAllContacts


https://localhost:443/api/Contact/GetContact?criteria=9890398207 -

for fetching conatct need to provide details in body in Json format
passing parameter criteria and value either FirstName or ContactNumber or Email

https://localhost:443/api/Contact/UpdateContact-

for adding conatct need to provide details in body in Json format
{
	"FirstName":"Piyush",
	"LastName":"Bhole",
	"Email":"Piyush.Bhole@gmail.com",
	"ContactNumber":"9890398207"
}


https://localhost:443/api/Contact/DeleteContact?criteria=9890398207 - 

for adding conatct need to provide details in body in Json format
passing parameter criteria and value either FirstName or ContactNumber or Email


