# ASP.NetCoreWebAPIwithJWTAuthentication

ASP.NetCore WebAPI with JWT Authentication to access data from MSSQL server.


1. Clone the repository:

   git clone https://github.com/SagarBuchkul/ASP.NetCoreWebAPIwithJWTAuthentication.git
Navigate to the project directory:


cd ASP.NetCoreWebAPIwithJWTAuthentication
Install dependencies:


Update the database connection string in the appsettings.json file:

json

"ConnectionStrings": {
  "DefaultConnection": "YOUR_CONNECTION_STRING"
}
Apply the database migrations:

dotnet ef database update
Usage
Start the API:

dotnet run
Access the API endpoints using a tool like cURL, Postman, or any other HTTP client.

API Endpoints
/api/products: Get a list of products.
/api/products/{id}: Get a specific product by ID.
/api/products/add: Add a new product.
/api/products/{id}/update: Update an existing product.
/api/products/{id}/delete: Delete a product.
[Provide any additional details about your specific API endpoints here.]

Authentication
This project uses JWT (JSON Web Token) authentication.

To obtain an access token, make a POST request to the /api/auth/login endpoint with the following credentials:

Username: Jaydeep
Password: Pass@777
Include the received token in the Authorization header for subsequent requests as Bearer [TOKEN].

Contribution
If anyone wants to contribute to this project or start working with JWT and Redis cache, please feel free to do so. Fork the repository, make your changes, and submit a pull request.
