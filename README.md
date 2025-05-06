## Dorisoy.Pan

Dorisoy.Pan is a cross-platform document management system based on .net core8, using MS SQL 2012 / MySql8.0 (or higher) backend database, you can run it on Windows, Linux or Mac, all methods in the project are asynchronous, support token-based authentication, and the project architecture follows well-known software patterns and best security practices. The source code is fully customizable, hot-swappable and clear architecture, making it easy to develop customized functions and follow any business requirements. The system uses the latest Microsoft technology, high performance stability and security.

### Prerequisites

.NET 7.0+ SDK and VISUAL STUDIO 2019, SQL SERVER, MySQL 8.0

### Server startup steps

1. Using visual studio 2019+, open the solution file "Dorisoy.Pan.sln".

2. Right-click on the solution explorer and restore the nuget packages.

3. Change the database connection string in "appsettings" in the "Dorisoy.Pan.API ​​project.

4. Open the Package Manager Console from "Visual Studio Menu-->Tools-->Nuget Package Manager-->Package Manager Console".

5. In the Package Manager Console, select the default project as "Dorisoy.Pan.Domain".

6. Run the "Update-Database" command in the Package Manager Console to create a database and insert initial data.

7. If your database is MySQL (example), attach the SQL steps under SQL/PROCEDURE-MySQL.sql and rebuild the stored procedure.

8. In the Solution Explorer, right-click "Dorisoy.Pan.API" and click `Set as Startup Item` from the menu.

9. Press F5 to run the project.

### Front-end startup steps

If you don't have nodejs installed yet, download and install nodejs globally: https://nodejs.org , make sure your nodejs version >= 4.0 and NPM >= 3 and install TypeScript globally.

Globally install Angular-CLI command: "npm install -g @angular/cli"

1. Open the project directory "\UI" with visual code.

2. New: Terminal-> "npm install" to initialize the installation of dependencies.

3. Terminal-> "npm run start" to start Angular Server.

4. When ** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ ** is listening, run in the browser.

To run the local copy and build the source in production mode, execute "ng build --prod", which will generate a production version of the application, all html, css and js code are minified and put into the dist folder. This folder can be put into the production server when publishing the application.

### Demo

Demo address: [http://pan.doriso.cn/](http://pan.doriso.cn/)

Default account: admin@gmail.com Password: admin@123

### Project structure

<pre class="prettyprint">

├──Dorisoy.Pan.sln/                     * Solution
│   │
│   ├──Dorisoy.Pan.API                  * REST API Controller, Dependancy configuration, Auto mapper profile 
│   │
│   ├──Dorisoy.Pan.MediatR              * Command handler, Query handler, Fluent API validation
│   │
│   ├──Dorisoy.Pan.Repository           * Each entity repository
│   │
│   ├──Dorisoy.Pan.Domain               * Entity framework dbContext 
|   |
│   ├──Dorisoy.Pan.Common               * Generic repository and Unit of work patterns
│   │ 
│   ├──Dorisoy.Pan.Data                 * Entity classes and DTO classes
│   │
│   ├──Dorisoy.Pan.Helper               * Utility classes

</pre>

### Screenshots

## Desktop client example

<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/desktop1.png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/desktop2.png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/desktop3.png"/>

## Web Client Example

<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(1).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(2).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(3).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(4).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(5).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(6).png"/>
<img src="https://github.com/dorisoy/Dorisoy.Pan/blob/main/Screen/s%20(7).png"/>
