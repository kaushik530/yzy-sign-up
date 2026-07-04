# YZY Sign-Up Form

A responsive sign-up form inspired by YEEZY visual design and created as part of The Odin Project curriculum.

The project focuses on HTML form structure, CSS Flexbox, responsive layouts, form validation states, custom typography, and background image styling.

## Preview

The page consists of:

- A responsive image banner with YZY branding
- Image attribution
- A two-column registration form
- Responsive form layout for narrow screens
- Styled password validation states
- Account creation and login UI

## Built With

- HTML5
- CSS3
- Flexbox
- Media Queries
- HTML Form Validation
- CSS Pseudo-classes
- Custom Web Fonts

## Features

### Responsive Layout

The desktop layout uses two main sections:

    ┌────────────────┬──────────────────────────┐
    │                │                          │
    │  IMAGE BANNER  │      SIGN-UP FORM        │
    │                │                          │
    └────────────────┴──────────────────────────┘

At smaller viewport widths, the layout changes to:

    ┌──────────────────────────┐
    │       IMAGE BANNER       │
    ├──────────────────────────┤
    │       SIGN-UP FORM       │
    └──────────────────────────┘

The form fields also change from two columns to a single-column layout.

### Form Fields

The form contains fields for:

- First name
- Last name
- Email
- Phone number
- Password
- Password confirmation

### Password Validation Styling

Password fields use HTML validation together with CSS pseudo-classes:

    input[type="password"]:invalid {
        border: 2px solid red;
    }

    input[type="password"]:valid {
        border: 2px solid green;
    }

This provides visual feedback based on the validity of password inputs.

## Concepts Practiced

This project helped me practice:

- Creating page layouts with Flexbox
- Using nested flex containers
- Understanding the main axis and cross axis
- Using `flex-direction`
- Using `justify-content` and `align-items`
- Using automatic margins in Flexbox
- Understanding `height` versus `min-height`
- Building responsive layouts with media queries
- Creating responsive sizing with `clamp()`
- Controlling background images with `background-size` and `background-position`
- Handling text overflow with `white-space`, `overflow`, and `text-overflow`
- Styling valid and invalid form states
- Associating labels with form inputs
- Using custom fonts

## Responsive Behavior

The project uses a media query to switch layouts when the available viewport width becomes limited:

    @media (max-width: 700px) {
        form {
            flex-direction: column;
        }

        .main {
            flex-direction: column;
        }

        .banner,
        .formArea {
            width: 100%;
        }
    }

This allows both the page layout and form layout to adapt to smaller screens.

## Image Credit

Background image credited to Mike Apostolakis and sourced via Pinterest.

## Future Improvements

Potential improvements include:

- JavaScript password matching validation
- More detailed validation messages
- Improved keyboard accessibility
- Better mobile spacing and typography
- Form submission handling
- Improved focus states
- Additional responsive breakpoints

## Acknowledgements

Created as part of The Odin Project Sign-Up Form project.
