# Contoso
Contoso University Web App


<!-- Server=mysql;Port=4000;Database=votes;User=root;SslMode=None

Server=localhost;Database=test;Uid=root;Pwd=123456; -->

dotnet aspnet-codegenerator razorpage -m Student -dc SchoolContext -udl -outDir Pages\Students --referenceScriptLibraries

dotnet aspnet-codegenerator controller -name StudentsController -async -api -m Student -dc SchoolContext --relativeFolderPath Controllers

dotnet ef migrations add InitialCreate
dotnet ef database update

https://localhost:5001/School/Create 可以访问

https://127.0.0.1:5001/api/Student   api连接访问