# 🔍 Lost and Found Web App – README

Welcome to the official documentation and submission guidelines for the **Lost and Found Web Application Project**.

This project is designed to guide you through the full web development lifecycle – from basic HTML/CSS/JS to advanced backend technologies – by building a full-stack Lost and Found portal.

---

## 🧰 Tech Stack Used

| Layer         | Technologies Used                                               |
|---------------|----------------------------------------------------------------|
| **Frontend**  | HTML, CSS, JavaScript, React.js, Bootstrap, Material UI        |
| **Backend**   | Node.js, Express.js                                            |
| **Database**  | PostgreSQL (using Filess.io hosting)                           |
| **API Tools** | Postman, ThunderClient (VS Code extension)                     |
| **Version Control** | Git, GitHub                                             |
| **Deployment (Optional)** | Render / Vercel / Netlify / Railway (suggested) |

---

## 📆 Week-wise Plan

### 🟢 Week 0: Frontend Basics – *HTML, CSS, JavaScript*
**Deadline**: 15th May EOD

- Learn and practice HTML, CSS, and JavaScript fundamentals.
- Complete beginner tutorials and reference docs.

---

### 📝 Assignment 0: Personal Resume Website
**Deadline**: 21st May EOD

Build a **Personal Information Website** using HTML, CSS, and JavaScript.  
Include:
- Dynamic greeting message (Good Morning/Afternoon/Evening)
- Current date and weekday using JS
- Sections for:
  - Name
  - About Me
  - Education
  - Skills
  - Hobbies
  - Contact Details
- At least one profile image and other relevant images

---

### ⚛️ Week 1: Advanced Frontend – *React + UI Libraries*
**Deadline**: 31st May EOD

- React basics: components, props, state, hooks
- UI Libraries: Bootstrap & Material UI
- Setup your first React app

---

### 📝 Assignment 1: Frontend for Lost and Found
**Deadline**: 14th June EOD

- Create a **React-based frontend** for your Lost and Found site.
- Include pages like:
  - Home
  - Lost Items
  - Found Items
  - Add Item Form
  - About/Contact
- No need to make login/register functional yet.

---

### 🖥️ Week 2 & 3: Backend Development – *CRUD APIs*
**Deadline**: 29th June EOD

- Build CRUD APIs using **Node.js + Express.js**
- Connect to **PostgreSQL** hosted on Filess.io
- Create and test routes using **Postman**

#### APIs to Implement:
- `POST /items` → Add lost/found item
- `GET /items` → View all items
- `PUT /items/:id` → Update item info
- `DELETE /items/:id` → Delete item

#### PostgreSQL Table Schema:
```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  description TEXT,
  status TEXT CHECK (status IN ('lost', 'found', 'returned to owner')),
  location TEXT,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);



# Submission Guidelines

Welcome to the submission guidelines for your assignments. Please follow the instructions carefully to ensure your submission is correctly processed.

## Steps for Submission

1. **Fork the Repository**:
   - Begin by creating a fork of the main repository to your own GitHub account.

2. **Upload Your Submission**:
   - Navigate to the appropriate assignment folder. Each assignment has its own dedicated folder under `Assignments`.
   - Upload your **project folder** into the corresponding assignment folder. The name of your folder should follow this format:
     - `Assignment_0_<Your Roll Number>`
     - **Example**: If your roll number is `230540`, your folder should be named `Assignment_0_230540` and placed in `Assignments/Assignment0`.

3. **Create a Pull Request**:
   - After uploading your folder, create a pull request to the main repository.
   - Ensure that your pull request includes all necessary details and any relevant comments about your submission.

## Example

If you are submitting your assignment for Assignment 0 and your roll number is `230540`, the steps would be:

1. Fork the repository.
2. Upload your folder named `Assignment_0_230540` to the folder `Assignments/Assignment0`.
3. Create a pull request with your changes.

By following these steps, you ensure that your assignment is correctly submitted and will be reviewed.

Thank you for your cooperation!

---

Feel free to reach out if you have any questions or need further assistance.
