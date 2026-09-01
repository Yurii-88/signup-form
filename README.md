# Signup Form

A modern, responsive signup form built with HTML and CSS. This project features a clean two-column layout with a visually appealing design and comprehensive form validation.

## Overview

This is a fully functional signup form with a professional design that includes user authentication fields and proper form handling. The form is inspired by The Odin Project's curriculum and demonstrates modern web development best practices.

## Features

- **Responsive Layout** — Two-column design with sidebar and main content area
- **Form Validation** — Built-in HTML5 validation for email and phone fields
- **Accessibility** — Proper label associations, required attributes, and autocomplete hints
- **Custom Styling** — Comic Relief font, custom colors, and smooth spacing
- **User Feedback** — Visual feedback for invalid inputs with red border highlighting
- **Professional Design** — Clean typography, proper spacing, and modern color scheme

## Project Structure

```
.
├── index.html          # Main HTML file with form structure
├── style.css           # CSS styling with nested selectors
├── images/             # Image directory
│   ├── halie-west-25xggax4bSA-unsplash.jpg  # Sidebar background
│   └── odin-lined.png                        # Logo
└── README.md          # Project documentation
```

## Technologies Used

- **HTML5** — Semantic markup with form elements
- **CSS3** — Modern CSS with native nesting support
- **Google Fonts** — Comic Relief font family

## Form Fields

The form collects the following information:

| Field            | Type     | Validation                  | Autocomplete   |
| ---------------- | -------- | --------------------------- | -------------- |
| First Name       | Text     | Required                    | `given-name`   |
| Last Name        | Text     | Required                    | `family-name`  |
| Email            | Email    | Required, format validation | `email`        |
| Phone Number     | Tel      | Required, numeric pattern   | `tel`          |
| Password         | Password | Required                    | `new-password` |
| Confirm Password | Password | Required                    | `new-password` |

## Key Features Explained

### HTML Validation

- Email input uses `type="email"` for format validation
- Phone input uses `pattern="[0-9\s]+"` to allow only numbers and spaces
- All fields are marked as `required`

### Accessibility

- All labels are properly connected to inputs using `for` and `id` attributes
- Autocomplete attributes provide browser hints for better UX
- Semantic HTML structure for screen readers

### Visual Feedback

- Invalid inputs display a red border using the `:user-invalid` pseudo-class
- Clear focus states for better keyboard navigation
- Professional color scheme with green accent color (#596d48)

### Responsive Fonts

- Used `rem` units for scalable typography
- Comic Relief font for distinctive branding
- Fallback to system-ui and sans-serif for compatibility

## Browser Support

- Chrome 120+
- Firefox 121+
- Safari 17.2+
- Edge 120+

All modern browsers with support for:

- CSS nesting
- `:user-invalid` pseudo-class
- Flexbox layout

## Setup & Usage

1. Clone or download the project
2. Ensure the `images/` directory contains the required images
3. Open `index.html` in a web browser
4. Fill out the form to see validation in action

### Testing Validation

1. **Email validation**: Type invalid text (e.g., "abc") and blur the field
2. **Phone validation**: Type non-numeric characters
3. **Required fields**: Try to submit without filling a field
4. The input border will turn red for invalid entries

## CSS Architecture

The stylesheet uses modern CSS nesting for organized, readable code:

```css
.container {
  display: flex;

  .sidebar {
    /* Sidebar styles */
  }

  .main-content {
    /* Main content styles */
  }
}
```

Key styling decisions:

- Flexbox for layout flexibility
- Shadow effect on form inputs for depth
- Proper spacing with `gap` and `padding` properties
- Nested selectors for logical code organization

## Color Scheme

- Primary Button: `#596d48` (sage green)
- Text: Default black
- Borders: `#ccc` (light gray)
- Invalid State: Red
- Background: `rgba(0, 0, 0, 0.03)` (subtle dark overlay)

## Future Enhancements

- Add client-side password matching validation
- Implement form submission handling with JavaScript
- Add success message after form submission
- Enhance mobile responsiveness with media queries
- Add password strength indicator
- Implement loading state for submit button

## Credits

- Background image by [Halie West](https://unsplash.com/) on Unsplash
- Logo: Odin Project branding
- Font: Comic Relief from Google Fonts

## Notes

- This is a front-end form only; backend integration required for actual form submission
- Passwords are not encrypted; use proper security measures in production
- Phone number validation is basic; customize the pattern as needed for your region
