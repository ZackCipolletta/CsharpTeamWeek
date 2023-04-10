# Ecommerce Website

#### An Ecommerce website utilizing an Api to store products and product information.

#### By Zachary Cipolletta, Stephen Zook & James Provance

## Technologies Used

* C#
* .Net 6
* HTML
* JavaScript
* JSON
* SQL
* EFCore
* Identity
* Authentication

## Description


## Setup/Installation Requirements

1. Clone this repo.
2. Open your terminal (e.g., Terminal or GitBash) and navigate to this project's production directory named "E-Commerce_website".
3. Create a file named ['appsettings.json'] in the production directory (E-Commerce_website) and include a new database connection string. The string should be as follows:
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306[Or-Your-Desired-Port-Number];database=[DATABASE-NAME-HERE];uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];",
  }
}
Create a database name, update username and password to match the username and password of your computer.
4. Enter 'dotnet ef database update' in the terminal inside the production directory (this will create the database schema in MySQL which the application will access later), enter 'dotnet run' or 'dotnet watch run' in the command line to start the project in development mode with a watcher (Optionally, you can run "dotnet build" to compile the app without running it). 
5. You will need to clone this repository to your desktop for the back end database: https://github.com/ZackCipolletta/EcommerseApi and follow set up instructions.
6. Once both repositories are up and running users will be able to view and interact with the website.
7. Users are able to browse all products, view products by category, see further details of each product, add and delete them to their shopping cart and even checkout using PayPal.

## Known Bugs
* Once a user checks out using PayPal, the cart does not clear.
* Users are able to register, but they do not seem to be getting saved to the database.  This causes an error as only users who are logged in are able to checkout.
* The footer div containing links to logout and home index and which displays the username/email of a logged in user is not being properly displayed.

## License
MIT

Copyright (c) Zachary Cipolletta, Stephen Zook & James Provance

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.




{
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  },
  "AllowedHosts": "*",
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=ecommercewebsite;uid=root;pwd=epicodus;"
  }

}