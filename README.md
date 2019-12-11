# Contoso
Contoso University Web App


<!-- Server=mysql;Port=4000;Database=votes;User=root;SslMode=None

Server=localhost;Database=test;Uid=root;Pwd=123456; -->

dotnet aspnet-codegenerator contoso -m Movie -dc SchoolContext -udl -outDir Pages\School --referenceScriptLibraries

dotnet aspnet-codegenerator controller -name StudentController -async -api -m Student -dc SchoolContext --relativeFolderPath Controllers