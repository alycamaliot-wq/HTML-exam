# Multi-Page Personal Website: HTML Exam / Assignment

A hands-on assignment for teaching **pure HTML**: semantic structure, navigation, forms, and links. Students build a small multi-page personal website **without any CSS**. The finished site can later be reused as the starting point for a **CSS exam**.

---

## 1. Overview

| | |
|---|---|
| **Subject** | HTML fundamentals |
| **Level** | Beginner |
| **Duration** | 60-90 minutes (exam) or 1-2 lessons (assignment) |
| **Tools** | Any code editor + web browser |
| **Allowed** | HTML only. No CSS, no JavaScript, no frameworks |
| **Total score** | 100 points |
| **Passing score** | 60 points |

---

## 2. What This Assignment Covers

By completing it, students demonstrate that they can:

- Use **semantic HTML elements** instead of generic `<div>` tags
- Structure content with a correct **heading hierarchy** (`h1` to `h3`)
- Build **navigation** both between pages and inside a page (anchor links)
- Separate sections with unique **`id` attributes**
- Create a **form** that collects user data with proper labels and input types
- Add **external links** (social media) and contact links (`mailto:`, `tel:`)
- Organize a project into **multiple linked files**

---

## 3. Task Description (give this to students)

Create a personal website made of **4 HTML pages**:

| Page | File | Content |
|---|---|---|
| 1 | `index.html` | About you (part 1): introduction, education, hobbies |
| 2 | `about2.html` | About you (part 2): background, experience, goals |
| 3 | `skills.html` | What you can do: skills, services, projects |
| 4 | `contact.html` | Contact form + social media links |

Every page must share the same navigation and footer, and every page must be reachable from every other page.

**Restrictions:** do not use CSS (no `<style>`, no `style=""`, no `.css` files) and do not use JavaScript.

---

## 4. The 20 Requirements (Grading Rubric)

Each requirement is worth **5 points**. Total: **100**. Pass: **60 or more** (12 requirements).

### A. Structure and Semantics (25 points)

| # | Requirement | Pts |
|---|---|---|
| 1 | Every page has a valid skeleton: `<!DOCTYPE html>`, `<html lang>`, `<head>`, `<meta charset>`, `<title>`, `<body>` | 5 |
| 2 | Every page has a **unique, meaningful `<title>`** | 5 |
| 3 | Uses semantic elements: `<header>`, `<nav>`, `<main>`, `<footer>` on every page | 5 |
| 4 | Content is grouped with `<section>` and `<article>` where appropriate (not `<div>` everywhere) | 5 |
| 5 | Exactly **one `<h1>`** per page | 5 |

### B. Headings and Content (20 points)

| # | Requirement | Pts |
|---|---|---|
| 6 | Headings follow the correct hierarchy (`h1` > `h2` > `h3`) with no skipped levels | 5 |
| 7 | Pages 1 and 2 contain real information about the student (name, education, background, goals) | 5 |
| 8 | Page 3 describes what the student can do (skills, services or projects) | 5 |
| 9 | Uses at least **one list** (`<ul>` or `<ol>`) and **one table** with `<thead>` / `<tbody>` | 5 |

### C. Navigation and IDs (25 points)

| # | Requirement | Pts |
|---|---|---|
| 10 | A **main navigation** (`<nav>` with a list of links) is present on every page | 5 |
| 11 | Main navigation links work between all 4 pages (no broken links) | 5 |
| 12 | Every `<section>` has a **unique `id`** that describes its content | 5 |
| 13 | At least **one in-page navigation** uses anchor links (`href="#id"`) that jump to those section ids | 5 |
| 14 | Pages have **Next / Previous** links so a visitor can move page to page, plus a "Back to top" link | 5 |

### D. Form (20 points)

