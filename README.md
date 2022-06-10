- 👋 Hi, I’m @congtranna
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
congtranna/congtranna is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Table o## Contributors

|       Name         |  Student ID | Contribution % |
|:-------------------:|:-----------:|:--------------:|
|<a href="=>Trần thành Công</a> | ITITIU19089 |             |

CHAPTER 1- INTRODUCTION	2
1.1.	Motivation	2
1.2.	Problems Statement:	2
1.3.	Scope	3
CHAPTER 2 - LITERATURE REVIEW	3
2.1.	Similar Applications / Systems	3
2.2.	Platform and Tools Review	5
CHAPTER 3 - SYSTEM DESIGN	6
3.1.	System Requirement Specification	6
3.2.	System Design Specification	28
3.2.1.	Use – Case Diagram:	28
3.2.2.	Sequence Diagram:	28
3.2.3.	Activity Diagram:	31
3.2.4.	Entity – Relationship Diagram:	4
3.2.5.	Database Relational Schema	5
CHAPTER 4 - SYSTEM IMPLEMENTATION	5
CHAPTER 5- CONCLUSION	26
REFERENCE	28
1/ Create a blog using PHP and MySQL: https://www.youtube.com/watch?v=OofP9BhzQMU	28
 
CHAPTER 1- INTRODUCTION
1.1.	Motivation:

When deciding where to sell products online, many merchants choose between selling on a marketplace and creating their own website. While each option has its own set of pros and cons – and there is no one-size-fits-all solution that works perfectly for everyone – we believe businesses that are truly serious about ecommerce should have their own website.

Of course, marketplaces (like Amazon, Etsy, eBay, and Walmart Marketplace) can be great sales channels for many merchants, but there are plenty of limitations. And according to BigCommerce’s History of Ecommerce, customers will soon expect to be able to “research, browse, shop, and purchase seamlessly between different devices and on different platforms (like a standalone web store, an Amazon presence, etc.)” — a marketplace alone is not enough.


1.2.	Problems Statement:
Some of the problems that the team will likely encounter throughout the process of developing the project are:
-	Every member is still extremely novice to Web Development.
-	There is not much time since most member have multiple projects to work on during this semester.
 
-	There may be difficulties in designing an attractive website.
-	There may be difficulties in creating a fully functional website.
-	There may be difficulties in connecting the database with the website.
-	There may be difficulties in making a secure website.
-	There may be difficulties in working on the project together since teamwork has never been easy.
1.3.	Scope:
During the project, some of the below issues may have higher chances to be resolved:
-	Get more used to coding and designing web pages.
-	Work together to create a decent looking website (e.g., a website that looks good enough, but not too spectacular).
-	Finish some of the main functionalities of a basic website (e.g., Order, Get Payment, search for items, etc.).
-	Try to understand each other and share the work logically.

CHAPTER 2 - LITERATURE REVIEW
2.1.	Similar Applications / Systems:
There are obviously many websites that provides the same functionalities as our website, and most of them are better in multiple ways:
-	Shoppee https://shopee.vn/
o	Strengths:
	Users can login to an account.
 
	Users have their own account, which can connect to Facebook and Instagram.
	User can find the item via item categories.
	Users can find item via recommendation of “Most search for”.
	Users can download mobile app via QR code on the webpage.
	Users can view some discount packages for many kinds of item.
	Has detailed discount voucher for each item.
	Has many of hot deal.
	User can become a Shopee seller.
o	Weaknesses: There are no significant weaknesses for this website.
-	Tiki: https://tiki.vn/
o	Strengths:
	This webpage has sufficient search bar.
	Has detailed discount voucher for each item.
	Has many of hot deal.
	Detailed homepage.
	Also contains recommendation for each items.
o	Weaknesses: There are no significant weaknesses for this website.
-	Lazada: https://www.lazada.vn/ 
o	Strengths:
	User can login to an account.
	Has a vertical search bar
o	Weaknesses:
	The design is not eye-catching.
	There are no significant weaknesses for this website.
-	Sendo: https://www.sendo.vn/
o	Strengths:
	Has a sufficient search bar.
	Has a chat box for users.
	Has a list recommendation for each item.
	Also has discount voucher, but not too many.
o	Weaknesses:
	The design is quite simplistic, but it is still nice to look at.
	There are no significant weaknesses for this website.
-	And many more…
2.2.	Platform and Tools Review:
-	The programming languages used for this project are:
o	Hyper Text Markup Language (HTML).
o	Cascading Style Sheet (CSS).
o	Structured Query Language (SQL).
o	JavaServer Page (JSP) & Servlet
o	Tomcat 10
 
