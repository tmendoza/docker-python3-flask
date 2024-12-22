# docker-python3-flask
Python Flask Docker starter kit

# Basic Dockerized Flask App

This repository contains a simple Flask application that demonstrates a "Hello, World" response served via a Dockerized web service.

---

## Features

- A basic Flask app with a single route.
- Dockerized setup for easy deployment.
- Configured for development mode.

---

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) installed on your system.
- Python 3.10 or higher (if running without Docker).

---

### Installation

1. **Clone the Repository**:
   ```bash
   git clone <repo_url>
   cd <repo_directory>
   ```

2. **Prepare the Environment**:
   Ensure the `requirements.txt` file includes any necessary Python dependencies (e.g., Flask).

---

### Running with Docker

1. **Build the Docker Image**:
   ```bash
   docker compose build
   ```

2. **Run the Container**:
   ```bash
   docker compose up
   ```

3. **Access the Application**:
   Visit `http://localhost:5000` in your web browser. You should see `Hello, World from Flask!`.

---

### Running Locally

1. **Install Dependencies**:
   Install Python dependencies listed in `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the Flask Application**:
   ```bash
   python app.py
   ```

3. **Access the Application**:
   Open your browser and go to `http://127.0.0.1:5000`.

---

### File Structure

```
.
├── app.py                # Flask application entry point
├── Dockerfile            # Dockerfile to build the container image
├── docker-compose.yml    # Docker Compose configuration
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation (this file)
```

---

### Environment Variables

- `FLASK_ENV`: Specifies the Flask environment (`development` by default in `docker-compose.yml`).

---

### Additional Notes

- Ensure ports `5000:5000` are not in use on your machine before running.
- Modify the `Dockerfile` and `docker-compose.yml` for production settings as needed.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Happy coding! 🚀

