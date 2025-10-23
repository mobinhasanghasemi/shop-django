

````markdown
# 🛍️ Django Shop Project — Beginner Friendly

یک پروژه فروشگاه اینترنتی ساده و آموزشی ساخته‌شده با **Django**  
هدف این پروژه آموزش مفاهیم پایه‌ی جنگو به افراد مبتدیه، در قالب یک مثال واقعی و کاربردی.

---

## ✨ ویژگی‌ها (Features)

- 🧩 **افزودن به سبد خرید (Add to Cart)** بدون رفرش صفحه با **AJAX**
- 💬 **فرم تماس با ما (Contact Us)** به‌صورت **کاملاً داینامیک و بدون reload**
- 📦 **مدیریت محصولات، دسته‌بندی و اسلایدرها** از طریق پنل ادمین
- 📊 **دانلود گزارش Excel از موجودی محصولات** با استایل پیشرفته
- ⚠️ هشدار خودکار **موجودی کم**
- 👥 **مدیریت کاربران و پروفایل‌ها**
- 🧾 **مدیریت سفارش‌ها و آیتم‌های سفارش (Order & OrderItem)**
- 🖼️ نمایش تصویر بندانگشتی محصول در پنل ادمین
- 🌙 رابط کاربری ساده، تمیز و مناسب برای تمرین و آموزش جنگو

---

## 🧰 پیش‌نیازها (Requirements)

پیش از اجرا مطمئن شوید که **Python 3.10+** و **pip** روی سیستم شما نصب شده باشد.

سپس پکیج‌های زیر را نصب کنید 👇

```bash
pip install django==4.2.10
pip install pillow
pip install openpyxl
pip install phonenumbers
pip install django-phonenumber-field
````

---

## ⚙️ راه‌اندازی پروژه (Setup)

1. کلون کردن پروژه:

```bash
git clone https://github.com/mobinhasanghasemi/shop-django.git
cd shop-django
```

2. ساخت و فعال‌سازی محیط مجازی:

```bash
python -m venv venv
venv\Scripts\activate  # در ویندوز
# یا
source venv/bin/activate  # در لینوکس / مک
```

3. نصب وابستگی‌ها:

```bash
pip install -r requirements.txt
```

*(اگر فایل requirements.txt وجود نداشت، از بخش بالا پکیج‌ها را نصب کنید.)*

4. انجام مهاجرت‌ها (migrations):

```bash
python manage.py makemigrations
python manage.py migrate
```

5. ساخت ادمین:

```bash
python manage.py createsuperuser
```

6. اجرای سرور:

```bash
python manage.py runserver
```

---

## 🧠 آموزش AJAX (بدون رفرش)

در این پروژه دو بخش کلیدی با AJAX ساخته شده‌اند:

* افزودن محصول به سبد خرید (`add_to_cart`)
* فرم تماس با ما (`contact`)

هر دو بدون نیاز به رفرش صفحه کار می‌کنند و از **CSRF Token** به‌صورت ایمن استفاده می‌کنند:

```javascript
headers: { "X-CSRFToken": csrftoken },
```

---

## 🖼️ بخش ادمین (Admin Panel)

پنل ادمین شامل قابلیت‌های زیر است:

* مشاهده تصویر محصول (thumbnail)
* نمایش هشدار موجودی کم با رنگ قرمز
* دانلود گزارش اکسل از محصولات
* فیلتر و جستجوی پیشرفته
* نمایش محصولات مشابه در همان دسته‌بندی

---

## 📦 ساختار کلی پروژه

```
shop-django/
│
├── mainpagestore/
│   ├── admin.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── templates/
│   └── static/
│
├── store/
│   ├── settings.py
│   └── urls.py
│
└── manage.py
```

---

## 📞 تماس

ساخته‌شده با عشق ❤️ برای آموزش و تمرین برنامه‌نویسان تازه‌کار
Developed by [Mobin hasanghasemi](https://github.com/mobinhasanghasemi)

---

## 🪶 لایسنس

این پروژه صرفاً برای **یادگیری و تمرین Django** ساخته شده و استفاده آموزشی از آن کاملاً آزاد است.

```

---)
```
