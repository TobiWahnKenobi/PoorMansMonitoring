# PoorMansMonitoring
FileMaker based monitoring tool for FileMaker Servers and services

Open the file using the following credentials:

Username: admin

Password: admin

Encryption key: catch0myka5fatma_shorts_genossin8luck_henningPAKET


1. Deploy the file on your Monitoring Server (the Filemaker Server that should monitor your other FileMaker Servers)
2. Deploy the file on one of your Client Server(s) (the target FileMaker Servers)
3. Open the file on the Monitoring Server and configure as server using the setup assistant
4. Open the file on your Client Server(s) and set up as client using the setup assistant


If you want to use PMM to monitor a server script or other task, call the function
api.Client Push Ping To Server DataAPI {JSON|I}

Expected Parameters are described in the Script header

If you want to group multiple tasks into one entry in PMM, use the Process parameter:

"Process" : {
	"Name" : JSONString,
	"Value" : JSONString,
	"Max" : JSONString
}

At the moment only Process.Name is supported. Value and Max are reserved for future versions

For anything other than the basic FileMaker Server Monitoring the parameter "Is_Service" should be TRUE