-	The libraries / platforms used for this project are:
o	JSTL (Javs Standard Tag Library)
-	The tools used for this project are:
o	Visual Studio Code.
o	MySQL.
o	Eclipse
-	Framework:
o	BoostTrap

CHAPTER 3 - SYSTEM DESIGN
3.1.	System Requirement Specification:
List out all of the user’s requirement, which is also the system’s functionalities, in this section.
3.1.1.	Functional Requirements:
- Use case 1: Register

Aspect	System must be able allowed admin and user to log into the system to
perform many actions.
Trigger	When someone attempts to use
system functions.
 
Actors	Customer

Main Success Scenario :
1.	Customer click to the Login page
2.	Login interface is produced.
3.	Customer choose “Sign up” option
4.	Customer fill in email , password and some personal information
5.	Customer click “Sign up” button.
6.	System accept new user and add to database
7.	System displays “successfully sign-up” message.
Alternative Scenarios :
4.1.Customer enter incorrect email:
	+System display message “Email is not exist, please enter again”
4.2Customer enter invalid or empty password
	+System display “Invalid password, please enter again”

- Use case 2: Login

Aspect	System must be able allowed admin and user to log into the system to
perform many actions.
 
	
Trigger	When someone attempts to use
system functions.
Actors	Admin, customer

Main Success Scenario :
1.	User selects a login option.
2.	Login interface is produced.
3.	User enters password and username.
4.	System validates input against system database.
5.	System accepts user type.
6.	System displays “Successfully login” message.
7.	System automatically open home page
Alternative Scenarios :
- Either user name field of password field is empty or contain unaccepted characters. Error message display to verify input:

1.	Let’s user to re-enter username/password.
-	Person use forgot password:
1.	System asked user to recover password
2.	User type new password and answer the security question.
3.	System validates e-mail and display window for them to change their password and system update database if the answer is matched.
-	Username/Password invalid:
1.	System notifies “invalid username/password”.
2.	Let’s user to re-enter login information again.

-	Use case 3: View profile

Aspect	System must be able allowed customer to view their profile

Trigger	When customer click on “View profile”
Actors	Customer
Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “User”.
3.	Customer click on “View profile”
4.	System displays customer profile page.
5.	Customer can choose option “Update information”, “Show information”, “View order detail”
-	Use case 4: Update information

Aspect	System must be able allowed customer to edit information
Trigger	When customer click on “View profile”, choose “Update information”
 
Actors	Customer

Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “View profile”.
3.	Customer clicks on “Update information”.
4.	Customer edit any information of user profile.
5.	Customer clicks on “Update”
6.	System accepts changes and update profile.
-	Use case 4: View Order Detail

Aspect	System must be able allowed customer to view order detail

Trigger	When customer clicks on “View Profile” then click “View order detail”
Actors	Customer
Main Success Scenario :
 
1.	Login the Customer account.
2.	On the header bar. Click on “View profile”.
3.	Admin clicks on “View order detail”.
4.	System displays the list of order that customer made.
5.	System displays all detail information (date, category, payment..)
-	Use case 5: View all product

Aspect	System must be able allowed customer view all product of shop.
Trigger	When customer registered and login into webpage and choose “View all product”
Actors	Customer
Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “View all product”.
4.	System display all type of product.
-	Use case 6: Add product to wish list

Aspect	System must be able allowed customer to add item into wish list.
 
Trigger	When customer choose item and click “Add to wish list”

Actors	Customer

Main Success Scenario :
1.	Login the Customer account.
2.	On the webpage. Click on any item.
3.	Click “add item to my wish list”.
4.	System accepted to add item to wish list.
5.	Customer click view wish list
6.	System display all item added to wish list

Alternative Scenario :

	3.1 Customer click “Remove item from my wish list”.
	4.1 System remove item from wish list	

-	Use case 7: Add Product to Cart

Aspect	System must be able allowed customer to add product into Cart
Trigger	When customer select item and click “Add to Cart”

Actors	Customer
Main Success Scenario :
1.	Login the Customer account.
2.	On the webpage. Select any item.
3.	Click “Add item to my cart”
4.	System accepted to add item to the Cart
5.	Customer click “View Cart”
6.	System display a list of all item in Cart
7.	Customer can choose the payment for all item or remove item from the cart
-	Use case 8: Delete product in cart 
Aspect	System must be able allowed customer to delete product in Cart
Trigger	When customer select item in Cart and choose “remove”
Actors	Customer

Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “dashboard”.
3.	Customer clicks on “Cart”.
4.	Customer select any item in cart
5.	Admin clicks “remove”.
6.	System automatically remove the item.


