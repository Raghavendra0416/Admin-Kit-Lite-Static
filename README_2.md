# AdminKit Lite

A responsive, framework-free administrative interface built using **semantic HTML5 and CSS3**.

The project was created to practice core HTML and CSS concepts, browser behavior, responsive design, accessibility, and CSS organization before moving into JavaScript or frontend frameworks.

---

# 📚 Topics Covered

The following topics were practiced during this project.

## HTML Topics

### HTML Fundamentals
- HTML document structure
- `<!DOCTYPE html>`
- `<html lang="">`
- `<head>`
- `<body>`
- `<meta charset>`
- Viewport meta tag
- `<title>`
- External CSS linking

### Semantic HTML
- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<footer>`
- `<form>`
- `<fieldset>`
- `<legend>`

### Text and Content
- Headings: `<h1>`, `<h2>`, `<h3>`
- Paragraphs: `<p>`
- Lists: `<ul>`, `<li>`
- Horizontal rules: `<hr>`

### Links and Navigation
- `<a>`
- `href`
- Navigation between multiple HTML pages

### Forms
- `<form>`
- `<label>`
- `<input>`
- `<select>`
- `<option>`
- `<textarea>`
- `<button>`
- Text input
- Email input
- Password input
- Search input
- Checkbox
- `required`
- `placeholder`
- `autocomplete`
- `name`
- `id`
- `action`
- `method`

### Form Accessibility
- Connecting `<label>` with `<input>` using `for` and `id`
- `aria-label`
- Native form controls
- Keyboard-accessible controls
- Native browser validation

### Tables
- `<table>`
- `<caption>`
- `<thead>`
- `<tbody>`
- `<tr>`
- `<th>`
- `<td>`
- `scope="col"`

### Other HTML Concepts
- Native interactive elements
- Semantic document structure
- Basic HTML accessibility
- Browser-native form behavior

---

# 🎨 CSS Topics

## CSS Fundamentals
- External CSS
- CSS syntax
- Selectors
- Properties and values
- CSS comments
- CSS cascade
- Specificity
- Source order
- Inheritance

## CSS Box Model
- Content
- Padding
- Border
- Margin
- `box-sizing`
- `border-box`

## Typography
- `font-family`
- `font-size`
- `font-weight`
- `line-height`
- Heading styles
- Paragraph styles
- Text colors

## Colors and Visual Styling
- `color`
- `background-color`
- Borders
- Border radius
- Box shadows

## CSS Custom Properties
- `:root`
- CSS variables
- `var()`
- Design tokens
- Centralized colors
- Centralized spacing
- Centralized font sizes
- Centralized border radius
- Centralized shadows

## Flexbox
- `display: flex`
- `flex-direction`
- `justify-content`
- `align-items`
- `flex-wrap`
- `gap`
- Responsive Flexbox layouts

> Flexbox was already familiar/practiced and was also used in this project.

## CSS Grid
- `display: grid`
- `grid-template-columns`
- `repeat()`
- `fr`
- `gap`
- Responsive Grid layouts

> CSS Grid was introduced and used in this project. More dedicated Grid practice will be done separately.

## Responsive Design
- Media queries
- Breakpoints
- Desktop layouts
- Tablet layouts
- Mobile layouts
- Responsive navigation
- Responsive cards
- Responsive forms
- Responsive tables

> Responsive design was implemented and tested. More dedicated media-query practice will be done separately.

## Pseudo-classes and States
- `:hover`
- `:focus`
- `:focus-visible`

## Forms and Controls
- Input styling
- Select styling
- Textarea styling
- Checkbox styling
- Button styling
- Focus states
- Hover states

## Tables
- Table width
- `border-collapse`
- Cell padding
- Borders
- Header styling
- Responsive table handling

## CSS Architecture
- Separation of concerns
- Design tokens
- Global styles
- Layout styles
- Component styles
- Page-specific styles
- Multiple stylesheet organization

---

# ♿ Accessibility Topics

The project also practiced:

- Semantic HTML
- Native interactive elements
- Form labels
- Label/input association
- Keyboard navigation
- Focus visibility
- `:focus-visible`
- Table accessibility
- `scope="col"`
- Accessible form controls
- Browser-native validation

---

# 🛠️ Browser & DevTools Topics

The project was tested using browser DevTools.

Topics practiced:

- Inspecting HTML elements
- Inspecting CSS
- Styles panel
- Computed styles
- CSS box model
- Flexbox inspection
- Grid inspection
- Responsive/device mode
- Debugging CSS
- Testing different viewport sizes
- Keyboard accessibility testing

---

# 📁 Project Structure

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

# 📄 Files and Topics Used

Instead of repeating the complete topic list on every page, this section shows **which topics are actually used by each file**.

---

## `index.html` — Dashboard

The Dashboard provides an overview of the system.

### HTML Topics Used

- Basic HTML document structure
- Semantic HTML
- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<footer>`
- Headings
- Paragraphs
- Links
- Lists
- Navigation between pages

