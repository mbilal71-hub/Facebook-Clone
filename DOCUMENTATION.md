# Project Documentation

This document provides a detailed overview of the Facebook Clone project structure and customization options.

## Project Structure

The project references a standard web development structure with Tailwind CSS.

```
Facebook Clone/
├── node_modules/       # Dependencies installed via npm
├── src/                # Source files
│   ├── imgs/           # Image assets
│   ├── index.html      # Main HTML file
│   ├── input.css       # Tailwind CSS entry point
│   └── output.css      # Compiled CSS file (generated)
├── package.json        # Project metadata and scripts
├── package-lock.json   # Exact dependency versions
├── README.md           # Quick start guide
└── DOCUMENTATION.md    # This detailed documentation
```

## detailed File Descriptions

### `src/index.html`
The main entry point of the application. It contains the HTML structure of the Facebook page clone. It links to `output.css` for styling.

### `src/input.css`
This file contains the `@import "tailwindcss";` directive and is used as the source for generating the utility classes. You can add custom CSS rules here if needed.

### `package.json`
Manages project dependencies, specifically `tailwindcss` and `@tailwindcss/cli`.

## Tailwind CSS Setup

This project uses Tailwind CSS v4. The setup is lightweight and relies on the Tailwind CLI.

**Key Command:**
```bash
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```
- `-i`: Input file (`src/input.css`)
- `-o`: Output file (`src/output.css`)
- `--watch`: Rebuilds the CSS automatically when changes are detected in source files.

## Customization

To customize the look and feel:

1.  **Modify HTML**: Update classes in `src/index.html`.
2.  **Add Custom CSS**: Add your custom CSS rules in `src/input.css`.
3.  **Images**: Place new images in `src/imgs/` and reference them in your HTML.

## Troubleshooting

- **CSS not reflecting changes?**
  Ensure the `--watch` command is running in your terminal.
- **Missing styles?**
  Check that `src/output.css` is correctly linked in your `src/index.html` file:
  ```html
  <link href="./output.css" rel="stylesheet">
  ```
