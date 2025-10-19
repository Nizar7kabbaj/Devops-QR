# DevOps QR Code

This project is part of my **DevOps Capstone**. It’s a simple web app that generates QR codes for any URL you provide.  
The front-end is built with **Next.js**, and the back-end API is developed with **Python (FastAPI)**.

---

## 🧩 Application Overview

**Front-End:**  
A Next.js web interface where users can enter URLs and get their QR codes.

**API:**  
A FastAPI service that receives URLs, generates QR codes, and uploads them to **AWS S3** for storage.

---

## ⚙️ Running Locally

### API Setup

1. Clone this repository.  
2. Go to the `api` directory.  
3. Create a virtual environment:  
   ```bash
   python -m venv .venv
4. Activate it and install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
5. Create a `.env` file with your AWS credentials (check `.env.example` for reference).
6. Update the `BUCKET_NAME` in `main.py` to match your own S3 bucket.
7. Start the API server:

   ```bash
   uvicorn main:app --reload
   ```

   The API should be running at [http://localhost:8000](http://localhost:8000)

---

### Front-End Setup

1. In a new terminal, go to the `front-end-nextjs` directory.
2. Install the dependencies:

   ```bash
   npm install
   ```
3. Run the development server:

   ```bash
   npm run dev
   ```

   The front-end will be live at [http://localhost:3000](http://localhost:3000)

---

## 🎯 Goal

The goal of this project is to practice key **DevOps** concepts like containerization, CI/CD, and monitoring while building a functional, cloud-connected application.