### CSS Topics Used

- CSS variables
- Typography
- Colors
- Backgrounds
- Spacing
- Borders
- Border radius
- Box shadows
- Flexbox
- CSS Grid
- Responsive design
- Media queries
- Hover states
- Focus states
- Card styling

### Main UI Components

- Site header
- Navigation
- Dashboard overview
- Statistics cards
- Recent activity
- System status
- Footer

---

# `users.html` — Users Page

The Users page provides a basic user-management interface.

### HTML Topics Used

- Semantic HTML
- Forms
- `<label>`
- Search input
- `<button>`
- Tables
- `<caption>`
- `<thead>`
- `<tbody>`
- `<tr>`
- `<th>`
- `<td>`
- `scope="col"`
- Links

### CSS Topics Used

- CSS variables
- Form styling
- Flexbox
- CSS Grid
- Table styling
- Borders
- Spacing
- Typography
- Button styling
- Responsive design
- Horizontal table scrolling
- Media queries
- Hover states
- Focus states

### Main UI Components

- Users introduction
- Search form
- Search button
- User table
- Table caption
- User status information

---

# `settings.html` — Settings Page

The Settings page demonstrates how a larger form can be separated into logical groups.

### HTML Topics Used

- Semantic HTML
- Forms
- `<form>`
- `<fieldset>`
- `<legend>`
- `<label>`
- Text input
- Email input
- Password input
- Checkbox
- `required`
- `autocomplete`
- `placeholder`
- `id`
- `name`
- Submit button

### CSS Topics Used

- CSS variables
- Form styling
- Flexbox
- Fieldset styling
- Input styling
- Checkbox styling
- Button styling
- Spacing
- Borders
- Border radius
- Responsive forms
- Focus states
- Hover states

### Form Sections

```text
Profile
├── Full Name
└── Email Address

Notifications
├── Email Notifications
├── Push Notifications
└── SMS Notifications

Security
├── Password
├── Confirm Password
└── Two-Factor Authentication
```

---

# `registration.html` — Community Event Registration

The Registration page demonstrates a complete HTML form for a community technology meetup.

### HTML Topics Used

- Semantic HTML
- Headings
- Paragraphs
- Sections
- Forms
- Labels
- Text input
- Email input
- Select
- Option
- Textarea
- Checkbox
- Button
- Links
- `required`
- `autocomplete`
- `placeholder`
- `action`
- `method`
- `aria-label`
- Example success message
- Example validation error

### CSS Topics Used

- CSS variables
- Form styling
- Flexbox
- Input styling
- Select styling
- Textarea styling
- Checkbox styling
- Button styling
- Form actions
- Success message styling
- Error message styling
- Borders
- Border radius
- Spacing
- Responsive layout
- Focus states
- Hover states

### Form Flow

```text
Event Information
       ↓
Personal Information
       ↓
Experience Level
       ↓
Dietary Requirements
       ↓
Terms & Conditions
       ↓
Register / Cancel
```

---

# 🎨 CSS Files and Their Responsibilities

The CSS is separated into five files.

---

## `token.css`

### Purpose

Stores reusable design values rather than styling individual elements.

### Contains

- Colors
- Spacing
- Font sizes
- Border radius
- Shadows
- Content width

Example:

```css
:root {
    --color-primary: #2563eb;
    --color-background: #f1f5f9;
    --color-surface: #ffffff;

    --space-sm: 0.5rem;
    --space-md: 1rem;
    --space-lg: 1.5rem;

    --radius-md: 0.5rem;
}
```

These variables are consumed by the other CSS files using:

```css
var(--variable-name)
```

---

# `base.css`

### Purpose

Provides global/default styling for HTML elements.

### Topics Used

- CSS reset
- `box-sizing`
- Typography
- Links
- Form controls
- Buttons
- Lists
- Tables
- Focus styles
- Horizontal rules

Examples:

```css
body
h1
h2
h3
p
a
input
select
textarea
button
table
th
td
ul
hr
```

---

# `layout.css`

### Purpose

Controls the overall structure of the application.

### Topics Used

- Flexbox
- Header layout
- Navigation layout
- Main content width
- Footer
- Spacing
- Responsive layout
- Media queries

Main elements:

```text
.site-header
.nav-links
main
footer
```

---

# `components.css`

### Purpose

Styles reusable UI components.

### Components Used

- Dashboard cards
- Activity section
- Status section
- Forms
- Fieldsets
- Buttons
- Form actions
- Checkbox groups
- User table
- Success messages
- Error messages

### Topics Used

- CSS Grid
- Flexbox
- CSS variables
- Borders
- Border radius
- Shadows
- Spacing
- Responsive components
- Form styling

---

# `pages.css`

### Purpose

Contains styling specific to individual pages.

### Pages Covered

```text
Dashboard
Users
Settings
Registration
```

### Topics Used

- Page-specific spacing
- Page-specific layouts
- CSS Grid
- Flexbox
- Responsive styling
- Media queries
- Component positioning
- Form layout
- Success/error message styling

