# Flipr Placement – Backend Development Task

## Overview
This project implements the frontend and backend for an **e-commerce platform**, providing core functionalities such as user authentication, product management, cart management, and order management. The backend is designed to be robust, scalable, and secure, handling typical operations required for an e-commerce application.

---

## Live Demo
[Click here to visit the website](https://ietianswear.netlify.app)


## Features

### Authentication
- **Sign Up** (`POST /signup`): Allows new users to register with their name, email, password, and optional address.
- **Sign In** (`POST /signin`): Enables existing users to log in and receive a session token.

### Product Management
- **Add Product** (`POST /addproduct`): Add new products with details like name, description, price, and category.
- **Update Product** (`PUT /updateproduct/:productId`): Update product details by its unique ID.
- **Delete Product** (`DELETE /deleteproduct/:productId`): Remove a product from the platform.
- **Get All Products** (`GET /products`): Fetch all available products.

### Cart Management
- **Add Product to Cart** (`POST /cart/add`): Add a product to the cart or update its quantity if already in the cart.
- **Update Cart** (`PUT /cart/update`): Modify the quantity of a product in the cart or remove it if the quantity is set to zero.
- **Delete Product from Cart** (`DELETE /cart/delete`): Remove a specific product from the cart.
- **Get Cart** (`GET /cart`): Retrieve all items in the customer’s cart along with the total cost.

### Order Management
- **Place Order** (`POST /placeorder`): Finalize the purchase of items in the cart, capturing shipping details and generating an order ID.
- **Get All Orders** (`GET /getallorders`): Fetch all orders, including customer and product details (admin feature).
- **Get Orders by Customer ID** (`GET /orders/customer/{customerId}`): Retrieve all orders specific to a customer.

---

## Tech Stack
- **Backend Framework:** Node.js with Express.js  
- **Database:** MongoDB  
- **Authentication:** JSON Web Tokens (JWT) and bcrypt for password hashing  
- **API Documentation:** Postman  

---

## Installation

1. **Clone the repository:**
 
   git clone <repository-url>
   cd <project-folder>

2. **Set up Environment Variables**
   Create a .env file in the root directory
   Add the following variables:

  MONGO_URI=<your-mongodb-connection-string>
  JWT_SECRET=<your-jwt-secret-key>
  PORT=<port-number>
  
3. **Start the Server:**
   npm start








   

   

   
