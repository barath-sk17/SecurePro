
# Secure Pro File Sharing System

The Secure Pro File Sharing System is a robust web application designed to facilitate seamless collaboration and secure file sharing among users within groups. Built with a strong emphasis on security and user privacy, the system employs modern technologies and best practices to ensure data integrity and confidentiality.

## Key Features

### User Management
- Users can sign up by providing their username, full name, and password.
- User credentials are securely stored in a MongoDB database using salted and hashed passwords for enhanced security.
- Upon signup, user details are sent to the admin for approval.

### Admin Approval
- The system includes an admin role with complete control over user management and group creation.
- The admin reviews user signup requests and can approve or deny them based on discretion.

### Group Creation
- Once approved by the admin, users can create groups within the system.
- Group creation requests are also sent to the admin for approval.
- Upon approval, users can create groups and collaborate within them securely.

### File Storage
- Files uploaded by users are securely stored in Amazon S3 buckets, ensuring reliability, scalability, and durability.
- Access to files is restricted based on user permissions within the group.

### Admin Privileges
- The admin has complete control over the application, including the ability to deactivate groups, manage user accounts, and enforce security policies.

## Tech Stack

### Backend
- Built using Express.js, a fast, unopinionated web framework for Node.js.
- Express provides a robust foundation for building RESTful APIs and handling user authentication.

### Database
- MongoDB is used as the database system for storing user credentials, group information, and other application data.
- MongoDB's flexibility and scalability make it well-suited for managing dynamic data structures.

### File Storage
- Amazon S3 (Simple Storage Service) is utilized for secure file storage, providing high availability, durability, and scalability for storing and retrieving files uploaded by users.

## Getting Started

To get started with the Secure Pro File Sharing System, follow these steps:

1. Clone the repository to your local machine.
2. Install the necessary dependencies using npm or yarn.
3. Set up a MongoDB instance for storing application data.
4. Configure environment variables for MongoDB connection and Amazon S3 credentials.
5. Run the application locally using `npm start` or `yarn start`.

## Contributing

Contributions are welcome! If you'd like to contribute to the Secure Pro File Sharing System, please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with descriptive messages.
4. Push your changes to your fork.
5. Submit a pull request to the main repository.
