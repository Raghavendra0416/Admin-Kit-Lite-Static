# AdminKit Lite

A responsive, framework-free administrative interface built using **semantic HTML5 and CSS3**.

The purpose of this project is to understand how modern web interfaces are structured and styled using native browser capabilities before introducing JavaScript frameworks or component libraries.

---

## 📌 Project Overview

**AdminKit Lite** is a small administrative dashboard consisting of four pages:

- Dashboard
- Users
- Settings
- Community Event Registration

The project focuses on building a clean, responsive, accessible interface using only HTML and CSS.

No JavaScript or frontend framework is used in this project.

---

## 🎯 Project Objectives

The main objectives of this project are to practice:

- Semantic HTML
- HTML forms
- Native interactive elements
- CSS cascade
- CSS box model
- CSS custom properties
- Flexbox
- CSS Grid
- Responsive design
- Keyboard accessibility
- Focus accessibility
- Tables
- Form controls
- Browser DevTools
- Organizing CSS into multiple files

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and semantic markup |
| CSS3 | Styling and responsive layout |
| CSS Custom Properties | Centralized design tokens |
| Flexbox | Navigation and layout alignment |
| CSS Grid | Dashboard cards and search layout |
| Browser DevTools | Testing and debugging |

### Not Used

- JavaScript
- React
- Bootstrap
- Tailwind CSS
- jQuery
- Any JavaScript framework or UI library

---

# 📂 Project Structure

```text
adminkit-lite/
│
├── index.html
├── users.html
├── settings.html
├── registration.html
│
├── styles/
│   ├── token.css
│   ├── base.css
│   ├── layout.css
│   ├── components.css
│   └── pages.css
│
└── README.md
```

---

# 📄 Pages

## 1. Dashboard

**File:** `index.html`

The Dashboard provides an overview of the system.

### Includes

- Admin welcome message
- Navigation links
- Total users
- Active users
- Pending tasks
- Recent activity
- System status
- Footer

### Example Dashboard Cards

```text
Total Users       120
Active Users       98
Pending Tasks      15
```

The dashboard cards use CSS Grid on larger screens and become a single-column layout on smaller screens.

---

## 2. Users

**File:** `users.html`

The Users page provides a simple user-management interface.

### Includes

- Users page introduction
- Search users form
- User table
- User name
- Email
- Role
- Status
- Joined date

The table uses semantic HTML elements such as:

```html
<table>
<thead>
<tbody>
<tr>
<th>
<td>
<caption>
```

Column headers use:

```html
<th scope="col">
```

to improve table accessibility.

---

## 3. Settings

**File:** `settings.html`

The Settings page demonstrates how forms can be organized into meaningful groups.

### Profile

Contains:

- Full Name
- Email Address

### Notifications

Contains:

- Email Notifications
- Push Notifications
- SMS Notifications

### Security

Contains:

- Password
- Confirm Password
- Two-Factor Authentication

The form uses semantic:

```html
<fieldset>
<legend>
```

elements to group related controls.

---

## 4. Community Event Registration

**File:** `registration.html`

This page demonstrates a complete event registration form.

### Includes

- Event information
- Full Name
- Email Address
- Experience Level
- Dietary Requirements
- Terms and Conditions
- Register button
- Cancel action
- Example success message
- Example validation error

The form uses native HTML controls such as:

```html
<input>
<select>
<textarea>
<input type="checkbox">
<button>
```

Required fields use the native:

```html
required
```

attribute.

---

# 🎨 CSS Architecture

The CSS is separated into five files.

This keeps the project organized and demonstrates how larger projects can separate responsibilities instead of putting everything into one stylesheet.

---

## `token.css`

Contains the project's design tokens using CSS Custom Properties.

Examples:

```css
:root {
    --color-primary: #4f46e5;
    --color-background: #f8fafc;
    --color-surface: #ffffff;

    --space-sm: 0.5rem;
    --space-md: 1rem;
    --space-lg: 1.5rem;

    --radius-md: 0.5rem;
}
```

These variables are reused throughout the other CSS files.

For example:

```css
.card {
    background-color: var(--color-surface);
    padding: var(--space-lg);
    border-radius: var(--radius-lg);
}
```

This provides consistency and makes the design easier to maintain.

---

## `base.css`

Contains global styles and default styling for HTML elements.

Responsibilities include:

- Global reset
- Typography
- Links
- Form controls
- Buttons
- Checkboxes
- Tables
- Lists
- Focus styles
- Horizontal rules

---

## `layout.css`

Controls the overall page structure.

Responsibilities include:

- Header
- Navigation
- Main content width
- Footer
- Mobile layout
- Tablet layout
- Responsive navigation

---

## `components.css`

Contains reusable UI components.

Examples:

- Dashboard cards
- Activity section
- System status section
- Forms
- Fieldsets
- Buttons
- Form actions
- User table
- Success/error components

---

## `pages.css`

Contains styles specific to individual pages.

