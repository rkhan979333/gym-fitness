# README: TRAIN THE FIGHTER IN YOU - Fitness Guidance Platform

## 1. Project Title
**Fitness Guide Pro: TRAIN THE FIGHTER IN YOU**

## 2. Project Goal
* To provide a comprehensive, interactive front-end platform offering structured fitness guidance.
* This project serves as a minimum viable product (MVP) for a full-scale web application.
* The focus is on high-value user tools like personalized plans and an integrated calculator.

## 3. Technology Stack
* **Markup:** HTML5 (Used across all pages, e.g., `gym3.html`, `cal.html`, `div1.html`, etc.).
* **Styling:** Custom CSS3 (Internal `<style>`).
    * Defines visual hierarchy, responsive layout, and interactive states (e.g., card hovers).
* **Client-Side Logic:** Vanilla JavaScript.
    * Powers all interactivity, including the Macronutrient Calculator logic and the navigation between content pages.

## 4. Technical Architecture: Multi-Page Application (MPA)

* The project utilizes a basic Multi-Page Application (MPA) model for content separation.
* **Primary Entry Point:** `gym3.html` (Home/Dashboard).
* **Navigation:** Handled primarily via standard HTML anchors (`<a href="filename.html">`) linking the main page to separate content modules.
* **Modular Tools:** The interactive Macronutrient Calculator resides in a dedicated module (`cal.html` or a visible form block) using Vanilla JS for client-side computation (TDEE/Macro Split).

## 5. Deployment and Setup

* This is a zero-dependency project.
* **Environment:** Requires only a modern web browser.
* **Execution:** Launch the application by opening `gym3.html` directly in the browser.

## 6. Core Functionality Breakdown

* **Plan Display:** Content is split across six separate HTML files (`div1.html` - `div6.html`). The main page acts as a directory.
* **Macronutrient Calculator:** Custom JavaScript logic implementing a simplified TDEE/BMR calculation method.
    * Results are calculated instantly on form submission without server contact.
    * *Note:* Logic is implemented but requires activation (uncommenting the script).
* **Styling:** Uses CSS variables (`--primary-color`, etc.) for theme consistency.

## 7. Future Development Roadmap

* **Decoupling Assets:** Separate all inline CSS and JavaScript into external `styles.css` and `script.js` files to enhance caching, maintainability, and code hygiene.
* **Calculator Upgrade:** Implement the more accurate Mifflin-St Jeor equation for BMR calculation.
* **Advanced Interactivity:** Refactor the navigation to use AJAX/Fetch API to load plan content asynchronously onto the main page, converting the MPA structure to a hybrid or full SPA model.
* **User Data Persistence:** Introduce a cloud-based backend service (e.g., Firebase, AWS Amplify) to save calculated macro results and plan selections.