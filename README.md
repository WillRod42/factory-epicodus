# Hair Salon

#### By William Rodriguez

## Technologies Used

* HTML
* Bootstrap
* .NET Core
* ASP.NET
* Entity Framework Core
* MySQL

## Description

A web-app that keeps track of a factory's engineers, machines, and which engineers can repair which machines.

## Setup/Installation Requirements

### Setup Repository
* Clone this repository to your desktop or any directory of your choice
  * Run the command below in a bash terminal with [git](https://github.com/git-guides/install-git) installed
```
git clone https://github.com/WillRod42/factory-epicodus.git
```
* Or download as a zip file
  * Click the green code button on the repository page
  * At the bottom of the popup window select `Download ZIP`
  * Extract the downloaded .zip folder
* Make sure you have the [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) installed and setup correctly for your OS
* Open the `Factory` folder of the downloaded repsoitory
* Run these commands in a terminal
  ```
  dotnet restore
  dotnet build
  dotnet run
  ```
* This will open a live instance of the web-app at [http://localhost:5000](http://localhost:5000)

### Setup MySQL Server
* Download and install the version of [MySQL](https://dev.mysql.com/downloads/mysql/) for your OS
* Inside the `Factory` folder, create a file named `appsettings.json`
  * Inside add these lines and save the file
  ```
  {
    "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=<database name here>;uid=<username here>;pwd=<password here>;"
    }
  }
  ```
* Run this command in a terminal at this location
  ```
  dotnet ef database update
  ```

## Known Bugs

* None

## License

MIT

Copyright (c) 2022 William Rodriguez