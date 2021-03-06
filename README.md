# Eau Claire's Salon

### A Week X Epicodus Project, 21 May 2021

_By Jonathan Stull_

## **Description**

[Eau Claire's Salon](https://github.com/jonathanstull/HairSalon.Solution.git) required an app to manage its many (theoretical) stylists and clients. This application allows the owner of Eau Claire's Salon, Claire, to add new stylists, manage their contact information and contract-related information, assign them new clients, and manage client contact information and appointment history.

## **Setup/Installation Requirements**

* Software requirements (internet browser, code editor, etc.)
  1. Internet browser
  2. A code editor like VSCode or Atom to view or edit the codebase

* Download/clone instructions
  1. Download this repository onto your computer by clicking the 'code' button
  2. Open the project folder.

* Open via Bash/GitBash:
  1. Clone this repository onto your computer: `git clone https://github.com/jonathanstull/HairSalon.Solution.git`
  2. In a terminal window, navigate into the `~/HairSalon.Solution` directory and open in VSCode or preferred text editor with the command `code .`
  3. This project uses C#/.NET. To build and execute the code, use the command `dotnet run`

* Setting up a MySQL database
  1. Download and install MySQL and MySQLWorkbench in accordance with [this tutorial](https://www.learnhowtoprogram.com/c-and-net/getting-started-with-c/installing-and-configuring-mysql)
  2. Open MySQLWorkbench and navigate to the **Administration** tab in the left-hand panel
  3. Under **Management**, select **Data Import/Restore**
  4. Select **Import from Self-Contained File** and open the dump file in the root directory of this project by navigating to `~/HairSalon.Solution/jonathan_stull.sql`
  5. **Do not select a Default Target Schema.** `jonathan_stull.sql` contains MySQL command lines that will create a schema for you upon import
  6. Select **Start Import**
  7. Add a `.appsettings.json` file to specify the MySQL database using the following settings (please note that **you must change `[YOUR_USERNAME]` and `[YOUR_PASSWORD]`** to reflect your user information):
  
    ```
    {
    "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=jonathan_stull;uid=[YOUR_USERNAME];pwd=[YOUR_PASSWORD];"
      }
    }
    ```


## **Known Bugs**

* **v. 0.9**
  * Application unsuccessfully integrates SCSS and global CSS stylesheets

## **Specs**

* The salon owner needs to be able to see a list of all stylists
* The salon owner needs to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist
* The salon owner needs to add new stylists to our system when they are hired
* The salon owner needs to be able to add new clients to a specific stylist and should not be able to add a client if no stylists have been added

## **Technologies Used**

* C#/.NET
* MySQL and MySQLWorkbench
* Entity Framework Core (5.0.0) and Pomelo (5.0.0-alpha.2)
* HTML/CSS
* VS Code
* Google Chrome/Mozilla Firefox

## **MIT License**

Copyright (c) 2021 Jonathan Stull

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## **Contact Information**

If you are interested in this work, please reach out to Jonathan at <jonathan.d.stull@gmail.com>.