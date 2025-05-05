Inventory System

User Requirements:
To create a web application using Flask framework to manage inventory of a list of products in respective warehouses. Imaging this application will be used in a shop or a warehouse that needs to keep track of various products and various locations.
Inventory Management Web Application :
In the inventory Shop it contains product,location and product movements and show the Transactions Report.
•	I Had Successfully created the product.html page in that the user can add product name and Quantity if they wants to modify they can do in that pages.
•	In Location page  as successfully add their Location and modify in the Locations in Location.html
•	I had created product movement.html for showcasing the Transactions and Transaction history in that page.
Features I’m Added:
•	Login and Signup(By Hashing technique)
•	Search in Transactions by product name or Warehouse.
•	Easy Navigations
•	Using Sqlite Database.
•	Can easily Modify The Product Details and Location Details.
•	Bootstrap Styles are Used in Web pages.





File Paths:
├── aerele\
│   ├── __init__.py          # Flask app initialization
│   ├── models.py            # Database models (Product, Location, ProductMovement, User)
│   ├── routes.py            # Application routes and logic
│   ├── templates\           # HTML templates for the app
│   │   ├── signup.html      # Signup page template
│   │   ├── login.html       # Login page template
│   │   ├── product.html     # Product listing page
│   │   ├── location.html    # Location listing page
│   │   ├── movement.html    # Product movement page
│   │   ├── edit_product.html # Edit product page
│   │   ├── edit_location.html # Edit location page
│   │   ├── search_results.html # Search results page
│   ├── static\              # Static files (CSS, JS, images)
│   │   ├── back.jpg         # Background image
├── migrations\              # Database migration files
│   ├── versions\            # Individual migration scripts
│   │   ├── ...              # Migration file
├── requirements.txt         # Python dependencies
├── config.py                # Configuration file (if applicable)
└── run.py                   # Entry point to run the Flask app

Steps To Run the Application:
Step1: Extract the Zip File 
Step2: Migrate the Sqlite Database in Your System
•	flask --app aerele db init
•	flask --app aerele db migrate -m "Initial migration"
•	flask --app aerele db upgrade
Step 3: Import the Necessary Flask files in cmd.
Step 4: Run the Application 
•	python appname.py(python app.py)
Screenshots:
1.	First it Ask the User Details to Allow in Inventory Shop.
![image](https://github.com/user-attachments/assets/112bc648-5e5f-4f7f-bbd0-a95a61dd8909)

2.If the user details Are correct it will navigate to Base.html File
![image](https://github.com/user-attachments/assets/fb2419b0-76b6-4e61-b2df-4eb258e15b02)

3.After that we can add the products in product.html 
![image](https://github.com/user-attachments/assets/e0fc06cc-c5fd-489d-a9c9-5ad376dc08a8)

4.In sidebar if we click the Location It will navigate to the Location page and show the Available Locations I we need to Add Any new Locations.
![image](https://github.com/user-attachments/assets/3e36e5a0-1c94-46f1-af3d-a19b001dc918)

It Successfully Added the New Location Thiruvannamalai
![image](https://github.com/user-attachments/assets/4b2ff473-7865-4343-b235-b0322eea8e74)

5.Products Movements (Make Transactions and Available balances in Hub and Transaction History)
There are three type Of Transactions
1.Unknown to Hub (it reduces the Original product Quantity)
Example: I’m entered tomato As 100 Quantity
![image](https://github.com/user-attachments/assets/f4e8e52c-c2ba-47e4-84c9-a2671adea5bb)

I am moving 50 Quantity in(unknown to Hub) Transaction
![image](https://github.com/user-attachments/assets/daa4c3db-0ec5-4092-b43d-44ef87935107)

It successfully Transferred to Hub And shown in product balances and updated in Transaction history.
![image](https://github.com/user-attachments/assets/8f4bf776-2a7c-4211-8f75-157901c97f3a)

It also updated Remaining Available Quantity in product page I moved 50 quantity the Remaining will be updated successfully.
![image](https://github.com/user-attachments/assets/5548832d-654f-4eed-9524-1b63d66bd7cc)

 Type 2:(Hub to Hub)
In Hyderabad hub contains 50 quantity I move the 25 quantity to Coimbatore Hub.
![image](https://github.com/user-attachments/assets/c66f3179-676b-4647-a39c-7b9a58f88a23)
it successfully transferred Hyderabad hub to Coimbatore hub.
![image](https://github.com/user-attachments/assets/f54b79e8-37e2-4801-91ab-65e39a6ec348)
Type 3:(Hub to Consumer)
The Coimbatore hub Contains 25 quantity I want to sell 20 Quantity to consumer .
![image](https://github.com/user-attachments/assets/387a0cef-9206-4222-854e-f9d3ac9e82e5)

It successfully updated Coimbatore hub quantity as 5 and the product is selled in Coimbatore.

If we want to search the transaction history by product or Ware House:
Example :in search box I’ll entered “Tom” and click entered the result page will show like this.
![image](https://github.com/user-attachments/assets/5719ab40-91f2-444f-81b9-14be1e073565)
Hence all the Actions are done in the given Requirements and I add the few more features for user Flexibility .

Referances:
1.Bootsrap Styles – For user interface and styling.
2.For Developing This Application – WaterFall model in (OOSE-CCS356 (Anna University))
•	This model the Development starts Requirements gathering phase.
•	Then process analysis,design,coding,testing and Maintenance.

