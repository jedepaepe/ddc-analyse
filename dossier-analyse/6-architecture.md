# Architecture #
ddc-app est une application web écrite en c# avec une base de données Microsoft SQL Server.

Le design interne de ddc-app est de type MVC (Model View Controller).

L'authentification est réalisée en OpenID avec Microsoft Azure Entra ID.

ddc-app utilise les librairies :
- entity framework pour interfacer la DB
- azure.identity pour l'authentification
- bootstrap pour le css

