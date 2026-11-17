# Greeting page

A small static frontend that asks the greeting API for a personalized hello.

## Prerequisites

- Python 3 (for the built-in static file server)
- The `gate-demo-backend` rig in this project

## Start the backend

In a terminal, from the backend rig directory, run:

```sh
cd /home/ubuntu/proj/work/aae/demos/3-review-gate/gate-demo-backend
python3 server.py
```

The API listens at `http://localhost:8000`. Keep this terminal open.

## Start the frontend

In another terminal, from this rig directory, run:

```sh
cd /home/ubuntu/proj/work/aae/demos/3-review-gate/gate-demo-frontend
python3 -m http.server 3000
```

Open <http://localhost:3000> in your browser.

## Check the full interaction

1. Confirm both server commands are still running.
2. At <http://localhost:3000>, enter a name such as `Ada Lovelace` and select **Say hello**.
3. Confirm the page displays `Hello, Ada Lovelace!`.
4. Submit an empty or whitespace-only name and confirm the browser asks for a name without making an API request.
5. Stop the backend with Ctrl+C, submit a name, and confirm the page explains that it could not get the greeting. Restart the backend when done.
