# EduTrack

EduTrack is a simple web-based student record management system built using HTML, Tailwind CSS, and vanilla JavaScript. It allows users to add, view, edit, and delete student records entirely on the client side using browser `localStorage`.


## Features

* **Home Page:** Welcome screen with navigation links to other pages.
* **Add Record:** Form to input student details including full name, student ID, department, batch, current semester, credits completed, and CGPA.
* **Student Overview:** Displays all student records in a table with options to edit or delete each record.
* **Persistent Storage:** Uses `localStorage` to save student data so records persist across page reloads.


## Project Structure

* `index.html`
  The Home page of the application with navigation and a welcome message.

* `form.html`
  The form page where users can add new student records. Submitted data is saved in `localStorage`.

* `table.html`
  The dashboard displaying all stored student records. Includes functionality to edit and delete records.


## Technologies Used

* HTML5
* Tailwind CSS (via CDN)
* Vanilla JavaScript (ES6+)
* Browser `localStorage` for data persistence


## Usage

1. **Open `index.html`** in your browser to start the EduTrack app.
2. Navigate to **Add Record** to enter a new student's information.
3. Navigate to **Student Overview** to see all stored students.
4. Use the **Edit** button to update existing student information.
5. Use the **Delete** button to remove a student record.
6. All changes are saved locally on your browser using `localStorage`.


## How It Works

* Student data is stored as an array of objects in the browser's `localStorage` under the key `"students"`.
* When a new student is added, their data is appended to this array and saved back.
* The Student Overview page reads from `localStorage`, displays all records in a table, and allows inline editing and deletion.
* The edit modal pre-fills the existing student data, and updates the record on submission.
