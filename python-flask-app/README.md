# Flask App — AWS ECS Deployment

A minimal Flask web application built for learning containerization and deployment to AWS ECS (Elastic Container Service)
## Project Structure

```
flask-app-ecs/
├── app.py                 # Flask app with routes
├── run.py                 # Entry point (host 0.0.0.0, port 80)
├── requirements.txt       # Python dependencies
├── templates/
│   └── index.html         # Landing page
├── Dockerfile             # Simple single-stage build
└── Dockerfile-multi       # Multistage build with distroless
```

## Dockerfiles Explained

### Simple (`Dockerfile`)

Single-stage build using `python:3.14-slim`. Straightforward — copies everything, installs dependencies, runs the app. Good for development and learning.

### Multistage (`Dockerfile-multi`)

Two-stage build:
1. **Builder stage** — installs dependencies into a separate directory using `python:3.14-slim`
2. **Final stage** — copies only the app and deps into a `distroless` image