-	Use case 9: Create Order

Aspect	System must be able allowed customer to make order for products
Trigger	When Customer clicks on “Cart” then click “order”
Actors	Customer
Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “dashboard”.
3.	Customer clicks on “Cart”.
4.	Custom click select all item in Cart and click “Order”
5.	System display cost and payment
6.	System display message “Do you want to make order”
7.	Customer choose “Yes” option
8.	System automatically make an order, set date and asked for customer’s address.
9.	Customer order can be view in “View order detail”
Alternative Scenario :
4.1 If there is no item in Cart. System display “There’s no item in Cart, you cannot make an order”
6.1 If customer choose “Cancel” system won’t make an order
-	Use case 10: Cancel Order

Aspect	System must be able allowed customer to recover password
Trigger	When Customer forgot password, click on “forgot password”

Actors	Customer
Main Success Scenario :
1.	Login the Customer account.
2.	On the header bar. Click on “dashboard”.
3.	Customer clicks on “Cart”.
4.	Custom click select all item in Cart and click “Order”
5.	System display cost and payment
6.	System display message “Do you want to make order”
7.	Customer choose “Yes” option
8.	System automatically make an order, set date and asked for customer’s address.
9.	Customer order can be view in “View order detail”
Alternative Scenario :
4.1 If there is no item in Cart. System display “There’s no item in Cart, you cannot make an order”
6.1 If customer choose “Cancel” system won’t make an order
 
-	Use case 11: Password recovery

Aspect	System must be able allowed customer to recover password
Trigger	When Customer forgot password, click on “forgot password”

Actors	Customer
Main Success Scenario :
1.	Customer open login page.
2.	Choose option “Forgot password”.
3.	Customer retype username.
4.	Customer enter new password.
5.	System display security question.
6.	System compare the to answer saved in database.
7.	Customer answer security question
8.	System confirm and make the change in database.
9.	System return to login page.
Alternative Scenario :
3.1 If username is not correct. System display “Incorrect usename”
4.1 If password is invalid or empty. System display notice.
5.1 If the answer does not matched
6.1 System display “Wrong answer. Try again”
-	Use case 11: Admin Add product

Aspect	System must be able allowed admin to add new product
Trigger	When administrator clicks on “Manage product” click “add new product”

Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	System display add item page
5.	Admin edit any information of the post.
6.	Admin clicks “Add item”.
7.	System accepted and save to the database

-	Use case 12: Remove Product

Aspect	System must be able allowed admin
to remove item 
Trigger	When administrator clicks on “Manage Product” then click “remove item”
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	System display add item page
5.	Admin choose any item
6.	Admin click “Remove item”
7.	System accept and delete item out of database
-	Use case 13: Edit Product

Aspect	System must be able allowed admin to edit new product
Trigger	When administrator clicks on
“Manage Product” then click “Edit product”
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	Admin enters name/id of the product that need to be edited.
5.	Admin edit information (brand, discount, price, status,..)
6.	Admin click “Update product”
7.	System accept and save changed into database.


-	Use case 14: Show all product

Aspect	System must be able allowed admin to show all product
Trigger	When administrator clicks on
“Manage Product” then click “show all product”
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	Admin clicks on “show all product”.
5.	System display all type of product and information
-	Use case 15: Search by Brand/Category
Aspect	System must be able allowed admin to search item by brand/category
Trigger	When administrator clicks on
“Manage product” then click “search” bar
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Search product”.
4.	Admin search brand/category of product on the search bar
5.	System displays all product that matched brand/category


-	Use case 16: Add new category

Aspect	System must be able allowed admin
to add new category
Trigger	When administrator clicks on “Manage product” choose an item and edit its category
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	Admin select an item.
5.	Admin edit new categories
6.	Admin click “Update product”
7.	System accept and save into database
-	Use case 17: Delete category:

Aspect	System must be able allowed admin to delete product categories.

 
Trigger	When administrator clicks on “Manage product” select a product and delete categories.

Actors	Admin

Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	Admin select any product
5.	Admin select any current category.
6.	Admin select “delete”
7.	System accept and remove out of database
-	Use case 18: Add new brand

