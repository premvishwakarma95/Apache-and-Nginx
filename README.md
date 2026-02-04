# Apache and Nginx

This document provides a concise and beginner-friendly overview of **Apache HTTP Server** (and can be extended to Nginx) for use in project documentation or server architecture explanations.

---

## Apache

**Apache HTTP Server** is one of the most widely used open-source web servers in the world. Its primary role is to **serve websites and web applications to users over the internet**.

### 1. What Does Apache Do?

Apache listens for **HTTP/HTTPS requests** from web browsers (such as Chrome, Firefox, or Edge) and responds with the requested content, including:

* HTML pages
* CSS and JavaScript files
* Images and videos
* API responses (via backend integrations)

> **In simple terms:** Apache delivers your website when someone opens a URL in their browser.

---

### 2. How Apache Works (Simple Flow)

1. A user enters `https://example.com` in their browser.
2. The request reaches the server on:

   * **Port 80** for HTTP, or
   * **Port 443** for HTTPS.
3. Apache processes the request:

   * Locates the requested file or route
   * Applies configured rules (security, redirects, rewrites, etc.)
   * Sends the appropriate response back to the browser

---

### 3. Apache in a Real Server Setup

A typical server architecture using Apache looks like this:

```
Browser
   ↓
Apache Server
   ↓
Backend Application (PHP / Node.js / Python)
   ↓
Database (MySQL / MongoDB)
```

In this setup:

* Apache handles incoming web requests
* Backend services process business logic
* The database stores and retrieves data

---

> This structure makes Apache suitable for hosting static websites, dynamic applications, and acting as a reverse proxy for backend services.
