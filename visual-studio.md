
Change Nugget source:
---
Tools-->Nugget Package Manager--> Package Manager Settings--> Package Sources --> Press + and add source as ```https://api.nuget.org/v3/index.json```.   

OR via CLI:   
```dotnet add package Swashbuckle.AspNetCore -s https://api.nuget.org/v3/index.json```

Generate project global.json file for specific sdk:
---
```dotnet new globaljson --sdk-version 6.0.100```
