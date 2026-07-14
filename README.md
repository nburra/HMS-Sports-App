# HMS Sports Project Repository

## Description

An all-in-one database for a high school sports team that allows streamlined activity for its users. Because our app is focused on our specific user stories and personas, some aspects of the code are "hard-coded" to display only results that pertain to them.

## Features

This repo contains features for four archetypical users: Coach, Athlete, Recruiter, and Athletic Director. We use Role-Based Access Control to specify certain abilities and access. Here are the tools created for their use:

* **Coach Features:** Schedule viewing (games and practices), strategy viewing (all strategies registered with the team).
* **Recruiter Features:** Search for players that meet their recruitment requirements (has access to academic and athletic stats).
* **Athlete Features:** Stats management (can view or update), can view schedules (games, practices, and recruitment events), recruitment profile (includes highlight reels and scholarship guidance).
* **Athletic Director Tools:** View all teams they manage (with roster and coach info), practice management (can view all practices and their info, and can add or delete practices).
* **App Features:** Clear buttons on how to access tools, navigation sidebar that lets the user log out and go back to the previous page.

## Built With

* werkzeug
* flask
* flask-login
* flask-mysql
* cryptography
* python-dotenv
* pandas
* streamlit
* requests
* validators

## Prerequisites

* A GitHub account.
* A terminal-based Git client or GUI Git client such as GitHub Desktop or the Git plugin for VS Code.
* VS Code with the Python extension.
* A distribution of Python running on your laptop. The distribution supported by the course is Anaconda or Miniconda.

## Installation

Clone your forked version of this repository:

1. Clone the project:

   * In GitHub: **Code > SSH > Copy**
   * In the terminal:

     * `git clone <paste URL>`

2. Set up the `.env` file in the `api` folder using `.env.template`.

   * Enter a new passcode.

3. Install dependencies from the `requirements.txt` files:

   * For the API folder:

     * `pip install -r ./api/requirements.txt`
   * For the app folder:

     * `pip install -r ./app/requirements.txt`

4. Use Docker to start the services:

   * `docker compose up -d`

5. To stop and restart containers when updating the backend:

   * `docker compose down`
   * `docker compose up -d`

6. Create a new data source in DataGrip and connect to the database (used for testing queries and updating the database):

   * Create a new project.
   * Name it **project repo**.
   * Change the port to **3200**.
   * Username: **root**.
   * Enter the password from the `.env` file.
   * Test the connection.

## Usage

This athletics management platform offers intuitive tools for team and individual management. Users can:

* Log in to access role-specific dashboards (e.g., coach tools, recruiter search).
* Create player profiles with academic and athletic achievements.
* Access highlights for top athletes.
* Manage schedules, track stats, and connect directly with colleges and recruiters.

## Further Steps

In the future, we would like to implement more tools for our users that would further streamline activity. For example, we would add contact information for all users that would allow easy access and communication. Additionally, we could have a messaging tool that allows users to directly send and receive messages between users.
