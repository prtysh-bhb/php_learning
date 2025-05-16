# 🧠 WordPress Zero-to-Hero (Weekend Plan + Laravel/Vue Mapping)

A focused, minimal yet powerful roadmap to master WordPress as a team lead — in just a few weekends.

---

## 🗓️ Weekend Plan: 4-Week Sprint

### ✅ Weekend 1: Foundation & WP Thinking

**Time:** 3–4 hours  
**Focus:**
- WordPress architecture (Themes, Plugins, Core)
- Admin UI: Roles, Pages, Posts, CPTs

**Tasks:**
- Install WordPress (via LocalWP, XAMPP)
- Explore the admin dashboard
- Install a couple of common plugins (e.g., ACF)

**Read:**
- https://wordpress.org/support/article/first-steps-with-wordpress/
- https://developer.wordpress.org/themes/getting-started/

---

### ✅ Weekend 2: Theme Anatomy & Hooks

**Time:** 4–5 hours  
**Focus:**
- Template hierarchy (`single.php`, `index.php`, etc.)
- `functions.php` and theme setup
- Hooks: `add_action`, `add_filter`

**Tasks:**
- Create a child theme
- Register a menu, enqueue styles/scripts
- Add a widget area or a shortcode

**Read:**
- https://developer.wordpress.org/themes/basics/
- https://developer.wordpress.org/themes/basics/template-hierarchy/

---

### ✅ Weekend 3: Plugins, ACF, and CPTs

**Time:** 5–6 hours  
**Focus:**
- Writing a basic plugin
- Registering Custom Post Types (CPTs)
- Using Advanced Custom Fields (ACF)

**Tasks:**
- Create a "Books" CPT with ACF fields
- Use `WP_Query` to fetch and display content

**Read:**
- https://www.advancedcustomfields.com/resources/
- https://developer.wordpress.org/plugins/

---

### ✅ Weekend 4: QA, Code Review & Deployment

**Time:** 3–4 hours  
**Focus:**
- Code quality & security
- Plugin bloat, optimization
- Backups & deployment workflows

**Tasks:**
- Review a plugin/theme for performance or security issues
- Try a migration plugin (e.g., All-in-One WP Migration)

**Read:**
- https://developer.wordpress.org/plugins/security/
- https://kinsta.com/blog/wordpress-security/

---

## 🔄 WordPress vs Laravel/Vue: Mental Mapping

| Concept                    | WordPress                                   | Laravel Equivalent              | Vue Equivalent            |
|----------------------------|---------------------------------------------|----------------------------------|----------------------------|
| **Theme Templates**        | `single.php`, `page.php`, `archive.php`     | Blade templates (`.blade.php`)  | Vue components             |
| **functions.php**          | Adds features, registers assets             | `AppServiceProvider`, helpers   | Global config / mixins     |
| **Hooks (actions/filters)**| `add_action`, `add_filter`                  | Events, middleware, listeners   | Lifecycle hooks            |
| **Plugins**                | Extends core functionality                  | Laravel packages, service layer | Vue plugins, Vuex modules  |
| **Custom Post Types (CPTs)**| Define new entities (e.g., "Books")        | Models + Controllers            | Vuex store modules         |
| **ACF / Metaboxes**        | Admin UI for custom fields                  | FormRequest + Blade             | Dynamic Forms              |
| **WP_Query / get_posts()** | Custom data fetch                           | Eloquent query builder          | Axios or fetch             |
| **Admin Panel**            | `wp-admin` dashboard                        | Laravel Nova / Voyager          | Vue admin UI               |

---

## 🧭 WordPress File Structure at a Glance
```
wordpress/
├── wp-admin/ # Core admin files (Do NOT touch)
├── wp-includes/ # Core functionality files (Do NOT touch)
├── wp-content/ # Only place you'll work in
│ ├── plugins/ # Custom or 3rd-party plugins
│ │ └── my-plugin/
│ │ ├── my-plugin.php # Main plugin file (header + logic)
│ │ ├── post-types.php # CPTs, taxonomies
│ │ ├── shortcodes.php # Custom shortcodes
│ │ └── assets/ # JS, CSS used in plugin
│ │ ├── js/
│ │ └── css/
│ │
│ └── themes/ # Active theme directory
│ └── my-theme/
│ ├── style.css # Theme metadata + styles
│ ├── index.php # Main fallback template
│ ├── single.php # Post detail page
│ ├── page.php # Static page template
│ ├── archive.php # List view for CPTs/posts
│ ├── functions.php # Theme features, menus, etc.
│ ├── template-parts/ # Reusable HTML chunks
│ └── assets/
│ ├── js/
│ └── css/
│ └── screenshot.png # Theme preview image
├── wp-config.php # DB credentials, WP constants
├── .htaccess / nginx.conf # Server config
└── .env (if using Bedrock) # Environment variables (optional setup)
```


---

*Crafted with ❤️ and caffeine by Pratyush (PT) — guiding Wordpress journeys from zero to hero.*
