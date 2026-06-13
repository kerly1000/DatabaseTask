# DatabaseTask/ Pildid pdf failis
Code-First Migration

1.	Ava projekt failist DatabaseTask.snl
2.	Määra failis appsettings.json ühendus kohaliku serveri nimega, nt localhost
3.	Ava NuGet Package Manager, vali Default Project-> DatabaseTask.Data
4.	Sisesta käsklus-> Add-Migration InitialCreate
5.	Sisesta käsklus-> Update-Database

   


Database-First Migration

1.	Kustuta projektist Employee.cs ja DatabaseTaskDbContext.cs ning Migrations kaustas olevad failid.
2.	Avan Visual Code menüüs Tools-> Connect to Database
3.	Vali oma arvuti MS SQL server
4.	Linnuke kasti „Trust Server Certificate“
5.	Vali andmebaas, millega ühendust soovid luua
6.	Avan View-> Server Explorer-> parem klikk ühendusel-> Properties. Kopeeri  Connection String ja lisa see appsettings.json „ConnectionStrings“ plokki DataBaseConnestion alla.
7.	Package Manager Console’is kontrolli, et Default Project all on endiselt valitud DatabaseTask.Data ja anna käsklus stringiga + … : "Data Source=kompu\sqlexpress;Initial Catalog=Asd1234;Integrated Security=True" Microsoft.EntityFrameworkCore.SqlServer -outputdir Models -context DBTaskDBcontext -force
8.	Käsk loob Models alla andmebaasis olevate tabelite mudelid: 
 
