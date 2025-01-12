A basic Quora-like project implementing CRUD functionality using RESTful APIs. Users can create, read, update, and delete posts, providing a foundation for learning API development with Node.js and Express.

Features
	•	Display all posts on the main page.
	•	Add a new post with a username and content.
	•	View a specific post with its details.
	•	Edit the content of a post.
	•	Delete a post.
	•	Middleware for form data parsing and method overriding.
	•	Server-side rendering using EJS templates.

 Technologies Used
	•	Node.js: Backend runtime environment.
	•	Express: Web framework for handling routes and middleware.
	•	EJS: Template engine for server-side rendering.
	•	UUID: For generating unique IDs for posts.
	•	Method-Override: Enables HTTP methods like PATCH and DELETE.

 Installation
	1.	Clone the repository: git clone https://github.com/mahelika/REST-API-Quora.git
 	2.	Navigate to the project directory: cd REST-API-Quora
  3.	Install dependencies: npm install
  4.	Start the server: node index.js
  5.	The server will run on http://localhost:8080.

Folder Structure
 REST-API-Quora/
├── index.js         # Main server file
├── views/           # EJS templates for rendering pages
│   ├── index.ejs    # Displays all posts
│   ├── new.ejs      # Form to create a new post
│   ├── show.ejs     # Displays details of a specific post
│   └── edit.ejs     # Form to edit an existing post
├── public/          # Static assets (CSS, JS, images)
├── node_modules/    # Installed dependencies
├── package.json     # Project metadata and dependencies
├── package-lock.json# Dependency lockfile
└── .gitignore       # Ignored files and folders

Middleware Used
	1.	express.urlencoded: Parses application/x-www-form-urlencoded data for handling form submissions.
	2.	method-override: Enables HTTP verbs like PATCH and DELETE using _method query parameters.
	3.	express.static: Serves static files from the public directory.


How to Interact

Add a New Post
	1.	Visit http://localhost:8080/posts/new.
	2.	Fill out the form with your username and content, and click submit.
	3.	The new post will appear on the main page.

Edit a Post
	1.	Go to http://localhost:8080/posts.
	2.	Click the Edit button next to the post you want to modify.
	3.	Update the content in the form and submit.

Delete a Post
	1.	Go to http://localhost:8080/posts.
	2.	Click the Delete button next to the post you want to remove.
