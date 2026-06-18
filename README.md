# Tech & Insights Blog Portal

A responsive, lightweight full-stack blogging platform that enables users to publish articles, read community posts, and engage through an interactive comments section.

## 🌟 Key Features
- **User Authentication:** Simulates session-based user login and state retention.
- **Content Management:** Full CRUD operations allowing logged-in users to create and delete their own blog posts.
- **Interactive Comment System:** Live community interaction box embedded under every individual article.
- **State Persistence:** Built-in local storage engine that retains user sessions, articles, and corresponding comments across browser refreshes.

## 🛠️ System Architecture & Logic
The platform is designed with a monolithic frontend model that decouples data management from visual rendering:
- **State Management:** Uses an array-of-objects data layout mapped to unique timestamps (`Date.now()`) acting as relational keys between specific blog posts and their corresponding comment arrays.
- **Dynamic DOM Rendering:** Features custom JS lifecycle rendering functions (`renderPosts()`) that modify elements on-the-fly depending on user authorization status.

## 💻 Tech Stack
- **Frontend Architecture:** HTML5, CSS3 (Flexbox/Grid layout processing)
- **Engine Logic:** Vanilla JavaScript (ES6+ ECMAScript standards)
- **Data Layer:** Web Storage API (Local Persistence)
