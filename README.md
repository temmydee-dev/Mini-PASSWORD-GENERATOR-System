# PassVault – Modern Password Generator

PassVault is a clean, modern, and user-friendly password generator built with HTML, CSS, and JavaScript.
It allows users to generate secure passwords based on customizable criteria, with a polished UI, dark mode support, and smooth user feedback.

## Features

- **Custom Password Length** (e.g 4)
- **Character Type Selection**
  - Uppercase letters
  - Lowercase letters
  - Numbers
  - Symbols
- **Light & Dark Mode Toggle** (saved in localStorage)
- **One-Click Copy to Clipboard**
- **Toast Notifications** for actions and errors
- **Modern UI** with soft shadows and smooth animations
- **Validation Handling**
  - Prevents generating passwords when no options are selected

## Live Demo
[text](https://temmydee-dev.github.io/Mini-PASSWORD-GENERATOR-System/)


## Built With

- **HTML5** – Markup & structure
- **CSS3** – Custom properties, modern UI styling, light/dark themes
- **JavaScript** – Password logic, validations, clipboard handling

No frameworks or external dependencies required.

## Project Structure
PassVault/
│
├── index.html (Main HTML structure)
├── style.css (Styling light/dark themes, layout, UI)
├── script.js Password generation & interactions
└── README.md Project documentation

## How It Works
1. User selects password length and character types.
2. Each character type maps to a generator function:
   - Lowercase
   - Uppercase
   - Number
   - Symbol
3. Selected generators are looped through until the desired length is reached.
4. The final password is trimmed to match the chosen length.
5. A validation check ensures at least one character type is selected before generation to prevent errors.

### Validation & UX Handling

- Prevents infinite loops when all checkboxes are unchecked
- Displays toast messages instead of intrusive alerts
- Confirms successful copy actions
- Warns when there's nothing to copy

### Dark Mode

- Toggle switch allows users to switch between Light and Dark mode
- Theme preference is saved using localStorage
- Automatically restores the selected theme on reload

### Copy to Clipboard

- Uses the modern Clipboard API
- One click copies the generated password
- Visual feedback confirms the action

### Responsiveness

- Fully responsive for small screens
- Mobile-friendly spacing and layout
- Clean scaling for devices under 400px width
