# Facebook Clone

A responsive Facebook Clone built using HTML and Tailwind CSS (v4).

## Features

- **Responsive Design**: Adapts to different screen sizes.
- **Modern UI**: Styled with Tailwind CSS for a sleek look.
- **Project Structure**: Organized source files.

## Technologies Used

- **HTML5**: Markup structure.
- **Tailwind CSS (v4)**: Utility-first CSS framework for styling.

## Setup Instructions

1.  **Install Dependencies**
    Ensure you have Node.js installed. Run the following command to install the necessary packages:
    ```bash
    npm install
    ```

2.  **Start the Development Server / Build CSS**
    Use the Tailwind CLI to verify the build process:
    ```bash
    npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
    ```
    or simply:
    ```bash
    npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
    ```

## Usage

- Open `src/index.html` in your browser to view the application.
- Edit files in `src/` to make changes. The CSS will rebuild if you are running the watch command.

## License

This project is licensed under the MIT License.