Aspect	System must be able allowed admin to add new brand to shop
.
Trigger	When administrator clicks on “Manage VN Accommodations”
then click “Add new brand”
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Add new brand”.
4.	Admin enter new brand name
5.	Admin clicks “Update Brand”.
6.	System displays successfully updated message and save new brand to database
-	Use case 19: Delete brand
 
Aspect	System must be able allowed admin to delete brand out of the shop.

Trigger	When administrator select a brand and delete

Actors	Admin

Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage Product”.
4.	Admin search a brand on search bar
5.	Admin select any existed brand.
6.	Admin click “Delete brand”.
7.	System displays successfully message and remove brand from database.
-	Use case 20: Add new security question

Aspect	System must be able allowed admin add new security question
Trigger	When administrator clicks on “Manage user”, choose “Security” , choose add new security question
Actors	Admin
Main Success Scenario :
 
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage User”.
4.	Admin clicks on “Security”.
5.	Admin enter new security question
6.	Admin clicks on “add new security question”.
7.	System accept and add new security question to database.
-	Use case 21: Delete security question

Aspect	System must be able allowed admin
delete a security question
Trigger	When administrator clicks on “Manage user”, choose “Security” , choose a security question to delete
Actors	Admin
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage User”.
4.	Admin clicks on “Security”.
5.	Admin choose a current security question
6.	Admin clicks “delete”.
7.	System accept and remove security question out of database
-	Use case 22: View all customer’s order

Aspect	System must be able allowed admin to view customer’s order
Trigger	When admin click “Manage user”, click “View customer’s order”
Actors	Admin
 
Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage User”.
4.	Admin clicks on “View customer order”.
5.	Admin search a user on search bar and choose him/her
6.	System display that customer information and all order that he/she made
7.	Admin can check status of customer order.
-	Use case 23: Delivery

Aspect	System must be able allowed admin to manage order delivery
Trigger	When user clicks on “Manage user”.
Choose delivery
Actors	Adimin

Main Success Scenario :
1.	Login the Admin account.
2.	On the header bar. Click on “dashboard”.
3.	Admin clicks on “Manage User”.
4.	Admin clicks on “Delivery”.
5.	System display all customer order status.
6.	Admin click “Delivery”
7.	System change order status to delived. And a shipper of shop will automatically get the order.
Alternative Scenario :
	7.1 If customer don’t receive the order. The Order status will change to “Cancel”

 
3.1.2.	Non-functional Requirements:
3.1.2.1	Product Requirements:

Name	Description
Usability Requirements	•	The System shall include 2
types of accounts: Customer and Admin..
•	If a password is forgotten by a system user, they have to recover password by answer security question.
•	Interface action and elements should be consistent.
•	The system should be implemented with simple HTML interfaces for it to be easy to understand and easy to learn.
Efficiency Requirements	•	The system should response to user actions within 20ms
•	The system should handle 100 users/second
Performance Requirements	•	Database processing time
should not exceed 100ms
•	The system shall facilitate data integrity
 










3.1.2.2	Organizational Requirements:

Name	Description
Delivery Requirements	•	The system shall be deployed within six months
•	The system shall be completed within the allocated budget.
Implementation Requirements	•	The system should be implemented with HTML and CSS for interfaces, PHP for sever side scripting, JSP& Servlet, Tomcat for the validation and MYSQL for database management system. 
•	The environment that shall be hosting the system should contain minimum hardware requirements.
•	The environmental that shall be hosting the system should contain minimum software requirements. (Windows 10)

