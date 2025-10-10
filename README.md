# Market Place Django Project

یک پروژه Django برای بازار آنلاین که کاربران می‌توانند کالاهای خود را به فروش بگذارند.

## ویژگی‌ها

- ثبت‌نام و ورود کاربران
- ایجاد و مدیریت کالاها
- دسته‌بندی کالاها
- جستجو در کالاها
- داشبورد شخصی
- سیستم پیام‌رسانی
- آپلود تصاویر

## نصب و راه‌اندازی

1. کلون کردن پروژه:
```bash
git clone <repository-url>
cd market
```

2. ایجاد virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # در Windows: venv\Scripts\activate
```

3. نصب dependencies:
```bash
pip install -r requirements.txt
```

4. اجرای migrations:
```bash
python manage.py migrate
```

5. ایجاد superuser:
```bash
python manage.py createsuperuser
```

6. اجرای سرور:
```bash
python manage.py runserver
```

## ساختار پروژه

- `core/`: صفحات اصلی و احراز هویت
- `item/`: مدیریت کالاها
- `dashboard/`: داشبورد کاربری
- `conversation/`: سیستم پیام‌رسانی

## تکنولوژی‌های استفاده شده

- Django 5.2.7
- Pillow (برای پردازش تصاویر)
- SQLite (پایگاه داده پیش‌فرض)
- Tailwind CSS (برای استایل)

## نکات مهم

- فایل‌های تصویر در پوشه `media/item_images/` ذخیره می‌شوند
- در حالت DEBUG، فایل‌های static و media به صورت خودکار سرو می‌شوند
- برای production، باید `DEBUG = False` و `ALLOWED_HOSTS` را تنظیم کنید

