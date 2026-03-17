# 📝 Laboratory Activity 5: Full CRUD Blog Application

## 🎯 Project Objectives
* Implement a complete **CRUD** system (Create, Read, Update, Delete).
* Use **Laravel Resource Controllers** to handle data logic.
* Work with **Eloquent Models** and Database Migrations.
* Create dynamic UI using **Blade Templates** and Route helpers.

---

## 🗺️ CRUD File Location Map
This map shows the specific files created for the Blog functionality:

```text
lastname_blogapp/
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── PostController.php    <-- [Logic] Handles CRUD actions (index, store, etc.)
│   └── Models/
│       └── Post.php                  <-- [Model] Represents the 'posts' table (Mass Assignment)
├── database/
│   └── migrations/
│       └── xxxx_create_posts_table.php <-- [Database] Schema for 'title' and 'body'
├── resources/
│   └── views/
│       └── posts/                    <-- [Folder] All Blog-related views
│           ├── index.blade.php       <-- [Read] Lists all posts
│           ├── create.blade.php      <-- [Create] Form for new posts
│           ├── edit.blade.php        <-- [Update] Form for editing existing posts
│           └── show.blade.php        <-- [Read] Displays a single full post
└── routes/
    └── web.php                       <-- [Routes] Uses Route::resource for 'posts'