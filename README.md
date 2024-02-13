# Amazon_Clone

# What the Project Does
This project is an Amazon-like e-commerce application that provides users with the ability to browse and purchase products, manage their shopping cart, and complete the checkout process. The application includes features such as user authentication, product management, order tracking, and payment processing using the Stripe API.

# Why the Project is Useful
The project is useful for developers looking to understand and implement a full-stack e-commerce application using technologies like React, Node.js, Express, MongoDB, and Stripe. It serves as a practical example of building features such as user authentication, product management, and payment processing within a web application.

# Get Started with the Project
To get started with the project, follow these steps:
1. Make sure you have Node.js installed. 
2. Set up a MongoDB database and obtain the connection URL. You can create a free account on MongoDB Atlas.
3. Clone the Repository
   ```bash
   git clone https://github.com/your-username/amazon-like-ecommerce.git
4. Navigate to the project directory and install the dependencies for both the client and server.
   ```bash
   cd amazon_clone/client
   npm install

   cd ../server
   npm install
5. Update the MongoDB connection URL in the server.js file located in the server directory.
   ```bash
   // server.js
   const connection_url = "YOUR_MONGODB_CONNECTION_URL";
   mongoose.connect(connection_url, {
   useNewUrlParser: true,
   useUnifiedTopology: true,
   });
6. Set up a Stripe account and replace the placeholder Stripe API keys in the server.js and Payment.js files.
   ```bash
   // server.js
   const stripe = require("stripe")("YOUR_STRIPE_SECRET_KEY");

   // client/src/Components/Payment.js
   const promise = loadStripe("YOUR_STRIPE_PUBLIC_KEY");
7. Start both the client and server applications.
   ```bash
   //Client (React App)
   cd ../client
   npm start
   
   //Server (Node.js/Express)
   cd ../server
   npm start
The client application will run on http://localhost:3000 and server will run on http://localhost:8000.
