* ASP WORKER SERVICE TEMPLATE/DEMO

* Features
	* .Net Core Worker Service
	* Asp.Netcore Web API Controller Functionality
   
* Load Template

```
load_template.cmd (in root folder)
dotnet new (look for new template entry)
```

 
* Quick Publish

```
cd $proj
dotnet restore
dotnet publish -o $Path
```

* Install Service

- In elevated terminal!

```
sc.exe create AspWorkerService binpath= $Path\AspWorkerService.exe
sc.exe start AspWorkerService
```