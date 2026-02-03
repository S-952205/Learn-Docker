# Next.js and FastAPI Demo Projects

This repository contains two basic projects:
1.  `next-js`: A basic Next.js application.
2.  `fastapi`: A basic FastAPI application.

## How to run the Next.js application

1.  Navigate into the `next-js` directory:
    ```bash
    cd next-js
    ```
2.  Install the dependencies:
    ```bash
    npm install
    ```
3.  Run the development server:
    ```bash
    npm run dev
    ```
    The Next.js application will be accessible at `http://localhost:3000`.

## How to run the FastAPI application

1.  Navigate into the `fastapi` directory:
    ```bash
    cd fast-app
    ```
2.  (Optional) Create and activate a Python virtual environment:
    ```bash
    python -m venv venv (linux)
    uv venv (windows)
    # On Windows 
    .venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```
3.  Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4.  Run the FastAPI application:
    ```bash
    uvicorn main:app --reload
    ```
    The FastAPI application will be accessible at `http://127.0.0.1:8000`. The API documentation will be available at `http://127.0.0.1:8000/docs`.
