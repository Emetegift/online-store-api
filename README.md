# Online Store API

This project is an online store API built with Flask-Smorest and tested with Insomnia. It provides endpoints for managing products, customers, and orders for an online store.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python 3.6 or higher
- pip

### Installation

1. Clone the repository
```
git clone https://github.com/yourusername/online-store-api.git
```

2. Install the required packages
```
pip install -r requirements.txt
```

3. Set up the database
```
flask db upgrade
```

4. Start the server
```
flask run
```

## Usage

### Endpoints

The following endpoints are available:

#### Products

- GET `/api/products`: get all products
- GET `/api/products/{id}`: get a single product by ID
- POST `/api/products`: create a new product
- PUT `/api/products/{id}`: update a product by ID
- DELETE `/api/products/{id}`: delete a product by ID

#### Customers

- GET `/api/customers`: get all customers
- GET `/api/customers/{id}`: get a single customer by ID
- POST `/api/customers`: create a new customer
- PUT `/api/customers/{id}`: update a customer by ID
- DELETE `/api/customers/{id}`: delete a customer by ID

#### Orders

- GET `/api/orders`: get all orders
- GET `/api/orders/{id}`: get a single order by ID
- POST `/api/orders`: create a new order
- PUT `/api/orders/{id}`: update an order by ID
- DELETE `/api/orders/{id}`: delete an order by ID

### Authentication

Authentication is required to access the API. To authenticate, send a POST request to `/api/auth/login` with a JSON body containing your username and password. The response will include a JWT access token, which should be included in the `Authorization` header of subsequent requests with the prefix `Bearer ` (including the space).

### Documentation

The API documentation is available at `/api/docs`. It was automatically generated by Flask-Smorest from the OpenAPI schema. You can also view and test the API endpoints from this page.

## Testing

The API can be tested using Insomnia. Import the `insomnia.json` file into Insomnia to use the preconfigured requests. The API must be running locally for the requests to succeed.

## Built With

- Flask - Web framework
- Flask-Smorest - Flask extension for building RESTful APIs with OpenAPI/Swagger documentation
- SQLite - Database engine

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
