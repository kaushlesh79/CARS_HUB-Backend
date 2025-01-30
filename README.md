 ### Car Hub Portal - Backend

This is the backend for the Cars Hub Portal, a web application responsible for handling user authentication, car photo uploads, and data management using MongoDB.

## Features
- User authentication (login, registration)
- Upload car photos to the server
- Fetch car photos from the server
- Delete car photos

## Technologies Used
- Node.js
- Express.js
- MongoDB (via Mongoose)
- Multer (for handling file uploads)
- JWT (for authentication)

# Create backend project structure
mkdir -p Car_backend/{config,controllers,models,routes,middleware,uploads}

# Create README.md file
echo "# Car Hub Portal - Backend

This is the backend for the Cars Hub Portal, a web application that handles user authentication, car photo uploads, and data management using MongoDB.

## Features
- User authentication (login, register)
- Upload car photos
- Fetch car photos
- Delete car photos

## Technologies Used
- Node.js
- Express.js
- MongoDB (via Mongoose)
- Multer (for file uploads)
- JWT (for authentication)

## Folder Structure

```
Car_backend/
├── config/                  # Contains database and configuration files
│   └── db.js                # Database connection logic
├── controllers/             # Controller functions for each route
│   └── userController.js    # User-related operations (login, register)
│   └── carController.js     # Car-related operations (upload, fetch, delete)
├── models/                  # Mongoose models for database
│   └── user.js              # User model (for authentication)
│   └── car.js               # Car model (for car photos)
├── routes/                  # Routes for different API endpoints
│   └── userRoutes.js        # Routes for user-related actions (login, register)
│   └── carRoutes.js         # Routes for car-related actions (upload, fetch, delete)
├── middleware/              # Middleware functions (authentication, validation)
│   └── authMiddleware.js    # Middleware for user authentication
├── uploads/                 # Folder where uploaded images are stored
├── .env                     # Environment variables (MongoDB URI, JWT Secret)
├── server.js                # Main entry point for the server
├── package.json             # Project dependencies and scripts
└── README.md                # This file
````

## Setup

### Prerequisites:
- Node.js installed
- MongoDB account (Atlas or local MongoDB setup)

### Install Dependencies:
1. Clone the repository:
   \`\`\`bash
   git clone https://github.com/yourusername/Car_backend.git
   cd Car_backend
   \`\`\`

2. Install the required dependencies:
   \`\`\`bash
   npm install
   \`\`\`

### Environment Configuration:
1. Create a \`.env\` file in the root of the project.
2. Add the following environment variables:

   \`\`\`env
   DATABASE=mongodb+srv://<your_username>:<your_password>@cluster0.mongodb.net/CarsHub?retryWrites=true&w=majority
   JWT_SECRET=<your_jwt_secret>
   \```

Replace `<your_username>` and `<your_password>` with your MongoDB credentials. Replace `<your_jwt_secret>` with a secret string for your JWT token.

### Running the Application:
1. Start the backend server:
   \`\`\`bash
   npm start
   \`\`\`

2. The server will start on port `4006`. You can now interact with the API using tools like Postman or through your frontend application.

### API Endpoints:
- **POST** `/user/api/login`: Login the user.
- **POST** `/user/api/register`: Register a new user.
- **POST** `/cars/upload`: Upload car photos (requires authentication).
- **GET** `/cars`: Get all uploaded car photos.
- **DELETE** `/cars/:id`: Delete a car photo by ID.

## Contributing
Feel free to fork this repository and create pull requests with bug fixes or new features.

## License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details." > Car_backend/README.md

 "Backend folder structure created and README.md file is set up." 

