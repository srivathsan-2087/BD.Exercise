# BD.Exercise
# CONTENTS																

There are 2 zip files containing the source

	1. NumberProcessor.Server.zip - Contains the Web API source code.
	2. NumberProcessor.Client.zip - Contains Angular Client source code.
	
# Nuget packages used:
1. Microsoft.Extensions.DependencyInject.Abstractions 	- Accessing IServicesCollection type outside the API project.
2. Microsoft.Extensions.Hosting.Abstractions 			- Accessing IHostedService type outside the API project.
3. Moq													- Mocking of service dependencies in Unit Tests.
4. RestSharp											- Library to make Http calls in the NumberProcessor.Proxies project.
5. XUnit												- Test library used in unit tests.

# Setup Steps:
## Server:
1. 	The Web API component uses certain nuget packages.
2. 	Extract the NumberProcessor.Server.zip file. Locate the solution file - NumberProcessor.sln.
3. 	Restore the nuget packages and compile the solution.
4. 	Once compiled, Debugging the solution will start an instance of IIS express. 
	  Launching a browser windows has been disabled. 
5. 	The Web API component can be accessed through the URL - http://localhost:4516

## Client:
1. 	Extract the NumberProcessor.Client.zip and navigate to the 'src' folder. Open Folder from VS Code.
2. 	Open a new terminal within VS Code
3.  Run the command 'npm install' to restore the packages required for the Angular client.
4. 	When 'npm install' command completes, issue the command 'ng serve'. 
5. 	Open the browser and access the url - http://localhost:4200 - to use the angular client.
