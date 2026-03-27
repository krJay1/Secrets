# Secrets

## 🚀 Getting Started
Follow these instructions to get the project up and running on your local machine.

### Prerequisites
* Python 3.12 or 3.13 (Recommended for stability with Pillow)
* Git (For version control)

## 🛠️ Installation & Setup

### Clone the Repository
```bash
git clone <your-repository-url>
cd Secrets
```

### Create a Virtual Environment
Using Python 3.13 to avoid build errors:
```bash
py -3.13 -m venv .venv
```

### Activate the Environment
Git Bash / MINGW64:
```bash
source .venv/Scripts/activate
```

PowerShell:
```powershell
.\.venv\Scripts\Activate.ps1
```

### Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Environment Variables
Create a `.env` file in the root directory and add your secret keys (this project uses `python-dotenv`):
```env
DEBUG=True
SECRET_KEY=your-django-secret-key-here
DATABASE_URL=sqlite:///db.sqlite3
```

## 🏃 Running the Application

### Apply Migrations
```bash
python manage.py migrate
```

### Start the Development Server
```bash
python manage.py runserver
```
Your app will be live at http://127.0.0.1:8000/.

## 📦 Dependencies
| Package | Version | Purpose |
| :--- | :--- | :--- |
| Django | 5.1.7 | Web Framework |
| Pillow | 11.1.0 | Image Processing |
| python-dotenv | 1.0.1 | Environment Variable Management |
| asgiref | 3.8.1 | ASGI Server Support |
| sqlparse | 0.5.3 | SQL Formatting/Parsing |