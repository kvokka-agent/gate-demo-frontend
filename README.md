# Greeting frontend

A small browser frontend that sends a name to the greeting backend and displays its response.

## Prerequisites

- Python 3
- The greeting backend running at `http://127.0.0.1:8001`

## Start the frontend

From this directory, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000> in your browser. Keep the backend running on port 8001; the backend must allow browser requests from `http://127.0.0.1:8000`.

## Check the complete flow

1. Start the backend on port 8001.
2. Start the frontend with the command above.
3. Open <http://127.0.0.1:8000>, enter `Ada` in the name field, and select **Get greeting**.
4. Confirm the page displays `Hello, Ada!`, as returned by the backend.
5. To check the error state, stop the backend and submit a name again. The page displays an error explaining that the greeting could not be retrieved.
