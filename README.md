
---

# Humans Origins Website Setup Guide

This guide provides instructions on installing and configuring the **Humans Origins** website along with the backend API, allowing users to manage the server and view real-time data.

## Table of Contents

- [About](#about)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Starting the Project](#starting-the-project)
- [Contributing](#contributing)
- [License](#license)

## About

The **Humans Origins** website is designed to provide a user-friendly interface for interacting with the Minecraft server. It includes a backend API that fetches real-time data from the server, displays stats, and lets users manage certain aspects of the server.

---

## Prerequisites

Ensure you have the following installed:

- **Node.js** (>=14)
- **npm** or **yarn** (for package management)
- **MongoDB** or other supported database for storing data (optional, if needed by backend)
- **Git** (for cloning the repository)

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/DankiCalamari/humansorigins.git
cd humansorigins
```

### 2. Install Dependencies

#### Backend Dependencies

Navigate to the backend folder and install dependencies:

```bash
cd backend
npm install
```

#### Frontend Dependencies

Go back to the root directory, navigate to the frontend folder, and install dependencies:

```bash
cd ../frontend
npm install
```

---

## Configuration

1. **Backend Configuration**: In the `backend` folder, create a `.env` file to store environment variables.

   Example `.env`:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_uri
   DISCORD_BOT_TOKEN=your_discord_bot_token
   DISCORD_CHANNEL_ID=your_discord_channel_id
   ```

2. **Frontend Configuration**: In the `frontend` folder, create a `.env` file to store frontend-specific environment variables (e.g., API endpoints).

   Example `.env`:

   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

---

## Starting the Project

### 1. Start the Backend Server

From the `backend` folder, run:

```bash
npm start
```

The backend server should now be running on `http://localhost:5000`.

### 2. Start the Frontend Server

From the `frontend` folder, run:

```bash
npm start
```

The frontend server should now be running on `http://localhost:3000`.

---

## Accessing the Website

Once both the backend and frontend servers are running, visit `http://localhost:3000` in your browser to access the Humans Origins website.

---

## Contributing

If you’d like to contribute, please fork the repository, create a new branch, and make your changes. Then submit a pull request for review.

---

## License

This project is licensed under the MIT License.

--- 

This guide provides a full setup to run both the website and backend for **Humans Origins**. Let me know if you'd like additional sections, such as troubleshooting or deployment tips!