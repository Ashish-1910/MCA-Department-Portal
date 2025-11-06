# MCA Department Portal (Static Prototype)

This project is a static front-end prototype for a comprehensive **MCA Department Portal** for the University Institute of Computing (UIC), Chandigarh University. It was submitted in partial fulfillment of the requirements for the Master of Computer Applications (MCA) degree.

The entire portal is built using only client-side technologies (**HTML, CSS, and JavaScript**) to serve as a high-fidelity proof-of-concept. It demonstrates the user interface, information architecture, and navigation of a potential future dynamic system.

**Key Characteristic:** This project features **no backend or database**. All student data, grades, and course information are hard-coded directly into the HTML files to simulate the user experience.

---

## 🏛️ Project Architecture

This project's navigation system is built using the HTML `<frameset>` element. This creates a persistent header and a separate content window.

* `mainframe.html`: The parent file that defines the layout, splitting the viewport into a 10% header and a 90% content area.
* `quick.html` (Header Frame): The top frame that contains the persistent navigation bar.
* `contentFrame` (Content Frame): The main frame that loads all other pages (like `new.html`, `profile.html`, etc.) when a user clicks a navigation link.



---

## ✨ Key Features

* **Persistent Navigation:** The `<frameset>` architecture keeps the navigation bar visible at all times while the content below it changes.
* **Homepage:** A landing page (`new.html`) with departmental info, a video, a `<marquee>` for announcements, and CSS-animated carousels for reviews and logos.
* **Student Profiles:** A student list page (`profile.html`) that links to detailed individual profile pages (e.t., `arudh.html`).
* **Grade Reports:** A master grade list (`grades.html`) that links to detailed individual report cards (e.g., `arudh-grade.html`).
* **Course Specializations:** Static pages detailing the various MCA specializations offered.
* **Static Registration Form:** A multi-field registration form (`registration.html`) that, upon submission, navigates to a `thankyou.html` page.
* **Client-Side Validation:** The registration form features robust, client-side JavaScript validation for:
    * **Name/Surname:** Alphabets and spaces only.
    * **Aadhaar:** Must match the `1234-5678-9012` format.
    * **Contact No.:** Must be a valid 10-digit Indian mobile number.
    * **Email:** Must end in `@gmail.com`, `@hotmail.com`, or `@outlook.com`.
    * **Date of Birth:** User must be at least 18 years old (dynamically calculated).

---

## 🚀 How to Run

No installation, build steps, or dependencies are required.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/mca-department-portal.git](https://github.com/your-username/mca-department-portal.git)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd mca-department-portal
    ```
3.  **Open the main file:**
    Find the `mainframe.html` file and open it in your web browser.

    > **Important:** You must open `mainframe.html`, as it is the parent container that loads all other pages into the frames. Opening `profile.html` or `new.html` directly will result in a broken (or missing) navigation bar.

---

## 🛠️ Technologies Used

* **HTML5:** Used for the core structure, content, and layout (including `<table>`, `<form>`, and `<frameset>`).
* **CSS3:** Used for all styling, layout (Flexbox/Grid), and animations (`@keyframes` for carousels).
* **JavaScript (ES6+):** Used exclusively for client-side form validation on the registration page.

---

## 📸 Screenshots

| Homepage | Student Profile List |
| :---: | :---: |
| 

[Image of Homepage]
 | 

[Image of Profile List Page]
 |
| **Detailed Grade Report** | **Registration Form** |
|  | 

[Image of Registration Form]
 |

---

## 🔮 Future Scope

This static prototype serves as a solid foundation ("Version 1.0"). The logical next step ("Version 2.0") would be to build a dynamic, database-driven application.

* **Backend & Database:** Re-implement the system with a server-side language (like Node.js, Python/Django, or PHP) and a database (MySQL, PostgreSQL, or MongoDB).
* **Dynamic Content:** Fetch all student/grade information from the database instead of hard-coding it.
* **User Authentication:** Implement a secure login system with roles (Admin, Faculty, Student).
* **Admin Dashboard:** Create a CRUD (Create, Read, Update, Delete) interface for admins to manage records.
* **Modern Frontend:** Replace the deprecated `<frameset>` with a modern SPA (React, Angular) or a server-side templating engine.
* **Live Form Submission:** Connect the registration form to the backend to actually save new user data.

---

## 🎓 Academic Context

This project was submitted as part of the MCA program at **Chandigarh University**.

* **Author:** Ashish (25MCA20104)
* **Supervisor:** Dr. Krishan Tulli (HOD, UIC)