---

# 🔗 CSS Loading Architecture

Every HTML page loads the stylesheets in the following order:

```html
<link rel="stylesheet" href="styles/token.css">
<link rel="stylesheet" href="styles/base.css">
<link rel="stylesheet" href="styles/layout.css">
<link rel="stylesheet" href="styles/components.css">
<link rel="stylesheet" href="styles/pages.css">
```

The relationship is:

```text
token.css
    │
    │ Defines reusable CSS variables
    ↓
base.css
    │
    │ Global HTML styles
    ↓
layout.css
    │
    │ Overall page structure
    ↓
components.css
    │
    │ Reusable UI components
    ↓
pages.css
    │
    │ Page-specific styling
    ↓
Final rendered page
```

The CSS files do not need to import one another.

All five stylesheets are loaded by the HTML page, so the variables defined in `token.css` are available to the other stylesheets.

---

# 📱 Responsive Design

The application was designed and tested for different screen sizes.

## Desktop

- Horizontal navigation
- Three-column dashboard cards
- Wider content area
- Multi-column search layout

## Tablet

- Flexible navigation
- Adjusted content width
- Responsive cards and forms

## Mobile

- Vertical navigation
- Single-column dashboard cards
- Stacked form actions
- Responsive forms
- Horizontally scrollable users table

Example breakpoint:

```css
@media (max-width: 768px) {
    ...
}
```

A smaller breakpoint is also used:

```css
@media (max-width: 480px) {
    ...
}
```

Responsive behavior was tested using browser DevTools.

---

# ♿ Accessibility Implementation

Accessibility was considered as part of the HTML and CSS implementation.

### Semantic Structure

```html
<header>
<nav>
<main>
<section>
<footer>
```

### Form Accessibility

```html
<label for="email">Email Address</label>
<input id="email" type="email">
```

### Table Accessibility

```html
<th scope="col">Name</th>
```

### Keyboard Accessibility

Interactive elements use native HTML controls so they can be accessed through the keyboard.

### Focus Accessibility

Visible focus styles are provided using:

```css
:focus-visible
```

---

# 🧪 Testing Completed

The project was tested for:

### Responsive Design

- Desktop
- Tablet
- Mobile
- Different viewport sizes
- Navigation behavior
- Dashboard card behavior
- Form layout
- Table overflow

### Accessibility

- Keyboard navigation
- Tab navigation
- Focus visibility
- Native interactive elements
- Form labels
- Table headers

### Browser DevTools

- Element inspection
- CSS inspection
- Computed styles
- Box model
- Flexbox
- Grid
- Responsive/device mode

---

# 🚫 JavaScript

JavaScript is **not included** in this project.

This is intentional.

The project is designed to build a strong understanding of:

```text
HTML
  +
CSS
  +
Browser behavior
```

before introducing JavaScript or frontend frameworks.

Therefore, there is no:

```text
script.js
```

or JavaScript framework in this project.

---

# 🔮 Future Enhancements

JavaScript can be introduced in a future version to provide dynamic behavior such as:

- Dynamic user search
- Adding/removing users
- Form submission handling
- Dynamic success/error messages
- Dashboard statistics
- User filtering
- Settings interactions
- API integration

These features are intentionally outside the scope of the current HTML/CSS project.

---

# 📚 Learning Progress

### Already Practiced

- HTML fundamentals
- Semantic HTML
- Forms
- Tables
- Native interactive elements
- HTML accessibility
- CSS fundamentals
- CSS cascade
- Box model
- Typography
- Colors
- Borders
- Shadows
- CSS variables
- Design tokens
- Flexbox
- Form styling
- Table styling
- CSS architecture
- Keyboard accessibility
- Focus accessibility
- Browser DevTools
- Responsive design implementation and testing

### Introduced / Needs More Dedicated Practice

- CSS Grid
- Media queries

CSS Grid and media queries were implemented in AdminKit Lite, but additional small projects will be used to practice these concepts more deeply.

---

# 🚀 How to Run

No installation or build process is required.

Open:

```text
index.html
```

in a modern web browser.

Then use the navigation links to move between:

```text
Dashboard
Users
Settings
Registration
```

---

# 📌 Project Status

**Completed ✅**

AdminKit Lite currently includes:

- ✅ Four HTML pages
- ✅ Semantic HTML
- ✅ Forms
- ✅ Tables
- ✅ Native interactive elements
- ✅ Accessibility features
- ✅ Organized CSS architecture
- ✅ CSS custom properties
- ✅ Design tokens
- ✅ Flexbox
- ✅ CSS Grid
- ✅ Responsive design
- ✅ Media queries
- ✅ DevTools testing
- ✅ Responsive testing
- ✅ Accessibility testing
- ❌ JavaScript — intentionally excluded

---

# 👨‍💻 Author

**Raghavendra**

**Project:** AdminKit Lite  
**Technologies:** HTML5 + CSS3  
**Project Type:** Framework-free frontend practice project