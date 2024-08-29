# 🚀 Flask Application with Playwright Integration

## 📝 Overview

This project is a Flask-based web application designed to automate interactions with Quora, such as fetching questions and posting answers. The application uses Playwright, a powerful browser automation tool, to perform actions on Quora's web interface. The integration with AgentQL allows for querying specific elements on the page, making the process of locating and interacting with elements more efficient.

## ✨ Features

- **Fetch Questions**: This API endpoint allows you to fetch a list of questions from a specified Quora page.
- **Post Answers**: This API endpoint enables automated posting of answers to specific Quora questions.
- **State Management**: The application can save and load a signed-in browser state to maintain session continuity.
- **Playwright Integration**: Utilizes Playwright for browser automation tasks, such as navigating pages, filling forms, and clicking buttons.
- **AgentQL Queries**: Uses AgentQL to efficiently locate and interact with specific page elements.

## 🛠 Prerequisites

- **Python 3.7+**
- **Docker**
- **Playwright**
- **Flask**
- **AgentQL**

## 🔧 Environment Variables

The application requires several environment variables to function correctly. These can be set in a `.env` file:

- `EMAIL`: The email address used to log in to Quora.
- `PASSWORD`: The password associated with the Quora account.
- `PORT`: The port on which the Flask server will run (default is `5000`).
- `RENDER`: Set this to enable the production mode, which uses a different path for the Quora session state.

Example `.env` file:

```env
EMAIL=your-email@example.com
PASSWORD=your-password
PORT=5000
RENDER=1  # Set this only if deploying on Render or a similar platform
