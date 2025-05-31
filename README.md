# Agent API 🚀

![Agent API](https://img.shields.io/badge/Agent%20API-v1.0.0-blue.svg)  
[![Releases](https://img.shields.io/badge/Releases-v1.0.0-orange.svg)](https://github.com/HackerGCLASS/agent-api/releases)

Welcome to the **Agent API** repository! This project offers a minimal and open-source setup for serving agents using **FastAPI** and **Postgres**. Designed for speed, clarity, and developer happiness, it provides a robust foundation for building agent-based applications.

## Table of Contents

1. [Features](#features)
2. [Getting Started](#getting-started)
3. [Installation](#installation)
4. [Usage](#usage)
5. [API Documentation](#api-documentation)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Features 🌟

- **FastAPI**: Leverage the power of FastAPI for building APIs quickly and efficiently.
- **Postgres**: Utilize PostgreSQL for a reliable and scalable database solution.
- **Minimal Setup**: Get started with a straightforward configuration.
- **Developer Friendly**: Focus on developer happiness with clear documentation and a clean codebase.

## Getting Started 🏁

To get started with the Agent API, follow these steps to set up your environment.

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7 or higher
- PostgreSQL
- pip (Python package installer)

### Installation 🛠️

1. **Clone the repository**:

   ```bash
   git clone https://github.com/HackerGCLASS/agent-api.git
   cd agent-api
   ```

2. **Install the required packages**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the database**:

   Create a new PostgreSQL database and update the `DATABASE_URL` in the `.env` file with your database credentials.

4. **Run the migrations**:

   Use the following command to set up the database schema:

   ```bash
   alembic upgrade head
   ```

5. **Start the server**:

   Run the FastAPI application with the command below:

   ```bash
   uvicorn main:app --reload
   ```

## Usage 💻

Once your server is running, you can access the API at `http://127.0.0.1:8000`. Use tools like **Postman** or **curl** to interact with the endpoints.

### Example Request

To create a new agent, send a POST request to `/agents` with the following JSON body:

```json
{
  "name": "Agent Smith",
  "type": "AI",
  "status": "active"
}
```

### Example Response

You will receive a response like this:

```json
{
  "id": 1,
  "name": "Agent Smith",
  "type": "AI",
  "status": "active"
}
```

## API Documentation 📖

For detailed API documentation, visit the interactive API docs provided by FastAPI at `http://127.0.0.1:8000/docs`.

## Releases 📦

For the latest releases, visit our [Releases section](https://github.com/HackerGCLASS/agent-api/releases). You can download the latest version and execute it to start using the Agent API.

## Contributing 🤝

We welcome contributions to the Agent API! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your fork and submit a pull request.

Please ensure your code follows the existing style and includes appropriate tests.

## License 📜

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact 📬

For questions or feedback, feel free to reach out to the maintainers of this project. You can also join our community discussions on GitHub.

---

Thank you for checking out the Agent API! We hope you find it useful for your projects. Don't forget to check our [Releases section](https://github.com/HackerGCLASS/agent-api/releases) for updates and new features. Happy coding!