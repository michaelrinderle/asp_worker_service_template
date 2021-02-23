* ASP WORKER SERVICE TEMPLATE/DEMO

* Features
	* .Net Core Worker Service
	* Asp.Netcore Web API Controller Functionality
    
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