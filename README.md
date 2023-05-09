# ProMan
ProMan is a simple web-based project management tool, something similar to Trello, built using Flask and PostgreSQL. It allows you to organize your projects and tasks using a drag-and-drop interface, and keep track of their status as they move through different stages of completion.
# Features
- Create new projects and add tasks to them.
- Organize tasks into different columns (To Do, In Progress, Done).
- Move tasks between columns by dragging and dropping them.
- Edit and delete tasks as needed.
- User authentication and authorization.

# Technologies Used
- Python 3.9.5
- Flask 2.0.0
- Postgres
- Jinja2 3.0.1
- HTML 5
- CSS 3
- JavaScript

# Installation
To get started with ProMan, follow these steps:

1. Clone the repository to your local machine:

- git clone https://github.com/MadalinaRadulescu/ProMan.git
- cd ProMan

2. Create a virtual environment and activate it:

- python3 -m venv venv
- source venv/bin/activate

3. Install the required dependencies:

- pip install -r requirements.txt

4. Create a PostgreSQL database and configure its URL in the .env file:

- createdb proman
- cp .env.example .env

Edit the .env file and set the DATABASE_URL variable to your PostgreSQL URL.

5. Create the database tables:

- flask db upgrade

6. Run the application:

- flask run
You should see a message saying that the application is running at http://localhost:5000.

7. Open the URL in your web browser and start using ProMan!
# Usage
When you first open ProMan, you will see a list of all your projects. You can create a new project by clicking the "New Board" button and entering a name for it.

Once you have created a project, you can add tasks to it by clicking the "Add Task" button and filling in the details. Each task has a title, a description, and a due date. You can also assign the task to a specific user.

Tasks are organized into columns based on their status: To Do, In Progress, and Done. You can move a task between columns by dragging and dropping it. You can also edit or delete a task by clicking on it.
When you are logged in you can create private boards that only you can see.

# Screenshots
**HomePage**

<img width="1204" alt="Screenshot 2023-05-09 at 09 44 38" src="https://user-images.githubusercontent.com/101947079/237020751-d3698e73-f198-43c2-8cb9-fabc7920a3c2.png">

**Board Tasks**

<img width="1145" alt="Screenshot 2023-05-09 at 09 44 59" src="https://user-images.githubusercontent.com/101947079/237021018-8ff60bc9-e03a-4cb1-83ed-139902615394.png">

**User's Boards**

<img width="1245" alt="Screenshot 2023-05-09 at 09 47 05" src="https://user-images.githubusercontent.com/101947079/237021162-98838878-0692-4f54-904d-dee53ece57c1.png">

**Creating a new board/task**
<img width="911" alt="Screenshot 2023-05-09 at 09 45 20" src="https://user-images.githubusercontent.com/101947079/237021246-913ff2ba-ee03-4ddc-a882-7a714f1b3839.png">

<img width="762" alt="Screenshot 2023-05-09 at 09 45 43" src="https://user-images.githubusercontent.com/101947079/237021283-0b150662-aa3f-4933-9c08-4cfa3beeb547.png">

# License
ProMan is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