| # | Requirement | Pts |
|---|---|---|
| 15 | `contact.html` has a `<form>` with `action` and `method` attributes | 5 |
| 16 | Every input has a matching `<label for="...">` and a `name` attribute | 5 |
| 17 | Uses at least **4 different input types** (e.g. `text`, `email`, `tel`, `number`, `date`, `radio`, `checkbox`) | 5 |
| 18 | Includes a `<select>` or `<textarea>`, a **submit button**, and at least one `required` field | 5 |

### E. Links and Contact (10 points)

| # | Requirement | Pts |
|---|---|---|
| 19 | Social media links for at least **3 platforms** (Instagram, Telegram, WhatsApp, etc.) that open in a new tab (`target="_blank"`) | 5 |
| 20 | Contact details use `mailto:` and `tel:` links; footer is present on every page | 5 |

---

## 5. Score Interpretation

| Score | Result |
|---|---|
| 90-100 | Excellent |
| 75-89 | Good |
| 60-74 | Pass |
| 0-59 | Fail: needs to retake |

**Automatic deductions (suggested):**

- Any CSS or JavaScript used: **-10 points**
- Broken links between pages: counted under #11
- Copied work: **0 points**

---

## 6. Reference Solution Structure

```
my-website/
├── index.html      → About me (1): #intro, #education, #hobbies
├── about2.html     → About me (2): #background, #experience, #goals
├── skills.html     → What I can do: #skills, #services, #projects
└── contact.html    → #contact-form, #socials
```

### Minimal page template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Me - Page 1</title>
</head>
<body id="page-about-1">

  <header id="site-header">
    <h1>Student Name</h1>

    <nav id="main-nav" aria-label="Main navigation">
      <ul>
        <li><a href="index.html">About Me (1)</a></li>
        <li><a href="about2.html">About Me (2)</a></li>
        <li><a href="skills.html">What I Can Do</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main id="main-content">
    <section id="intro">
      <h2>Introduction</h2>
      <p>...</p>
    </section>
  </main>

  <footer id="site-footer">
    <p>&copy; 2026 Student Name</p>
  </footer>

</body>
</html>
```

### Minimal form example

```html
<form action="#" method="post" id="form-contact">
  <p>
    <label for="fullname">Full name:</label>
    <input type="text" id="fullname" name="fullname" required>
  </p>
  <p>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  </p>
  <p>
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="5"></textarea>
  </p>
  <button type="submit">Send</button>
</form>
```

---

## 7. How Teachers Can Use This

1. **As an exam:** hand out Section 3 (task) and keep Section 4 (rubric) for grading.
2. **As a classroom example:** show the reference solution and walk through each requirement.
3. **As a self-check:** give students the rubric so they can score their own work before submitting.
4. **As a base for the CSS exam:** keep the students' HTML and ask them to style it. Because every section has a unique `id`, they can practise `#id` selectors, layout of `header` / `nav` / `main` / `footer`, styling forms, tables and lists, and so on.

### Quick grading checklist

- [ ] All 4 files exist and open in the browser
- [ ] No CSS / JS used
- [ ] Each page has the same nav and footer
- [ ] Section ids are unique and anchor links work
- [ ] Form has labels, varied input types, submit button
- [ ] Social links open in a new tab

---

## 8. Common Student Mistakes

| Mistake | Why it matters |
|---|---|
| Using `<div>` for everything | Misses the point of semantic HTML |
| Multiple `<h1>` on one page | Breaks heading hierarchy |
| Choosing a heading level for its size | Headings describe structure, not appearance |
| Duplicate `id` values | Ids must be unique per page |
| Inputs without `<label>` | Poor accessibility |
| Broken relative paths | Files must be in the same folder |
| Placeholder text left in (`[Your Name]`) | Content is incomplete |

---

## 9. Extension Ideas (optional)

- Add a CSS exam on top of the same site (colors, layout, navigation bar, form styling)
- Add an image with a proper `alt` attribute
- Add a `<video>` or `<audio>` element
- Add a favicon and meta description

---

*Feel free to copy, translate and adapt this assignment for your own classes.*