#
# VENTY - SOCIALS
#

---

## 1. PROJECT OVERVIEW

**Venty** is a full-stack social media web application built with Laravel as part of my independent development projects.  
It demonstrates the creation of a modern, scalable platform where users can connect, share posts, interact through comments and likes, and maintain personal profiles.

The project focuses on **clean architecture**, **database design**, and **real-world social features**, showcasing my understanding of full-stack Laravel development.

---

## 2. CORE FEATURES

* User authentication and profile management  
* Create, edit, and delete posts  
* Commenting and liking system  
* User-to-user relationships (follow / unfollow)  
* Category-based post grouping  
* Real-time UI updates with AJAX and Laravel Mix  
* Responsive and accessible design (Bootstrap 5)  
* Admin-level moderation tools  
* Data persistence using Eloquent ORM  
* Database migrations and seeding for setup  

---

## 3. PROJECT STRUCTURE

```
app/Models/          → Contains all Eloquent models (User, Post, Comment, Like, Profile, Category)
database/migrations/ → All migration files for tables and relationships
resources/views/     → Blade templates for all pages and layouts
routes/web.php       → Application routes for web interfaces
public/              → Public assets (CSS, JS, Images)
config/              → Configuration files (database, app, mail, etc.)
tests/               → Unit and feature tests
composer.json        → PHP dependencies
artisan              → Laravel CLI tool
```

---

## 4. SETUP & INSTALLATION

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Aliy7/laravel-cs368.git
   cd venty-socials
   ```

2. **Install dependencies:**
   ```bash
   composer install
   npm install && npm run dev
   ```

3. **Configure the environment:**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```
   Update `.env` with your MySQL credentials.

4. **Run migrations and seeders:**
   ```bash
   php artisan migrate --seed
   ```

5. **Start the development server:**
   ```bash
   php artisan serve
   ```

   Access the app via [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 5. DATABASE DESIGN

**Entities include:**  
* `users` – Stores user profiles and credentials  
* `posts` – Stores text and image posts  
* `comments` – User comments on posts  
* `likes` – Likes associated with posts  
* `profiles` – One-to-one relationship with users  
* `categories` – Organizes posts by type  

Relationships follow Laravel conventions using **Eloquent ORM**.

---

## 6. PROJECT PURPOSE

Venty was created to demonstrate the **core functionality of a modern social platform**, focusing on Laravel’s strength in:  
* MVC structure  
* Database relationships  
* Blade templating and component reuse  
* Validation, middleware, and routing control  

It served as both a **learning milestone** and a **portfolio project**, highlighting backend logic, UI design, and full CRUD integration.

---

## 7. FUTURE IMPROVEMENTS

* Implement messaging and notifications system  
* Add real-time post updates with Laravel Echo  
* Integrate profile picture uploads via Cloudinary  
* Create API endpoints for mobile integration  

---

## 8. CONCLUSION

**Venty** represents a complete social media system prototype built with Laravel, emphasizing scalability, maintainability, and clean coding practices.  
It demonstrates my understanding of **Laravel frameworks**, **database modeling**, and **end-to-end application development** suitable for real-world environments.

**----End----**
