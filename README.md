

# Accommodation Search System

A modern and reliable accommodation search platform designed specifically to help students easily find and manage affordable boarding houses, apartments, and other lodging options near their schools. By integrating backend and frontend technologies seamlessly, the system provides a smooth, efficient, and user-friendly experience tailored to the unique needs of students looking for convenient and budget-friendly places to stay.


---

## 🌟 Feature

### 🔍 Advanced Search  
- Find accommodations by location, price range, amenities, and type

### 👤 User Management  
- User registration and login with secure token authentication  
- Manage personal profiles and update passwords

### 🏡 Accommodation Management  
- Add, edit, and delete accommodation listings  
- Upload and manage images and amenities  
- Track availability status of listings  
- View accommodation locations integrated with Google Maps

---

## 🛠 Tech Stack

***Backend***
- Python
- Django
- MySQL
- Cloudinary
- OAuth2.0

***Frontend***
- React Native  
- Firebase  
- React Native Dotenv  
- React Native Elements  
- Lodash  

***Other***
- pip, Django ORM, Git

---

## ⚙ Installation 

### 1️⃣ Backend

```bash
git clone https://github.com/thien0709/AccommodationSearch.git
cd Accommodation-search-system-BE
```
***Config environment***
```bash
python -m venv venv
```
```bash
source venv/bin/activate   # Linux/Mac
```
```bash
venv\Scripts\activate      # Windows
```
```bash 
pip install -r requirements.txt
```
***Create a MySQL database named `accommodation_db`***

```bash
python manage.py migrate
python manage.py runserver
```
--- 

### 2️⃣ Frontend

```bash
git clone https://github.com/thien0709/AccommodationSearch.git
cd Accommodation_Search_System_FE
```
```bash
npm install
npm start
```

---

## 📂 Structure

**Backend**
```
Directory structure:
└── hoduclinh-accommodation-search-system-be/
    ├── README.md
    └── accommodation_system/
        ├── manage.py
        ├── requirements.txt
        ├── accommodation_app/
        │   ├── __init__.py
        │   ├── admin.py
        │   ├── apps.py
        │   ├── models.py
        │   ├── serializers.py
        │   ├── tests.py
        │   ├── urls.py
        │   ├── utils.py
        │   ├── views.py
        │   ├── migrations/
        │   │   ├── 0001_initial.py
        │   │   ├── 0002_alter_user_password.py
        │   │   ├── 0003_alter_user_password.py
        │   │   ├── 0004_post_is_approved.py
        │   │   ├── 0005_alter_commentpost_post_alter_commentpost_user.py
        │   │   └── __init__.py
        │   └── templates/
        │       ├── index.html
        │       └── admin/
        │           └── accommodation_stats.html
        └── accommodation_system/
            ├── __init__.py
            ├── asgi.py
            ├── settings.py
            ├── urls.py
            └── wsgi.py
```
**Frontend**
```
Directory structure:
└── thien0709-accommodation_search_system_fe/
    ├── README.md
    ├── LICENSE
    └── Accommodation_Search_System/
        ├── App.js
        ├── app.json
        ├── babel.config.js
        ├── index.js
        ├── package.json
        ├── components/
        │   ├── Explore/
        │   │   ├── Accommodation.js
        │   │   └── PagerViewComponent.js
        │   └── Home/
        │       ├── HomeStyles.js
        │       ├── Post.js
        │       ├── Search.js
        │       └── ToggleTheme.js
        ├── configs/
        │   ├── APIs.js
        │   ├── Firebase.js
        │   ├── MyUserContext.js
        │   └── MyUserReducers.js
        ├── navigation/
        │   ├── Stack.js
        │   └── Tab.js
        ├── screens/
        │   ├── AccommodationDetail.js
        │   ├── ChatDetailScreen.js
        │   ├── ChatScreen.js
        │   ├── CheckoutScreen.js
        │   ├── CommentScreen.js
        │   ├── CreateAccommodation.js
        │   ├── CreatePost.js
        │   ├── ExploreScreen.js
        │   ├── HomeScreen.js
        │   ├── LoginScreen.js
        │   ├── MyPostScreen.js
        │   ├── PersonalDetailsScreen.js
        │   ├── ProfileScreen.js
        │   ├── RegisterScreen.js
        │   └── WelcomeScreen.js
        └── styles/
            └── MyStyles.js
```