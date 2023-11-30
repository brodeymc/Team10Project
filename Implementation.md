# Computer World:
Welcome to Computer World our E-Commerce computer parts store! This Java-based application provides a user-friendly interface for buying computer parts. Users can create an account, browse through a variety of computer components, and make purchases securely. The application uses MySQL for data storage and Swing for the graphical user interface.

## Table of Contents
- [General Information](https://github.com/brodeymc/Team10Project/blob/main/Implementation.md#general-informartion)
- [Technologies Used](https://github.com/brodeymc/Team10Project/blob/main/Implementation.md#version-1-technology)
- [Features](https://github.com/brodeymc/Team10Project/blob/main/Implementation.md#features)
- [Environment Requirements](https://github.com/brodeymc/Team10Project/blob/main/Implementation.md#environment-requirements)
- [Application Cloning Steps](https://github.com/brodeymc/Team10Project/blob/main/Implementation.md#cloning-steps)
- [Source Code]()

### General Informartion
- We aimed to make something that people could use to find every and any computer part
- It acts as a sort of amazon, but instead for computer parts
- Our goal wasn't to just create an application that sold items, but to make something people would recommend to their friends

### Version 1 Technology
- Our language for Version 1 was java
- We used swing for the first version, but that could possibly change going forward
- SQL is what we used for our storage plan and that will probably remain the same for all versions

### Features
- User Registration: Create a personalized account by choosing a unique username and password. Your information is securely stored for future visits.
- Browse and Shop: Explore our extensive collection of computer parts, from powerful processors to sleek graphics cards. Our intuitive interface makes it easy to find the perfect components for your setup.
- Cart Management: Add items to your cart and review your selection before making a purchase. Experience a hassle-free shopping journey with our straightforward checkout process.
- Shipping Information: Provide your shipping and contact details during checkout to ensure a smooth delivery process. We value your time and convenience.
- Reciepts: At the end of every transaction the user will be prompted with a reciept of the transaction, shipping info, contact info which was provided, and few other small things.
- Admin Powers: There will be admins that will have some extra abilities such as running sales reports, changing inventory, and making other users into admins.

### Environment Requirements
- This can be run on all of the following operating systems:
  - Apple macOs
  - Microsoft Windows

### Cloning Steps
The following steps all assume that you have an IDE for whatever language you plan on coding in and as well as access to all the other proper technology, they will also be based off our experience and the technologies we used:
1. Clone the repository
2. Set Up MySQL Database:
    - Install MySQL on your machine if not already installed, you can download it from MySQL Downloads.
    - Start your MySQL server.
    - Connect to MySQL and create a new database for the application. 
3. Database Schema Scripts:
    - Navigate to the database-scripts folder in the project
    - Run the SQL scripts in numerical order to set up the necessary tables and data. You can use a MySQL client
4. Database Configuration:
    - Open the src/main/resources/config.properties file using your favorite text editor or IntelliJ IDEA.
5. Open Project in IntelliJ IDEA:
    - Open IntelliJ IDEA.
    - Choose "Open" from the welcome screen and select the cloned ecommerce-computer-parts directory.
6. Configure Project SDK:
    - Make sure your project SDK is set to JDK 8 or later:
    - Open IntelliJ IDEA settings (File -> Project Structure).
    - Under "Project," ensure the Project SDK is set to JDK 8 or later.
7. Build and Run:
    - In IntelliJ, navigate to the ECommerceApp class (src -> main -> ECommerceApp.java).
    - Right-click on the file and select "Run ECommerceApp.main()" or use the green arrow next to the main method.
8. Test User Authentication:
    - In the application's login page:
    - Use the username: user and password: password for regular user access.
    - Use the username: admin and password: password for admin/sales report access.
9. Explore and Use the Application:
    - Explore the inventory, add items to the shopping cart, and proceed through the checkout process.
    - For admin access, log in with admin credentials and explore the sales report.




