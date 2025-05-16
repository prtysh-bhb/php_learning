# ✅ Laravel Week Learning Plan

> 🗓️ Goal: Build strong foundation in Auth, Eloquent, Middleware, and Request Handling.  
> 🕰️ Target Time: 20–30 hours

---

## 🔐 1. Laravel Authentication (Breeze/UI)
- [ ] Install Laravel Breeze or UI in a new project  
- [ ] Understand auth routes: `login`, `register`, `logout`, etc.  
- [ ] Trace login flow: Route → Controller → Middleware → Redirect  
- [ ] Customize registration form (e.g., add `username`)  
- [ ] Show user's name on dashboard after login  

**⏱ Est. Time**: 3–4 hrs

---

## 🛡️ 2. Middleware & Role-Based Routing
- [ ] Protect `/dashboard` with `auth` middleware  
- [ ] Add `role` column to `users` table  
- [ ] Create two user types: `admin`, `user`  
- [ ] Use middleware or Spatie Permissions for role access  
- [ ] Redirect users to role-specific dashboards  

**⏱ Est. Time**: 3 hrs

---

## 📑 3. Form Requests & Validation
- [ ] Create Form Request classes for forms (e.g. Post CRUD)  
- [ ] Use built-in Laravel validation rules  
- [ ] Create and apply a **custom validation rule**  
  - e.g. Restrict specific words in post title  

**⏱ Est. Time**: 2–3 hrs

---

## 🔁 4. Eloquent Deep Dive
- [ ] Create models: `User`, `Post`, `Comment`, `Tag`  
- [ ] Set up relationships:
  - [ ] User → Posts (1:M)
  - [ ] Post → Comments (1:M)
  - [ ] Post ↔ Tags (M:M)
- [ ] Seed with Factories and Faker  
- [ ] Display nested relationships in views  

**⏱ Est. Time**: 6–7 hrs

---

## 🖼️ 5. Image Upload & Storage
- [ ] Store uploaded images via `Storage` facade  
- [ ] Use `php artisan storage:link`  
- [ ] Resize/optimize images using Intervention Image  

**⏱ Est. Time**: 2 hrs

---

## 💻 6. Artisan & CLI Tools
- [ ] Use `make:model -mcr` for full resource generation  
- [ ] Learn key Artisan commands:
  - `route:list`, `migrate`, `tinker`, etc.  
- [ ] Create a custom Artisan command (e.g. cleanup temp files)  

**⏱ Est. Time**: 2 hrs

---

## 🎁 7. Bonus (Optional)
- [ ] Explore & integrate 1 Laravel package
  - Suggestions: Spatie Permissions, Laravel Debugbar  
- [ ] Try deploying app to Render or Laravel Forge *(optional)*  

**⏱ Est. Time**: 2–3 hrs

---

## 🧘 Reflection & Review
- [ ] Write daily learning notes (Notion or Google Doc)  
- [ ] Record short Loom videos explaining key learnings (optional)  

**⏱ Ongoing**
