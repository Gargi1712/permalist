# to-do_list


To-do list is a dynamic and user-friendly web application that allows users to create, manage, and organize their tasks efficiently. Built with a modern tech stack, PermaList offers persistent data storage, intuitive UI, and seamless interaction with APIs to enhance task management.

🚀 Features
✅ Add, update, and delete tasks
✅ Organize tasks into multiple lists
✅ Persistent storage with PostgreSQL
✅ Responsive design for various devices
✅ Dynamic UI rendering using EJS
✅ RESTful API integration with CRUD functionality
✅ Error handling and validation

🛠️ Tech Stack
Frontend: HTML, CSS, EJS

Backend: Node.js, Express.js,EJS

Database: PostgreSQL

API: RESTful APIs for task management


⚙️ Installation
1. Install Dependencies
npm install
2. Configure Database
Create a PostgreSQL database named permalist.
Update the database connection in /config/db.js:

import pg from "pg";

const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "permalists",
  password: "sql123",
  port: 5432,
});



3. Run Database Migration
Run SQL queries to create the required tables:
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title VARCHAR(100) NOT NULL
);

INSERT INTO items (title) VALUES ('Buy milk'), ('Finish homework');

4. Start the Application
npm start
5. Open in Browser
Visit http://localhost:3000 to access the application.

📡 API Endpoints
Task Routes
GET / – Render home page

POST /add – Add a new task

POST /edit – Update task status

DELETE /delete – Delete a task

API Routes
GET /api/tasks – Get all tasks

POST /api/tasks – Add a new task

PUT /api/tasks/:id – Update task by ID

DELETE /api/tasks/:id – Delete task by ID

🎨 UI/UX Design
Clean and intuitive interface using HTML & CSS

Responsive design for desktop and mobile users

Dynamic content rendering using EJS templates

🤝 Contributing
Feel free to contribute to enhance the functionality of PermaList!
1.Fork the repository

2.Create a new branch (git checkout -b feature/your-feature).

3.Commit your changes (git commit -m 'Add new feature').

4.Push to the branch (git push origin feature/your-feature).

5.Open a pull request.

📧 Contact
For any inquiries or suggestions, feel free to contact:
[Gargi Jain]
🔗 GitHub: Gargi1712

