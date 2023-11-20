# Data Storage Plan
  This document will explain how our application will store data, as well as describe the libraries and technologies we go with. It's all listed below:
  
  
  1. Data Storage Choice:
     - **SQL Database**: Utilize a SQL relational database for persistent data storage.

  2. Database Technology:
     - **Microsoft SQL Server**: Choose Microsoft SQL Server as the specific SQL database, suitable for Windows environments.

  3. Swing Data Access Framework:
     - **Table Model Interface**: Implement a custom TableModel interface to represent product data, manage interactions between Swing components, and connect with the underlying Microsoft SQL Server database.
     - **Abstract Table Model**: Extend AbstractTableModel to provide a basic implementation of the TableModel interface for product data.

  4. Swing Components for E-Commerce Features:
     - **JTable**: Use JTable to display products, orders, and other relevant information.
     - **JTextFields, JComboBox, etc.**: Implement various Swing components for capturing user input related to product details, orders, and customer information.

  5. Database Initialization:
     - **SQL Script**: Create an SQL script to define the initial database schema, including tables for products, orders, and customers, and populate essential data.
     - **Initialization Code**: Develop Java code, integrated with Swing, to execute the SQL script during the application startup to ensure data availability.

  6. Connection Pooling and Data Access:
     - **Not Applicable**: As in the previous plan, direct data manipulation through Swing components doesn't necessitate a separate connection pooling library.
     - **Swing Actions**: Implement Swing Action classes to handle user actions (e.g., adding products to the cart, placing orders) and directly manipulate the underlying product and order data.

  7. Object-Relational Mapping (ORM):
     - **Custom Mapping**: Implement custom mapping logic within Swing components to map data between the e-commerce interface and the Microsoft SQL Server database, especially for products, orders, and customer information.

  8. Data Access Layer with Swing:
      - **Swing GUI Classes**: Organize Swing GUI classes to act as a presentation layer, handling user input, displaying product information, managing shopping carts, and directly interacting with the SQL database for order processing.

  9. Transaction Management:
     - **Swing Actions**: Implement transactional logic within Swing Action classes to ensure data consistency and integrity during complex order processing.

  10. Data Encryption:
      - **Optional**: Depending on the sensitivity of data, consider using Java cryptography libraries to encrypt and decrypt sensitive information, especially customer and order details.

  11. Data Migration and Seeding:
      - **Swing Initialization Logic**: Develop mechanisms within Swing components to seed initial product data into the Microsoft SQL Server database during the application's first launch.

  12. Backup and Recovery:
      - **Scheduled Backups**: Implement a scheduled backup mechanism within Swing components to periodically back up the SQL database, especially critical data like order history.
      - **Recovery Strategy**: Document a recovery strategy within Swing components to restore the SQL database in case of data loss.

  13. Logging:
      - **Log4j (Optional)**: Integrate Log4j within Swing components for logging user actions, errors, and other relevant events during e-commerce transactions.

  14. Scalability:
      - **Connection Pool Configuration (if needed)**: If scalability requires additional connections, consider configuring a connection pool (integrated with Swing) to handle increased demand, especially during peak shopping periods.

  15. Documentation:
      - **Javadoc**: Maintain comprehensive Javadoc documentation for Swing classes, methods, and data access logic.
      - **Database Schema Diagram**: Include a visual representation of the database schema within the Swing application for better understanding, emphasizing tables for products, orders, and customers.
