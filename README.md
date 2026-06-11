# To Do List

A simple, clean to-do list web app built with vanilla HTML, CSS, and JavaScript.

## Features

- **Add tasks** — type a task in the input field and press Enter to add it to the list
- **Complete tasks** — click the green check icon to mark a task as done (strikethrough styling)
- **Delete tasks** — click the red trash icon to remove a task
- **Persistent storage** — tasks are saved to `localStorage`, so they survive page refreshes and browser restarts

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML | Page structure and form |
| CSS | Styling and layout |
| JavaScript | App logic and localStorage interaction |
| Font Awesome 6 | Check and trash icons |

## How to Run

No build step or server needed. Just open `index.html` in any modern browser:

```
index.html   ← open this file
```

Or drag and drop `index.html` into your browser window.

## Project Structure

```
To do List/
├── index.html   # App markup
├── style.css    # Styles
└── index.js     # App logic
```

## How It Works

1. On page load, existing tasks are read from `localStorage` and rendered.
2. Submitting the form calls `toDoList()`, which creates a new `<li>` element with check and delete buttons.
3. Clicking the check button toggles the `checked` class (strikethrough + gray color).
4. Clicking the trash button removes the `<li>` from the DOM.
5. After every change, `updateLocalStorage()` serializes the current task list (name + checked state) back to `localStorage`.

## Screenshots

> Green background with a centered yellow card. Tasks appear below the input field separated by dotted borders, with a green check icon and red trash icon on the right of each task.

## Author

Made by **dilnadev**
