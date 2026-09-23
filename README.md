# Web Application

A simple and lightweight web application built using HTML, designed to provide users with different pages for workout planning, food scheduling, user registration, and password recovery.

## Features

* 🏠 Home page
* 📝 User sign-up page
* 🔐 Forgot password page
* 🍎 Food schedule page
* 🏋️ Workout page
* 📱 Simple and easy-to-use web interface
* 💻 Runs directly in a web browser

## Technologies Used

* HTML5
* CSS3
* JavaScript

## Project Structure

```text
Web/
├── index.html
├── Food_Schedule.html
├── Forget_Password.html
├── Sign_up.html
└── workout_page.html
```

## Run Locally

### Using Python

Clone the repository:

```bash
git clone https://github.com/saravana022/Web.git
```

Navigate to the project:

```bash
cd Web
```

Start a local web server:

```bash
python3 -m http.server 8082
```

Open the application in your browser:

```text
http://localhost:8082
```

Since `index.html` is present, it will be displayed as the main page.

## Run with Docker

You can also run the application using Docker and NGINX.

Create a `Dockerfile`:

```dockerfile
FROM nginx:alpine

COPY . /usr/share/nginx/html

EXPOSE 80
```

Build the Docker image:

```bash
docker build -t web-app .
```

Run the container:

```bash
docker run -d --name web-app -p 8082:80 web-app
```

Then open:

```text
http://localhost:8082
```

## Docker Commands

Check the running container:

```bash
docker ps
```

View container logs:

```bash
docker logs web-app
```

Stop the container:

```bash
docker stop web-app
```

Remove the container:

```bash
docker rm web-app
```

## Purpose

This project is a simple web application created for learning and practicing frontend web development, local hosting, Git/GitHub, and Docker containerization.

## Author

**Saravana Kumar R**

GitHub: [@saravana022](https://github.com/saravana022)
