# Online-store-api

Online Store Flask-Smorest API
This is an online store API built using Flask-Smorest, a Flask extension for building RESTful APIs with OpenAPI (formerly known as Swagger) documentation.

Features
The online store API provides the following features:

Product management: CRUD operations for managing products, including creating, updating, retrieving, and deleting products.
Order processing: Ability to add products to a cart, place orders, retrieve order history, retrieve order details, and cancel orders.
Authentication and authorization: User registration, login, and logout using JWT (JSON Web Token) for authentication and authorization.
Comprehensive documentation: Automatically generated OpenAPI documentation for all API endpoints with detailed information about parameters, responses, and authentication requirements.
Installation
To install and run the online store API, follow these steps:

Clone the GitHub repository:
bash
Copy code
git clone https://github.com/Emetegift/online-store-api.git
Change to the project directory:
bash
Copy code
cd online-store-api
Create a virtual environment (optional but recommended) and activate it:
bash
Copy code
python -m venv venv
source venv/bin/activate (for Mac/Linux)
venv\Scripts\activate (for Windows)
Install the required dependencies:
Copy code
pip install -r requirements.txt
Set up the environment variables:

SECRET_KEY: Secret key for Flask app
DATABASE_URL: URL of the database (SQLite)
FLASK_APP: Name of the Flask app ( app.py)
Make sure to configure these variables with appropriate values before running the API in your environment.

Usage
The online store API provides various endpoints for managing products, processing orders, and handling authentication. Here are some examples of how to use the API:

Product Management:

Create a new product: Send a POST request to /api/products with the product details in the request body.
Update a product: Send a PUT request to /api/products/{product_id} with the updated product details in the request body.
Retrieve a product: Send a GET request to /api/products/{product_id} to retrieve the details of a specific product.
Delete a product: Send a DELETE request to /api/products/{product_id} to delete a specific product.


Add products to cart: Send a POST request to /api/cart with the product details in the request body to add products to the cart.
Place an order: Send a POST request to /api/orders with the order details in the request body to place an order.
Retrieve order history: Send a GET request to /api/orders to retrieve the order history of the authenticated user.
Retrieve order details: Send a GET request to /api/orders/{order_id} to retrieve the details of a specific order.
Delete an order: Send a DELETE request to /api/orders/{order_id} to cancel a specific order.
Authentication and Authorization:

Register a new user: Send a POST request to /api/auth/register with the user details in the request body to register a new user.
Login: Send a POST request to /api/auth/login with the user credentials in the request body to obtain a JWT token for authentication.
Logout: Send a POST request to /api/auth/logout to logout the authenticated user.