![3.2.1.	Use – Case Diagram:](https://user-images.githubusercontent.com/106094332/173083738-33e6a5af-ac73-4349-8899-1189e65ae0cc.png)
![3.2.2.1.	Login to an Account ](https://user-images.githubusercontent.com/106094332/173089890-7a579ca7-430e-4355-b11b-b4eaad59564d.png)
![3.2.2.2.	Register new account ](https://user-images.githubusercontent.com/106094332/173090034-ca012480-ba71-413e-b293-93167170830a.png)
![3.2.2.3. Password Recovery ](https://user-images.githubusercontent.com/106094332/173090150-af2ec531-7fca-49b0-98c4-8cb789ca6fab.png)
![3.2.2.3.	Password Recovery ](https://user-images.githubusercontent.com/106094332/173090268-cfd131f4-bfe9-4cff-a4f0-b7edd4934473.png)
![3.2.2.4.	Display index page](https://user-images.githubusercontent.com/106094332/173090363-9cb62ecd-37ee-4b7e-80ac-9bd645416834.png)
![3.2.2.5.	Search product](https://user-images.githubusercontent.com/106094332/173090487-24a80854-efe3-46f9-9b03-87abf347b02c.png)
![3.2.2.6.	View detail](https://user-images.githubusercontent.com/106094332/173090623-99d252e4-13af-4e64-af65-12346a99f341.png)
![3.2.2.7.	Add product to wish list](https://user-images.githubusercontent.com/106094332/173090717-bd85c5db-0c64-4eb5-adf2-cbe552e3646c.png)
3.2.3.	Activity Diagram:
![3.2.3.1. Customer register ](https://user-images.githubusercontent.com/106094332/173090814-a3178479-5761-4317-b633-2e904433d33f.png)
![3.2.3.1. Customer Login ](https://user-images.githubusercontent.com/106094332/173090945-132b9110-ade5-456d-90eb-e1a7b2f041d7.png)
![3.2.3.1. Password Recovery](https://user-images.githubusercontent.com/106094332/173091032-f6d0c30c-f4c4-44c7-9e87-0aade6bc6652.png)

![3.2.4.	Entity – Relationship Diagram](https://user-images.githubusercontent.com/106094332/173091145-f64e0052-0947-402c-919a-ab003787b654.png)
![3.2.5.	Database Relational Schema:](https://user-images.githubusercontent.com/106094332/173091271-0390d45a-60e5-496a-8515-dfcbb56c0a8a.png)
CHAPTER 4 -out web
![page](https://user-images.githubusercontent.com/106094332/173091813-703ccd0a-05cc-4055-9aec-b2a09f7fb192.png)
![create account](https://user-images.githubusercontent.com/106094332/173091899-e7155045-3e1d-4acf-b5dd-9151c057777f.png)
![forrget password](https://user-images.githubusercontent.com/106094332/173092118-7111e259-2e3a-40d9-8f5d-304043208b47.png)
![mail check](https://user-images.githubusercontent.com/106094332/173092318-38bfcb28-b7bf-4837-9c46-a6bcab0e0c40.png)
![image](https://user-images.githubusercontent.com/106094332/173092480-94a8758c-b010-4a0b-8cbd-ad35a00809bc.png)
![image](https://user-images.githubusercontent.com/106094332/173092565-e001d044-5d39-4ad3-8415-7ac3e809ba69.png)
![image](https://user-images.githubusercontent.com/106094332/173092631-c92a05ae-ca42-4aea-a7ef-ffa6fa4ff04b.png)
![image](https://user-images.githubusercontent.com/106094332/173092759-e7990257-4ac9-4d19-8acc-2c391f478dec.png)
![image](https://user-images.githubusercontent.com/106094332/173092841-4ccfff4f-9d12-47a8-b887-1357f78fabbd.png)
![image](https://user-images.githubusercontent.com/106094332/173092984-6b7c1348-dd4c-4f0c-8b8f-b4d545e3f17f.png)
CHAPTER 5- CONCLUSION
5.1- Accomplished work:
 
-	The system is able for admin to add/delete product.
-	The system is able for admin to edit product.
-	The system is able for admin to add/delete categories.
-	The system is able for admin to add/delete new brand.
-	The system is able for admin to add/delete new security question.
-	The system is able for admin to manage customer order and delivery
-	The system is able for customer to register and login.
-	The system is able for customer to recovery password of account.
-	The system is able for customer to view profile.
-	The system is able for customer to view product and add to wish list.
-	The system is able for customer to create order.
5.2- Strength and Weakness:

Strength	Weakness
The system is able for users to recovery their password of account	The system does not optimize the comment section.
The system follows MVC model.	Only admin is allowed to delete comment in the database, not in the GUI of the website.
 
The system response quickly to the user’s request.	
The system has friendly GUI of the website.	



5.2- Future work:
-	Improve the comment section.
-	More logical function.
-	More friendly in use of GUI of the website.




REFERENCE
1/ Create a blog using PHP and MySQL: https://www.youtube.com/watch?v=OofP9BhzQMU
2/ PHP Mailer API: https://github.com/PHPMailer/PHPMailer
3/ PHP comment system with reply: https://www.youtube.com/watch?v=eD02QLsTUnY
4/ Trivalgo: https://www.trivago.vn/
5/ Create a Dynamic Blog with PHP and MySQL Database: https://www.youtube.com/watch?v=NCmA1fc_a_g
6/ PHP Forgot(Reset) Password Recover Code Using PHPMailer SMTP: https://www.youtube.com/watch?v=5yIqJSflMsY










