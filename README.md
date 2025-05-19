# Place-Log: A Place Review and Logging Web Application

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-green)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-orange)

## Overview
Place-Log is a web application built with Flask and MongoDB that allows users to log and review places they have visited. Users can create accounts, add places with details (e.g., name, location, rating, comments), and view their logged places. The application demonstrates a full-stack development approach, integrating a Python backend, MongoDB for data storage, and a responsive frontend.

This project showcases skills in web development, database management, user authentication, and deployment, making it relevant for roles in e-commerce and technology-driven companies.

## Features
- **User Authentication**: Secure sign-up and login functionality using password hashing.
- **Place Logging**: Add, edit, and delete place entries with details like name, location, rating, and comments.
- **MongoDB Integration**: Store and retrieve place data efficiently using MongoDB.
- **Responsive UI**: A clean, user-friendly interface built with HTML, CSS, and Bootstrap.
- **RESTful API**: Backend endpoints for CRUD operations on place data.

## Architecture
The application follows a client-server architecture:

![Place-Log Architecture](docs/architecture-diagram.png)

*Note*: Replace `docs/architecture-diagram.png` with an actual diagram created using tools like Draw.io or Lucidchart.

## Prerequisites
To run the project locally, ensure you have:
- Python 3.8 or higher
- MongoDB installed locally or a MongoDB Atlas account
- Git installed
- A code editor (e.g., VS Code)

## Installation and Setup
Follow these steps to set up and run Place-Log:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/nikhal99/Place-Log.git
   cd Place-Log
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure MongoDB**:
   - Set up a local MongoDB instance or create a MongoDB Atlas cluster.
   - Update the MongoDB connection string in `app.py` or use an environment variable:
     ```bash
     export MONGO_URI="mongodb://localhost:27017/placelog"  # Replace with your URI
     ```

5. **Run the Application**:
   ```bash
   python app.py
   ```
   Open `http://localhost:5000` in a browser to access the application.

## Repository Structure
```
Place-Log/
├── static/                   # CSS, JavaScript, and image files
│   ├── css/
│   ├── js/
├── templates/                # HTML templates for Flask
│   ├── index.html
│   ├── login.html
│   ├── register.html
├── app.py                    # Main Flask application
├── requirements.txt          # Python dependencies
├── docs/                     # Documentation and diagrams
│   ├── architecture-diagram.png
├── README.md                 # Project documentation
├── LICENSE                   # License file
```

## Usage
- **Register**: Create an account with a username and password.
- **Log In**: Access your account to manage place entries.
- **Add Place**: Submit details like place name, location, rating, and comments.
- **View Places**: Browse your logged places in a dashboard.
- **Edit/Delete**: Modify or remove place entries as needed.

## Testing
- Test user registration and login to ensure authentication works.
- Add a place and verify it appears in the dashboard.
- Check MongoDB to confirm data persistence.
- Use tools like Postman to test API endpoints (e.g., `POST /api/places`).

## Troubleshooting
- **MongoDB Connection Issues**: Verify the `MONGO_URI` and ensure MongoDB is running.
- **Dependency Errors**: Run `pip install -r requirements.txt` again or check Python version compatibility.
- **Flask Errors**: Check the console for error messages and ensure all templates are in the `templates/` folder.

## Future Improvements
- Add search and filter functionality for places.
- Implement image uploads for place entries.
- Deploy the application to a cloud platform like Heroku or AWS.
- Add unit tests using `pytest` for backend endpoints.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Flask for providing a lightweight web framework.
- MongoDB for flexible NoSQL database management.
- Bootstrap for responsive frontend design.

For questions or support, open an issue on GitHub.
