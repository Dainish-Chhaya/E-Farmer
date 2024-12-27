# 🌾 E-Farmer: Online Farming Shopping Portal

## 📄 Project Description
**E-Farmer** is an Online Transaction Processing (OLTP) system designed to directly connect farmers with consumers, eliminating intermediaries. The system streamlines processes such as order management, payment handling, and logistics, fostering transparency and efficiency across the agricultural supply chain.

## 🎯 Objective
The primary goals of this project are to:
- 🛒 Enable farmers to list and sell products directly to consumers.
- 🌐 Provide consumers with an online platform to browse and purchase agricultural goods.
- 🔄 Automate critical processes, including order management, payment processing, and logistics coordination.

## ✨ Key Features
- **Farmer Portal**: Farmers can list products, manage inventory, and track sales.
- **Consumer Portal**: Consumers can browse, search, and purchase products with ease.
- **Order Management**: Includes tracking, payment integration, and logistics.
- **Reports and Analytics**: Provides insights into inventory, sales trends, and top-performing products.
- **Database Views**: Offers valuable insights for better decision-making.
- **Automated Alerts**: Notifications for low stock, pending deliveries, and failed payments.

## 🛠️ Technologies Used
- **Database**: Oracle SQL Developer
- **Backend**: PL/SQL scripts for triggers, procedures, and functions
- **Frontend**: Basic UI setup for database interaction
- **Reporting**: Views and scripts for data analysis
- **Automation**: Triggers for active/inactive status and logistic updates

---

## ⚙️ Project Setup Instructions

### 🛠️ Prerequisite
Ensure that **Oracle SQL Developer** is installed and connected to a valid database connection.

### 🔧 Step-by-Step Setup

#### 1️⃣ **Application Admin Creation**
1. Run `CreateAdminUser.sql` to create the application admin user.
2. Use the credentials generated to establish a connection with the application admin user in Oracle SQL Developer.

#### 2️⃣ **Execute Data Definition Language (DDL) Scripts**
Navigate to the `DDL` folder and execute the scripts in the following order to create the necessary tables:
- `Farmer.sql`
- `Consumer.sql`
- `Product.sql`
- `Inventory.sql`
- `Order.sql`
- `Order_Item.sql`
- `Payments.sql`
- `Logistics.sql`

Then execute the scripts to create views:
- `Consumer_View.sql`
- `Inactive_Products_View.sql`
- `CurrentInventoryStatusView.sql`
- `Discount_On_Perishable_View.sql`
- `WeekWiseSalesView.sql`
- `TopSellingView.sql`
- `PendingDeliveries_View.sql`

#### 3️⃣ **Create Users and Grant Access**
Run `User_grant.sql` to create and grant necessary permissions to standard user roles (farmers, consumers, etc.).

#### 4️⃣ **Execute Sequence Creation Script**
Run `Sequence_Creation.sql` to generate sequences for tables like `Orders`, `Order_Item`, `Payments`, and `Logistics`.

#### 5️⃣ **Execute Data Manipulation Language (DML) Scripts**
Populate the database with sample data by running the following scripts in order:
- `Farmer_Insert.sql`
- `Consumer_Insert.sql`
- `Product_Insert.sql`
- `Inventory_Insert.sql`
- `Order_Insert.sql`
- `Order_Items_Insert.sql`
- `Payments_Insert.sql`
- `Logistics_Insert.sql`

#### 6️⃣ **Execute Trigger Scripts**
Run the following triggers for automated updates:
- `Active_Inactive_Trigger.sql`
- `Logistic_Status.sql`

#### 7️⃣ **Execute Stored Procedures**
Run the following procedures to handle various operations:
- `add_product_proc.sql`
- `low_stock_alert_proc.sql`
- `payment_proc.sql`
- `process_order_proc.sql`
- `update_logistics_proc.sql`

#### 8️⃣ **Execute Functions**
Run the following functions for analytics and insights:
- `get_average_order_value_function.sql`
- `get_category_wise_inventory_function.sql`
- `get_consumer_order_history_function.sql`
- `get_failed_payment_consumer_function.sql`

#### 9️⃣ **Execute Reports**
Generate reports by executing:
- `get_average_order_value_function.sql`
- `get_category_wise_inventory_function.sql`
- `get_consumer_order_history_function.sql`
- `get_failed_payment_consumer_function.sql`

---

## 🌟 Future Enhancements
- **Real-Time Notifications**: SMS and email alerts for orders and payments.
- **Mobile Application**: Extend functionality to mobile platforms.
- **Advanced Analytics**: AI-powered insights for predicting trends and optimizing inventory.
- **Payment Gateway Integration**: Support for popular payment platforms.
- **Improved UI**: Develop a rich and interactive user interface.

## 👥 Contributors 
- **Aravind Ravi**
- **Dainish Chhaya**
- **Divyansh-Jemni**
- **Nidhi Nair**
---

** In case of any questions, please contact me at chhaya.d@northeastern.edu 
