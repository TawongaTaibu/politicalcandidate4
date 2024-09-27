# Project Name

## Description

Provide a brief description of your project here.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Setup](#setup)
4. [Running the Application](#running-the-application)
5. [Docker Instructions](#docker-instructions)
6. [Usage](#usage)
7. [Credits](#credits)

## Prerequisites

Ensure you have the following installed:

- Python 3.x
- Docker
- Git

## Installation

### Using venv

1. **Clone the repository:**

    ```bash
    git clone https://github.com/TawongaTaibu/politicalcandidate4.git
    cd politicalcandidate4
    ```

2. **Create a virtual environment:**

    ```bash
    python -m venv TTenv
    ```

3. **Activate the virtual environment:**

    - On Windows:
      ```bash
      TTenv\Scripts\activate
      ```

    - On macOS/Linux:
      ```bash
      source TTenv/bin/activate
      ```

4. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

## Setup

1. **Apply database migrations (if applicable):**

    ```bash
    python manage.py migrate
    ```

## Running the Application

### Using venv

1. **Start the application:**

    ```bash
    python manage.py runserver
    ```

   Run the "python manage.py runserver" command to start your application. 
   
3. **Access the application in your browser:**

    After running the command, you'll be redirected by clicking the `http://localhost:8000` or the appropriate URL specified in your application.

5.
### Using Docker

1. **Build the Docker image:**

    ```bash
    docker build -t dfa .
    
    ```

    Using docker, we can create an image in this case called "dfa" which is our django app name

2. **Run the Docker container:**

    ```bash
    docker run -p 8000:8000 dfa
    ```

   By running this command you ensure that the docker container 'dfa' is ready to go.

3. **Access the application in your browser:**

    Visit `http://localhost:8000` or the appropriate URL specified in your Docker configuration.


## Usage
Firstly, you have to open the projects folder on your IDE and click *RUN* or by clicking 
an inverted triangle pointing to the left which is on the top right corner
if you're using *Visual Studio Code*. This allows you to go to the root directory of the project
and this is where you run the *python manage.py runserver* command. After a successful launch, a user is welcomed
by the *Home Page* of the political candidate and from here they are able to navigate to other pages of this webpage.
For example, if a user is willing to view the news of the political party he/she should be a registered and logged in user.

## Credits

https://www.techtarget.com/searchsoftwarequality/definition/documentation#:~:text=Software%20documentation%20provides%20information%20about,such%20as%20installation%20and%20troubleshooting.
https://www.tutorialspoint.com/docker/index.html

---
