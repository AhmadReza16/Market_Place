# Market Place Django Project

A Django-based online marketplace where users can register, list items for sale, browse categories, search products, and communicate via messaging.

## Features

- User registration and authentication
- Create, edit, and manage items
- Item categorization
- Search functionality
- Personal dashboard
- Messaging system between users
- Image upload for items

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd market
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Linux/macOS:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations:**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser:**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

----
## 📸 Screenshots

<img width="1349" height="1979" alt="Screenshot 2025-10-10 at 20-03-09 Welcome Market" src="https://github.com/user-attachments/assets/00763ec1-b17d-4237-91fc-717a40d89c2e" />

---


<img width="1349" height="1141" alt="Screenshot 2025-10-10 at 20-03-43 Brown shoes Market" src="https://github.com/user-attachments/assets/2d25c72c-6152-41c3-b228-386918467fd8" />

---

<img width="1349" height="1297" alt="Screenshot 2025-10-10 at 20-12-13 Items Market" src="https://github.com/user-attachments/assets/4e3d7363-68fc-4c26-85f9-e7f1ce49dbb9" />

## Project Structure

- `core/` — Main pages and authentication
- `item/` — Item management
- `dashboard/` — User dashboard
- `conversation/` — Messaging system

## Technologies Used

- Django 5.2.7
- Pillow (image processing)
- SQLite (default database)
- Tailwind CSS (styling)

## Important Notes

- Uploaded images are stored in `media/item_images/`
- In DEBUG mode, static and media files are served automatically
- For production, set `DEBUG = False` and configure `ALLOWED_HOSTS` appropriately

