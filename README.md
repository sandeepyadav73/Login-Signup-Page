# Glassmorphism Login & Signup Form

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://en.wikipedia.org/wiki/HTML5)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://en.wikipedia.org/wiki/CSS)
[![Responsive](https://img.shields.io/badge/Responsive-Yes-brightgreen?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ0IDZoMTR2MTJING0xMC04djZoNFY5bS05IDB2MWgyVjltLTcgMHY2aDR2LTZINHoiLz48cGF0aCBkPSJNMjAgMkg0Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bTAgMThINGYtMiAyVjRjMC0xLjEuOS0yIDItMmgxNmMxLjEgMCAyIC45IDIgMnYxNmYyLTJ6Ii8+PC9zdmc+)](https://www.w3schools.com/css/css_rwd_intro.asp)

A modern, fully responsive Login and Signup form built with **pure HTML5 and CSS3**. This project features a stunning glassmorphism effect and a seamless toggle between the two forms **without a single line of JavaScript.**

<img width="471" height="368" alt="image" src="https://github.com/user-attachments/assets/d6544d93-44e0-4ff1-b41a-3f0f9fbe2b51" /><img width="471" height="368" alt="image" src="https://github.com/user-attachments/assets/ec0d5b00-c609-47cb-9bff-4771a4804763" />


## ✨ Key Features

* **Modern Glassmorphism UI:** A beautiful "frosted glass" effect using `backdrop-filter`.
* **Pure CSS Form Toggle:** Switches between Login and Signup forms using the "Checkbox Hack" (no JavaScript needed).
* **Font Awesome Icons:** Clear visual cues for input fields (user, email, password).
* **Smooth Transitions:** Soft focus effects on inputs and hover animations on buttons.
* **Fully Responsive:** Looks great on all devices, from mobile phones to desktops, using a Flexbox-centered layout.
* **Gradient Button:** A subtle gradient on the primary button for a modern aesthetic.

---

## 💡 Core Concept: The "Checkbox Hack"

The most powerful feature of this project is its ability to switch forms without JavaScript. This is achieved using a hidden checkbox and CSS pseudo-selectors.

1.  An invisible `<input type="checkbox" id="form-switch">` is placed on the page.
2.  The "Sign up" and "Login" links are actually `<label>` elements pointing to this checkbox (`<label for="form-switch">`).
3.  When a user clicks the label, it toggles the checkbox's `:checked` state.
4.  CSS rules using the `:checked` pseudo-class and the general sibling selector (`~`) are used to show/hide the correct form container.

**Example CSS Logic:**
```css
/* By default, hide the Signup form */
.signup-container {
    display: none;
}

/* When the checkbox is checked, hide Login... */
#form-switch:checked ~ .login-container {
    display: none;
}

/* ...and show Signup */
#form-switch:checked ~ .signup-container {
    display: block;
}

## 🛠️ Technologies Used

* **HTML5:** Semantic markup for structure.
* **CSS3:**
    * **Flexbox:** For centering the form container perfectly.
    * **`backdrop-filter`:** To create the glassmorphism effect.
    * **`transition`:** For smooth hover and focus animations.
    * **Pseudo-classes (`:checked`, `:focus`):** To control UI states.
    * **Sibling Selector (`~`):** To power the form switch.
    * **Media Queries:** For mobile responsiveness.
* **Font Awesome:** For scalable vector icons.

---

## 🚀 How to Use

No setup or dependencies required!

1.  **Clone or download** this repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Navigate** to the project folder.
3.  **Open `index.html`** in your favorite web browser.
