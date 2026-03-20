---

# File Upload System

A simple Flask-based File Upload System that allows users to upload, validate, and preview files such as images, PDFs, and text documents through a clean web interface.

---

## Features

* Upload files (images, PDF, text)
* File type validation for security
* Image preview support
* View uploaded files
* Clean and simple user interface
* Deployable on Render

---

## Tech Stack

* Backend: Flask (Python)
* Frontend: HTML, CSS
* Server: Gunicorn

---

## Project Structure

```
file-upload-app/
│
├── app.py
├── requirements.txt
├── uploads/
├── templates/
│   └── index.html
├── static/
│   └── style.css
```

---

## Installation & Setup

### 1. Clone Repository

```bash
git clone YOUR_REPO_LINK
cd file-upload-app
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the App

```bash
python app.py
```

Open in browser:

```
http://127.0.0.1:5000
```

---

## Deployment (Render)

1. Push project to GitHub
2. Go to Render
3. Create a New Web Service
4. Use the following settings:

```
Build Command: pip install -r requirements.txt
Start Command: gunicorn app:app
```

---

## Important Note

Render uses temporary storage. Use `/tmp/uploads` for file storage in production.

---

## Future Improvements

* Multiple file upload
* Drag and drop interface
* Upload progress bar
* Cloud storage integration (AWS S3, Firebase)
* User authentication

---
