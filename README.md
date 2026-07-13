# EventSphere (EventFlow) 🚀

EventSphere (EventFlow) is a premium, responsive city experience discovery, booking, and hosting platform. It is built entirely on vanilla web technologies (HTML5, CSS3, and JavaScript ES6) with an elegant, modern, dark-themed user interface.

## 🌟 Key Features

* **Event Catalog & Discovery**:
  * Browse premium events across multiple categories: **Technology**, **Music**, **Workshops**, **Art & Crafts**, **Sports & Health**, and **Food & Culinary**.
  * Dynamic, responsive events grid with custom-generated canvas placeholder banners.
* **Interactive Chatbot (EventFlow Assistant)**:
  * Floating AI-style virtual guide to help users navigate and explore categories.
  * Suggests event information, answers greetings, lists active categories, and handles fallbacks gracefully.
* **Organizer Control Panel (CRUD Workspace)**:
  * A full admin interface to manage active event listings (Create, Read, Update, Delete).
  * **Multi-Category Filter Pills**: Allows administrators to filter listings by selecting one or more categories simultaneously.
  * **Registrants Roster**: View a modal displaying detailed names and emails of all attendees registered for any specific event.
* **Seamless Authentication Flow**:
  * Auto-registers new attendee email addresses on their very first log in.
  * Securely stores and validates passwords for subsequent logins to ensure account integrity.
  * Restricts duplicate registrations during manual signup.
* **Advanced Booking Flow**:
  * Real-time seat capacity tracker.
  * Multi-ticket booking with customized guest attendee registration.
  * Dynamic cancellation fee calculator according to standard refund policies.

## 🛠️ Tech Stack

* **Structure**: Semantic HTML5
* **Styling**: Modern CSS3 (CSS Variables, HSL color palettes, Glassmorphism, Flexbox, CSS Grid)
* **Logic**: Vanilla ES6 Javascript (Modules, Web Storage APIs, Custom Event Listeners)

## 📂 Project Structure

```text
├── index.html          # Main event discovery landing page
├── booking.html        # Multi-ticket booking interface
├── portal.html         # User profile and Organizer workspace
├── css/
│   └── styles.css      # Core style definitions and theme assets
└── js/
    ├── app.js          # Controller logic for main landing page & chatbot
    ├── auth.js         # Session service, route guards, and local DB
    ├── booking.js      # Booking modal and seat reservation controller
    ├── data.js         # LocalStorage database seeds and mock API
    └── portal.js       # Profile rendering & Admin CRUD control panel
```

## 🚀 How to Run Locally

Since this is a static site powered by ES6 Javascript Modules, running it directly from the file system (`file://` protocol) will trigger CORS restrictions. You must run it using a local HTTP server:

1. **Python Server**:
   ```bash
   python3 -m http.server 8000
   ```
2. **Node.js (http-server)**:
   ```bash
   npx http-server
   ```
3. Open your browser and navigate to the local port (e.g., `http://localhost:8000`).
