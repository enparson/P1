# RoSA
## RoSa, or Robotic Shopping Assisant, is a UiPath automation that shops for a vendor utilizing the Pega training website.
RoSA is your robotic shopping assistant, here to help you automate your shopping business. RoSA helps you shop for all your customers from online vendors. It provides customers individual expense reports sent via email. 
## Technologies Used
UiPath Studio 2020.10.7 <br>
Azure Data Studio/Microsoft Azure Portal<br>
Pega Training Website <https://training.openspan.com/login>
## Features
### Current Features
- Takes in customer shopping lists from excel files
- Shops for customer orders in the Pega platform.
- Uses customer information on file within SQLserver database for the client
- Records the expenses alongside base service fee and commission fee in a receipt as a .xlsx file and emails that to the client
- Emails the receipts to shopper for profit report
- Sends customers' order numbers to be stored in the database

### Future Improvements
- Store customers' individual orders within database
- Retrieve customer data into a simplified profit report to email to shopper

## Getting Started
- git clone https://github.com/enparson/P1.git
- open file Connect2DB.xaml
- edit "Connect to Database" and "Run Query" UiPath activities to connect to client SQLserver Database
- ensure SQLserver database client's customer information is stored in tables with columns in the following order: <br> ([Customer Id],[Customers], [Email], [Street Address], [Zip Code], [Primary Phone], [Card Numbers], [CVV], [Card Type], [Expiration Month], [Expiration Year])
- edit "CustomersDesire - Copy.xlsx" with customer shopping lists

## Usage
- open file actualorder.xaml with UiPath Studio
- under Debug File command, select Run File <br>
![Screenshot (15)](https://user-images.githubusercontent.com/91700281/174115444-24745da5-4462-4e3a-9b77-a44164e3e015.png)

## License
This project uses the following license: [MIT License](https://github.com/enparson/P1/blob/main/LICENSE).
