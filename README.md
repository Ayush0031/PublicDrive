# PublicDrive

## Overview
PublicDrive is a **cloud-drive alternative** developed as part of the **CDAC AAI team**. Instead of relying on external cloud servers, PublicDrive utilizes the user's local file system for storage. It enables **file uploads, sharing, and access control** while ensuring security through **JWT-based authentication**.

## Features
- **File Management**: Upload, edit, share, and delete files securely.
- **Local Storage**: Uses the local file system instead of cloud-based storage.
- **JWT Authentication**: Ensures secure access to user data.
- **Role-Based Access Control (RBAC)**: Different user roles with specific permissions.
- **Access Control**: Users with granted permissions can edit or view files.
- **Modern Tech Stack**: Built using **React, Redux Toolkit, MUI, Spring Boot, and MySQL**.

## Tech Stack
### Frontend:
- **React**: Component-based UI development.
- **Redux Toolkit**: State management.
- **Material-UI (MUI)**: UI components for a modern look.

### Backend:
- **Spring Boot**: Backend API development.
- **JWT Authentication**: Secure user authentication.
- **MySQL**: Relational database for file metadata storage.

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- **Node.js** (for frontend)
- **Java 17+** (for backend)
- **MySQL** (for database)

### Backend Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/ayush0031/publicdrive.git
   cd publicdrive/backend
   ```
2. Configure MySQL database:
   - Create a new database named `publicdrive`.
   - Update `application.properties` with your MySQL credentials.
3. Build and run the Spring Boot application:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

### Frontend Setup
1. Navigate to the frontend folder:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the React application:
   ```bash
   npm start
   ```

## Usage
1. **User Authentication**: Sign up or log in using JWT-based authentication.
2. **Upload Files**: Securely upload files from the local system.
3. **Manage Access**: Assign permissions for file sharing and editing.
4. **View & Edit**: Users with access can edit shared files.

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/api/auth/login` | User login |
| POST   | `/api/auth/signup` | User registration |
| POST   | `/api/files/upload` | Upload a file |
| GET    | `/api/files/{id}` | Get file details |
| PUT    | `/api/files/edit/{id}` | Edit file (if authorized) |
| DELETE | `/api/files/delete/{id}` | Delete a file |

## Contributing
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`.
3. Commit changes: `git commit -m "Your commit message"`.
4. Push to the branch: `git push origin feature-branch-name`.
5. Submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For queries or contributions, reach out via GitHub Issues.