Examples:

```text
Dashboard
Users
Settings
Registration
```

This prevents page-specific styling from unnecessarily affecting other pages.

---

# 🔗 CSS Loading Order

Each HTML page loads the stylesheets in this order:

```html
<link rel="stylesheet" href="styles/token.css">
<link rel="stylesheet" href="styles/base.css">
<link rel="stylesheet" href="styles/layout.css">
<link rel="stylesheet" href="styles/components.css">
<link rel="stylesheet" href="styles/pages.css">
```

The order provides a logical styling flow:

```text
token.css
    ↓
Design variables

base.css
    ↓
Global HTML styling

layout.css
    ↓
Page structure

components.css
    ↓
Reusable components

pages.css
    ↓
Page-specific styling
```

The files are loaded together by the HTML pages. `token.css` does not need to be imported separately into the other CSS files.

---

# 📱 Responsive Design

The project is designed to work across:

- Desktop
- Tablet
- Mobile

### Desktop

Dashboard cards appear in multiple columns:

```text
┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ Total Users │ │Active Users │ │Pending Tasks│
└─────────────┘ └─────────────┘ └─────────────┘
```

### Mobile

Cards become a single-column layout:

```text
┌─────────────────┐
│ Total Users     │
└─────────────────┘

┌─────────────────┐
│ Active Users    │
└─────────────────┘

┌─────────────────┐
│ Pending Tasks   │
└─────────────────┘
```

The navigation also changes to accommodate smaller screen sizes.

The Users table can scroll horizontally when the available screen width is insufficient.

---

# ♿ Accessibility

Accessibility was considered throughout the project.

## Semantic HTML

The project uses semantic elements such as:

```html
<header>
<nav>
<main>
<section>
<footer>
<form>
<label>
<table>
<fieldset>
<legend>
```

These elements provide meaningful structure to the document.

---

## Form Labels

Form controls are associated with labels using `for` and `id`.

Example:

```html
<label for="email">Email Address</label>

<input
    type="email"
    id="email"
    name="email"
>
```

---

## Native Interactive Elements

The project uses native HTML controls instead of recreating them with generic elements.

Examples:

```html
<button>
<input>
<select>
<textarea>
<a>
```

Native controls provide built-in browser behavior and accessibility.

---

## Keyboard Accessibility

Interactive elements can be reached using the keyboard.

The project also provides visible focus styles using:

```css
:focus-visible
```

This helps users identify which element currently has keyboard focus.

---

# 🧱 CSS Concepts Practiced

## CSS Box Model

The project uses:

```text
Content
   ↓
Padding
   ↓
Border
   ↓
Margin
```

The global rule:

```css
* {
    box-sizing: border-box;
}
```

makes width and height calculations easier to manage.

---

## Flexbox

Flexbox is used primarily for:

- Header alignment
- Navigation
- Form actions
- Responsive alignment

Example:

```css
.site-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
```

---

## CSS Grid

CSS Grid is used for the dashboard cards.

Example:

```css
.cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
}
```

On smaller screens:

```css
.cards {
    grid-template-columns: 1fr;
}
```

---

# 🧪 Testing

The project should be tested using browser DevTools.

### Responsive Testing

Test the application at:

```text
Desktop
Tablet
Mobile
```

### Keyboard Testing

Use the `Tab` key to navigate through:

- Navigation links
- Form controls
- Buttons
- Other interactive elements

### DevTools

Inspect:

- Box model
- Computed styles
- Flexbox
- Grid
- Responsive layouts
- Focus states

---

# 🚀 How to Run

No build tools or package installation are required.

Simply open:

```text
index.html
```

in a web browser.

Navigate between the pages using the navigation links:

```text
Dashboard
Users
Settings
Registration
```

---

# 📚 Learning Outcomes

After completing this project, the main concepts practiced are:

1. How semantic HTML structures a webpage.
2. How forms and native controls work.
3. How labels connect to form controls.
4. How the CSS box model works.
5. How CSS Custom Properties can create design tokens.
6. How Flexbox controls one-dimensional layouts.
7. How CSS Grid controls two-dimensional layouts.
8. How media queries create responsive layouts.
9. How focus states support keyboard accessibility.
10. How tables can be structured semantically.
11. How CSS can be separated according to responsibility.
12. How browser DevTools can be used to inspect and debug layouts.

---

# 📌 Project Status

**Status: Completed ✅**

The project currently includes:

- ✅ Dashboard
- ✅ Users page
- ✅ Settings page
- ✅ Community Event Registration
- ✅ Semantic HTML
- ✅ Forms
- ✅ Tables
- ✅ CSS design system
- ✅ Flexbox
- ✅ CSS Grid
- ✅ Responsive design
- ✅ Keyboard/focus accessibility
- ✅ Organized CSS architecture
- ✅ No JavaScript

---

# 👨‍💻 Author

**Raghavendra**

AdminKit Lite — HTML & CSS Practice Project
```
