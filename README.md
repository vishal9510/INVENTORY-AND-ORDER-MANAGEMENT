Features
User Authentication:

JWT-based authentication.
Role-based access control (Admin and Customer).
Inventory Management:

Admins can create, update, delete, and view products.
Admins can manage stock levels and receive alerts for low-stock products.
Order Processing:

Customers can place orders for multiple products.
Admins can view all orders, and Customers can view their own orders.
Stock levels are automatically updated when an order is placed.

Role-Based Access Control (RBAC)
Admin:

Can manage inventory (create, update, delete, view products).
Can update stock levels and view low-stock alerts.
Can view all orders.
Customer:

Can browse products.
Can place orders for multiple products.
Can view their own orders.

How It Works
User Authentication:

Users sign up or log in to receive a JWT token.
The token is included in the request headers to authenticate API requests.
Middleware verifies the token and assigns roles (admin or customer).
Product Management:

Admins can add, update, delete, and view products.
Products include fields like name, description, price, stock level, and a low-stock threshold.
Stock Management:

Admins can update the stock levels of products.
Low-stock alerts are triggered if a product's stock falls below the defined threshold.
Order Processing:

Customers can place orders for multiple products at once.
The total amount of the order is calculated based on the product prices.
Stock levels are updated accordingly, and low-stock alerts are sent to the admin.
Role-Based Access Control:

Admins have full control over inventory and order management.
Customers can only browse products, place orders, and view their own orders.
