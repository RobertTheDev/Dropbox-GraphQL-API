# Challenge: Dropbox-Integrated GraphQL API with Next.js and Apollo

## Objective:

Develop a full-stack application that includes a GraphQL API allowing users to authenticate with Dropbox, manage their files, and perform various file operations, integrated with a Next.js front-end using Apollo Client.

## Tasks:

### Setup and Authentication

#### Task 1.1: Environment Setup

- Set up a Node.js environment using Express.js.
- Initialize a new project with appropriate dependencies for GraphQL (e.g., `apollo-server-express`, `graphql`).
- Set up a Next.js project.
- Install Apollo Client and necessary dependencies in the Next.js project.

#### Task 1.2: Dropbox Authentication

- Register your app with Dropbox to get API keys.
- Implement OAuth 2.0 authentication with Dropbox.
- Create a GraphQL mutation `authenticateUser` that initiates the OAuth flow and returns an access token.
- Integrate the authentication flow with the Next.js front-end.

### User Management

#### Task 2.1: User Model

- Design a simple user model to store user data, including the Dropbox access token.

#### Task 2.2: Register and Login

- Implement GraphQL mutations for `registerUser` and `loginUser`.
- Ensure secure password storage and handling using bcrypt or similar.
- Create corresponding pages and forms in Next.js for user registration and login.

### File Operations

#### Task 3.1: List Files

- Create a GraphQL query `listFiles` that returns a list of files and folders in the user's Dropbox.
- Create a Next.js page to display the list of files using Apollo Client to query the GraphQL API.

#### Task 3.2: Upload File

- Implement a GraphQL mutation `uploadFile` that allows users to upload a file to their Dropbox.
- Handle file uploads using Apollo Server's file upload feature.
- Create a file upload form in Next.js.

#### Task 3.3: Download File

- Create a GraphQL query `downloadFile` that generates a temporary link to download a specified file.
- Integrate file download functionality in the Next.js front-end.

#### Task 3.4: Delete File

- Implement a GraphQL mutation `deleteFile` to delete a specified file or folder in the user's Dropbox.
- Add file deletion capability to the Next.js front-end.

### Advanced Features

#### Task 4.1: File Metadata

- Create a GraphQL query `getFileMetadata` to fetch metadata for a specific file (e.g., size, last modified date).
- Display file metadata in the Next.js application.

#### Task 4.2: Sharing

- Implement a GraphQL mutation `shareFile` to create a shared link for a file.
- Add a sharing feature in the Next.js front-end.

#### Task 4.3: Search

- Add a GraphQL query `searchFiles` to search for files within the user's Dropbox by name.
- Implement a search functionality in Next.js.

### Security and Testing

#### Task 5.1: Secure Endpoints

- Ensure that all API endpoints are secured and only accessible to authenticated users.
- Use JWT (JSON Web Tokens) for session management.
- Secure the Next.js pages to ensure only authenticated users can access them.

#### Task 5.2: Unit and Integration Tests

- Write unit tests for individual resolvers.
- Implement integration tests for the overall API functionality using a tool like Jest or Mocha.
- Write tests for the Next.js front-end using a testing library like Jest with React Testing Library.

### Documentation and Deployment

#### Task 6.1: Documentation

- Document your GraphQL schema using tools like GraphiQL or Apollo Server's built-in tools.
- Write a README file explaining the project, setup instructions, and usage examples.
- Document the Next.js front-end setup and usage.

#### Task 6.2: Deployment

- Deploy your GraphQL API to a cloud provider such as Heroku, AWS, or Vercel.
- Deploy the Next.js application to Vercel.
- Ensure that environment variables (such as Dropbox API keys) are securely managed in the deployment environment.

## Evaluation Criteria:

- **Functionality**: The API and front-end should cover all specified tasks and correctly interface with Dropbox.
- **Code Quality**: Clean, readable, and well-documented code with appropriate error handling.
- **Security**: Proper handling of authentication, access control, and data protection.
- **Testing**: Comprehensive tests that cover critical aspects of the API and front-end.
- **User Experience**: Smooth and intuitive interaction with the API and front-end, from authentication to file operations.
- **Deployment**: A live demo of the deployed API and front-end with clear instructions on how to use it.
